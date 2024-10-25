# Type definitions

> [Index](../README.md) > [Route53Domains](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Route53Domains](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
    type annotations stubs module [types-aiobotocore-route53domains](https://pypi.org/project/types-aiobotocore-route53domains/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## NameserverUnionTypeDef

```python
# NameserverUnionTypeDef definition

NameserverUnionTypeDef = Union[
    NameserverTypeDef,  # (1)
    NameserverOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NameserverTypeDef](./type_defs.md#nameservertypedef) 
2. See [:material-code-braces: NameserverOutputTypeDef](./type_defs.md#nameserveroutputtypedef) 



## AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef

```python
# AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef definition

class AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef(TypedDict):
    DomainName: str,
    Password: str,
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

## DnssecSigningAttributesTypeDef

```python
# DnssecSigningAttributesTypeDef definition

class DnssecSigningAttributesTypeDef(TypedDict):
    Algorithm: NotRequired[int],
    Flags: NotRequired[int],
    PublicKey: NotRequired[str],
```

## BillingRecordTypeDef

```python
# BillingRecordTypeDef definition

class BillingRecordTypeDef(TypedDict):
    DomainName: NotRequired[str],
    Operation: NotRequired[OperationTypeType],  # (1)
    InvoiceId: NotRequired[str],
    BillDate: NotRequired[datetime],
    Price: NotRequired[float],
```

1. See [:material-code-brackets: OperationTypeType](./literals.md#operationtypetype) 
## CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef

```python
# CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef definition

class CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## CheckDomainAvailabilityRequestRequestTypeDef

```python
# CheckDomainAvailabilityRequestRequestTypeDef definition

class CheckDomainAvailabilityRequestRequestTypeDef(TypedDict):
    DomainName: str,
    IdnLangCode: NotRequired[str],
```

## CheckDomainTransferabilityRequestRequestTypeDef

```python
# CheckDomainTransferabilityRequestRequestTypeDef definition

class CheckDomainTransferabilityRequestRequestTypeDef(TypedDict):
    DomainName: str,
    AuthCode: NotRequired[str],
```

## DomainTransferabilityTypeDef

```python
# DomainTransferabilityTypeDef definition

class DomainTransferabilityTypeDef(TypedDict):
    Transferable: NotRequired[TransferableType],  # (1)
```

1. See [:material-code-brackets: TransferableType](./literals.md#transferabletype) 
## ConsentTypeDef

```python
# ConsentTypeDef definition

class ConsentTypeDef(TypedDict):
    MaxPrice: float,
    Currency: str,
```

## ExtraParamTypeDef

```python
# ExtraParamTypeDef definition

class ExtraParamTypeDef(TypedDict):
    Name: ExtraParamNameType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: ExtraParamNameType](./literals.md#extraparamnametype) 
## DeleteDomainRequestRequestTypeDef

```python
# DeleteDomainRequestRequestTypeDef definition

class DeleteDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DeleteTagsForDomainRequestRequestTypeDef

```python
# DeleteTagsForDomainRequestRequestTypeDef definition

class DeleteTagsForDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    TagsToDelete: Sequence[str],
```

## DisableDomainAutoRenewRequestRequestTypeDef

```python
# DisableDomainAutoRenewRequestRequestTypeDef definition

class DisableDomainAutoRenewRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DisableDomainTransferLockRequestRequestTypeDef

```python
# DisableDomainTransferLockRequestRequestTypeDef definition

class DisableDomainTransferLockRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DisassociateDelegationSignerFromDomainRequestRequestTypeDef

```python
# DisassociateDelegationSignerFromDomainRequestRequestTypeDef definition

class DisassociateDelegationSignerFromDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    Id: str,
```

## DnssecKeyTypeDef

```python
# DnssecKeyTypeDef definition

class DnssecKeyTypeDef(TypedDict):
    Algorithm: NotRequired[int],
    Flags: NotRequired[int],
    PublicKey: NotRequired[str],
    DigestType: NotRequired[int],
    Digest: NotRequired[str],
    KeyTag: NotRequired[int],
    Id: NotRequired[str],
```

## PriceWithCurrencyTypeDef

```python
# PriceWithCurrencyTypeDef definition

class PriceWithCurrencyTypeDef(TypedDict):
    Price: float,
    Currency: str,
```

## DomainSuggestionTypeDef

```python
# DomainSuggestionTypeDef definition

class DomainSuggestionTypeDef(TypedDict):
    DomainName: NotRequired[str],
    Availability: NotRequired[str],
```

## DomainSummaryTypeDef

```python
# DomainSummaryTypeDef definition

class DomainSummaryTypeDef(TypedDict):
    DomainName: NotRequired[str],
    AutoRenew: NotRequired[bool],
    TransferLock: NotRequired[bool],
    Expiry: NotRequired[datetime],
```

## EnableDomainAutoRenewRequestRequestTypeDef

```python
# EnableDomainAutoRenewRequestRequestTypeDef definition

class EnableDomainAutoRenewRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## EnableDomainTransferLockRequestRequestTypeDef

```python
# EnableDomainTransferLockRequestRequestTypeDef definition

class EnableDomainTransferLockRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## FilterConditionTypeDef

```python
# FilterConditionTypeDef definition

class FilterConditionTypeDef(TypedDict):
    Name: ListDomainsAttributeNameType,  # (1)
    Operator: OperatorType,  # (2)
    Values: Sequence[str],
```

1. See [:material-code-brackets: ListDomainsAttributeNameType](./literals.md#listdomainsattributenametype) 
2. See [:material-code-brackets: OperatorType](./literals.md#operatortype) 
## GetContactReachabilityStatusRequestRequestTypeDef

```python
# GetContactReachabilityStatusRequestRequestTypeDef definition

class GetContactReachabilityStatusRequestRequestTypeDef(TypedDict):
    domainName: NotRequired[str],
```

## GetDomainDetailRequestRequestTypeDef

```python
# GetDomainDetailRequestRequestTypeDef definition

class GetDomainDetailRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## NameserverOutputTypeDef

```python
# NameserverOutputTypeDef definition

class NameserverOutputTypeDef(TypedDict):
    Name: str,
    GlueIps: NotRequired[List[str]],
```

## GetDomainSuggestionsRequestRequestTypeDef

```python
# GetDomainSuggestionsRequestRequestTypeDef definition

class GetDomainSuggestionsRequestRequestTypeDef(TypedDict):
    DomainName: str,
    SuggestionCount: int,
    OnlyAvailable: bool,
```

## GetOperationDetailRequestRequestTypeDef

```python
# GetOperationDetailRequestRequestTypeDef definition

class GetOperationDetailRequestRequestTypeDef(TypedDict):
    OperationId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## SortConditionTypeDef

```python
# SortConditionTypeDef definition

class SortConditionTypeDef(TypedDict):
    Name: ListDomainsAttributeNameType,  # (1)
    SortOrder: SortOrderType,  # (2)
```

1. See [:material-code-brackets: ListDomainsAttributeNameType](./literals.md#listdomainsattributenametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## OperationSummaryTypeDef

```python
# OperationSummaryTypeDef definition

class OperationSummaryTypeDef(TypedDict):
    OperationId: NotRequired[str],
    Status: NotRequired[OperationStatusType],  # (1)
    Type: NotRequired[OperationTypeType],  # (2)
    SubmittedDate: NotRequired[datetime],
    DomainName: NotRequired[str],
    Message: NotRequired[str],
    StatusFlag: NotRequired[StatusFlagType],  # (3)
    LastUpdatedDate: NotRequired[datetime],
```

1. See [:material-code-brackets: OperationStatusType](./literals.md#operationstatustype) 
2. See [:material-code-brackets: OperationTypeType](./literals.md#operationtypetype) 
3. See [:material-code-brackets: StatusFlagType](./literals.md#statusflagtype) 
## ListPricesRequestRequestTypeDef

```python
# ListPricesRequestRequestTypeDef definition

class ListPricesRequestRequestTypeDef(TypedDict):
    Tld: NotRequired[str],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ListTagsForDomainRequestRequestTypeDef

```python
# ListTagsForDomainRequestRequestTypeDef definition

class ListTagsForDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## NameserverTypeDef

```python
# NameserverTypeDef definition

class NameserverTypeDef(TypedDict):
    Name: str,
    GlueIps: NotRequired[Sequence[str]],
```

## PushDomainRequestRequestTypeDef

```python
# PushDomainRequestRequestTypeDef definition

class PushDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    Target: str,
```

## RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef

```python
# RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef definition

class RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## RenewDomainRequestRequestTypeDef

```python
# RenewDomainRequestRequestTypeDef definition

class RenewDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    CurrentExpiryYear: int,
    DurationInYears: NotRequired[int],
```

## ResendContactReachabilityEmailRequestRequestTypeDef

```python
# ResendContactReachabilityEmailRequestRequestTypeDef definition

class ResendContactReachabilityEmailRequestRequestTypeDef(TypedDict):
    domainName: NotRequired[str],
```

## ResendOperationAuthorizationRequestRequestTypeDef

```python
# ResendOperationAuthorizationRequestRequestTypeDef definition

class ResendOperationAuthorizationRequestRequestTypeDef(TypedDict):
    OperationId: str,
```

## RetrieveDomainAuthCodeRequestRequestTypeDef

```python
# RetrieveDomainAuthCodeRequestRequestTypeDef definition

class RetrieveDomainAuthCodeRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## TransferDomainToAnotherAwsAccountRequestRequestTypeDef

```python
# TransferDomainToAnotherAwsAccountRequestRequestTypeDef definition

class TransferDomainToAnotherAwsAccountRequestRequestTypeDef(TypedDict):
    DomainName: str,
    AccountId: str,
```

## UpdateDomainContactPrivacyRequestRequestTypeDef

```python
# UpdateDomainContactPrivacyRequestRequestTypeDef definition

class UpdateDomainContactPrivacyRequestRequestTypeDef(TypedDict):
    DomainName: str,
    AdminPrivacy: NotRequired[bool],
    RegistrantPrivacy: NotRequired[bool],
    TechPrivacy: NotRequired[bool],
    BillingPrivacy: NotRequired[bool],
```

## AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef

```python
# AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef definition

class AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateDelegationSignerToDomainResponseTypeDef

```python
# AssociateDelegationSignerToDomainResponseTypeDef definition

class AssociateDelegationSignerToDomainResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelDomainTransferToAnotherAwsAccountResponseTypeDef

```python
# CancelDomainTransferToAnotherAwsAccountResponseTypeDef definition

class CancelDomainTransferToAnotherAwsAccountResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CheckDomainAvailabilityResponseTypeDef

```python
# CheckDomainAvailabilityResponseTypeDef definition

class CheckDomainAvailabilityResponseTypeDef(TypedDict):
    Availability: DomainAvailabilityType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DomainAvailabilityType](./literals.md#domainavailabilitytype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDomainResponseTypeDef

```python
# DeleteDomainResponseTypeDef definition

class DeleteDomainResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableDomainTransferLockResponseTypeDef

```python
# DisableDomainTransferLockResponseTypeDef definition

class DisableDomainTransferLockResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateDelegationSignerFromDomainResponseTypeDef

```python
# DisassociateDelegationSignerFromDomainResponseTypeDef definition

class DisassociateDelegationSignerFromDomainResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableDomainTransferLockResponseTypeDef

```python
# EnableDomainTransferLockResponseTypeDef definition

class EnableDomainTransferLockResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContactReachabilityStatusResponseTypeDef

```python
# GetContactReachabilityStatusResponseTypeDef definition

class GetContactReachabilityStatusResponseTypeDef(TypedDict):
    domainName: str,
    status: ReachabilityStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ReachabilityStatusType](./literals.md#reachabilitystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOperationDetailResponseTypeDef

```python
# GetOperationDetailResponseTypeDef definition

class GetOperationDetailResponseTypeDef(TypedDict):
    OperationId: str,
    Status: OperationStatusType,  # (1)
    Message: str,
    DomainName: str,
    Type: OperationTypeType,  # (2)
    SubmittedDate: datetime,
    LastUpdatedDate: datetime,
    StatusFlag: StatusFlagType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: OperationStatusType](./literals.md#operationstatustype) 
2. See [:material-code-brackets: OperationTypeType](./literals.md#operationtypetype) 
3. See [:material-code-brackets: StatusFlagType](./literals.md#statusflagtype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterDomainResponseTypeDef

```python
# RegisterDomainResponseTypeDef definition

class RegisterDomainResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RejectDomainTransferFromAnotherAwsAccountResponseTypeDef

```python
# RejectDomainTransferFromAnotherAwsAccountResponseTypeDef definition

class RejectDomainTransferFromAnotherAwsAccountResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RenewDomainResponseTypeDef

```python
# RenewDomainResponseTypeDef definition

class RenewDomainResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResendContactReachabilityEmailResponseTypeDef

```python
# ResendContactReachabilityEmailResponseTypeDef definition

class ResendContactReachabilityEmailResponseTypeDef(TypedDict):
    domainName: str,
    emailAddress: str,
    isAlreadyVerified: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RetrieveDomainAuthCodeResponseTypeDef

```python
# RetrieveDomainAuthCodeResponseTypeDef definition

class RetrieveDomainAuthCodeResponseTypeDef(TypedDict):
    AuthCode: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransferDomainResponseTypeDef

```python
# TransferDomainResponseTypeDef definition

class TransferDomainResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransferDomainToAnotherAwsAccountResponseTypeDef

```python
# TransferDomainToAnotherAwsAccountResponseTypeDef definition

class TransferDomainToAnotherAwsAccountResponseTypeDef(TypedDict):
    OperationId: str,
    Password: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainContactPrivacyResponseTypeDef

```python
# UpdateDomainContactPrivacyResponseTypeDef definition

class UpdateDomainContactPrivacyResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainContactResponseTypeDef

```python
# UpdateDomainContactResponseTypeDef definition

class UpdateDomainContactResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainNameserversResponseTypeDef

```python
# UpdateDomainNameserversResponseTypeDef definition

class UpdateDomainNameserversResponseTypeDef(TypedDict):
    OperationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateDelegationSignerToDomainRequestRequestTypeDef

```python
# AssociateDelegationSignerToDomainRequestRequestTypeDef definition

class AssociateDelegationSignerToDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    SigningAttributes: DnssecSigningAttributesTypeDef,  # (1)
```

1. See [:material-code-braces: DnssecSigningAttributesTypeDef](./type_defs.md#dnssecsigningattributestypedef) 
## ViewBillingResponseTypeDef

```python
# ViewBillingResponseTypeDef definition

class ViewBillingResponseTypeDef(TypedDict):
    NextPageMarker: str,
    BillingRecords: List[BillingRecordTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BillingRecordTypeDef](./type_defs.md#billingrecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CheckDomainTransferabilityResponseTypeDef

```python
# CheckDomainTransferabilityResponseTypeDef definition

class CheckDomainTransferabilityResponseTypeDef(TypedDict):
    Transferability: DomainTransferabilityTypeDef,  # (1)
    Message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainTransferabilityTypeDef](./type_defs.md#domaintransferabilitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContactDetailOutputTypeDef

```python
# ContactDetailOutputTypeDef definition

class ContactDetailOutputTypeDef(TypedDict):
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    ContactType: NotRequired[ContactTypeType],  # (1)
    OrganizationName: NotRequired[str],
    AddressLine1: NotRequired[str],
    AddressLine2: NotRequired[str],
    City: NotRequired[str],
    State: NotRequired[str],
    CountryCode: NotRequired[CountryCodeType],  # (2)
    ZipCode: NotRequired[str],
    PhoneNumber: NotRequired[str],
    Email: NotRequired[str],
    Fax: NotRequired[str],
    ExtraParams: NotRequired[List[ExtraParamTypeDef]],  # (3)
```

1. See [:material-code-brackets: ContactTypeType](./literals.md#contacttypetype) 
2. See [:material-code-brackets: CountryCodeType](./literals.md#countrycodetype) 
3. See [:material-code-braces: ExtraParamTypeDef](./type_defs.md#extraparamtypedef) 
## ContactDetailTypeDef

```python
# ContactDetailTypeDef definition

class ContactDetailTypeDef(TypedDict):
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    ContactType: NotRequired[ContactTypeType],  # (1)
    OrganizationName: NotRequired[str],
    AddressLine1: NotRequired[str],
    AddressLine2: NotRequired[str],
    City: NotRequired[str],
    State: NotRequired[str],
    CountryCode: NotRequired[CountryCodeType],  # (2)
    ZipCode: NotRequired[str],
    PhoneNumber: NotRequired[str],
    Email: NotRequired[str],
    Fax: NotRequired[str],
    ExtraParams: NotRequired[Sequence[ExtraParamTypeDef]],  # (3)
```

1. See [:material-code-brackets: ContactTypeType](./literals.md#contacttypetype) 
2. See [:material-code-brackets: CountryCodeType](./literals.md#countrycodetype) 
3. See [:material-code-braces: ExtraParamTypeDef](./type_defs.md#extraparamtypedef) 
## DomainPriceTypeDef

```python
# DomainPriceTypeDef definition

class DomainPriceTypeDef(TypedDict):
    Name: NotRequired[str],
    RegistrationPrice: NotRequired[PriceWithCurrencyTypeDef],  # (1)
    TransferPrice: NotRequired[PriceWithCurrencyTypeDef],  # (1)
    RenewalPrice: NotRequired[PriceWithCurrencyTypeDef],  # (1)
    ChangeOwnershipPrice: NotRequired[PriceWithCurrencyTypeDef],  # (1)
    RestorationPrice: NotRequired[PriceWithCurrencyTypeDef],  # (1)
```

1. See [:material-code-braces: PriceWithCurrencyTypeDef](./type_defs.md#pricewithcurrencytypedef) 
2. See [:material-code-braces: PriceWithCurrencyTypeDef](./type_defs.md#pricewithcurrencytypedef) 
3. See [:material-code-braces: PriceWithCurrencyTypeDef](./type_defs.md#pricewithcurrencytypedef) 
4. See [:material-code-braces: PriceWithCurrencyTypeDef](./type_defs.md#pricewithcurrencytypedef) 
5. See [:material-code-braces: PriceWithCurrencyTypeDef](./type_defs.md#pricewithcurrencytypedef) 
## GetDomainSuggestionsResponseTypeDef

```python
# GetDomainSuggestionsResponseTypeDef definition

class GetDomainSuggestionsResponseTypeDef(TypedDict):
    SuggestionsList: List[DomainSuggestionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainSuggestionTypeDef](./type_defs.md#domainsuggestiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDomainsResponseTypeDef

```python
# ListDomainsResponseTypeDef definition

class ListDomainsResponseTypeDef(TypedDict):
    Domains: List[DomainSummaryTypeDef],  # (1)
    NextPageMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPricesRequestListPricesPaginateTypeDef

```python
# ListPricesRequestListPricesPaginateTypeDef definition

class ListPricesRequestListPricesPaginateTypeDef(TypedDict):
    Tld: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDomainsRequestListDomainsPaginateTypeDef

```python
# ListDomainsRequestListDomainsPaginateTypeDef definition

class ListDomainsRequestListDomainsPaginateTypeDef(TypedDict):
    FilterConditions: NotRequired[Sequence[FilterConditionTypeDef]],  # (1)
    SortCondition: NotRequired[SortConditionTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterConditionTypeDef](./type_defs.md#filterconditiontypedef) 
2. See [:material-code-braces: SortConditionTypeDef](./type_defs.md#sortconditiontypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDomainsRequestRequestTypeDef

```python
# ListDomainsRequestRequestTypeDef definition

class ListDomainsRequestRequestTypeDef(TypedDict):
    FilterConditions: NotRequired[Sequence[FilterConditionTypeDef]],  # (1)
    SortCondition: NotRequired[SortConditionTypeDef],  # (2)
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

1. See [:material-code-braces: FilterConditionTypeDef](./type_defs.md#filterconditiontypedef) 
2. See [:material-code-braces: SortConditionTypeDef](./type_defs.md#sortconditiontypedef) 
## ListOperationsRequestListOperationsPaginateTypeDef

```python
# ListOperationsRequestListOperationsPaginateTypeDef definition

class ListOperationsRequestListOperationsPaginateTypeDef(TypedDict):
    SubmittedSince: NotRequired[TimestampTypeDef],
    Status: NotRequired[Sequence[OperationStatusType]],  # (1)
    Type: NotRequired[Sequence[OperationTypeType]],  # (2)
    SortBy: NotRequired[ListOperationsSortAttributeNameType],  # (3)
    SortOrder: NotRequired[SortOrderType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: OperationStatusType](./literals.md#operationstatustype) 
2. See [:material-code-brackets: OperationTypeType](./literals.md#operationtypetype) 
3. See [:material-code-brackets: ListOperationsSortAttributeNameType](./literals.md#listoperationssortattributenametype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOperationsRequestRequestTypeDef

```python
# ListOperationsRequestRequestTypeDef definition

class ListOperationsRequestRequestTypeDef(TypedDict):
    SubmittedSince: NotRequired[TimestampTypeDef],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
    Status: NotRequired[Sequence[OperationStatusType]],  # (1)
    Type: NotRequired[Sequence[OperationTypeType]],  # (2)
    SortBy: NotRequired[ListOperationsSortAttributeNameType],  # (3)
    SortOrder: NotRequired[SortOrderType],  # (4)
```

1. See [:material-code-brackets: OperationStatusType](./literals.md#operationstatustype) 
2. See [:material-code-brackets: OperationTypeType](./literals.md#operationtypetype) 
3. See [:material-code-brackets: ListOperationsSortAttributeNameType](./literals.md#listoperationssortattributenametype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ViewBillingRequestRequestTypeDef

```python
# ViewBillingRequestRequestTypeDef definition

class ViewBillingRequestRequestTypeDef(TypedDict):
    Start: NotRequired[TimestampTypeDef],
    End: NotRequired[TimestampTypeDef],
    Marker: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ViewBillingRequestViewBillingPaginateTypeDef

```python
# ViewBillingRequestViewBillingPaginateTypeDef definition

class ViewBillingRequestViewBillingPaginateTypeDef(TypedDict):
    Start: NotRequired[TimestampTypeDef],
    End: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOperationsResponseTypeDef

```python
# ListOperationsResponseTypeDef definition

class ListOperationsResponseTypeDef(TypedDict):
    Operations: List[OperationSummaryTypeDef],  # (1)
    NextPageMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationSummaryTypeDef](./type_defs.md#operationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForDomainResponseTypeDef

```python
# ListTagsForDomainResponseTypeDef definition

class ListTagsForDomainResponseTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTagsForDomainRequestRequestTypeDef

```python
# UpdateTagsForDomainRequestRequestTypeDef definition

class UpdateTagsForDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    TagsToUpdate: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateDomainNameserversRequestRequestTypeDef

```python
# UpdateDomainNameserversRequestRequestTypeDef definition

class UpdateDomainNameserversRequestRequestTypeDef(TypedDict):
    DomainName: str,
    Nameservers: Sequence[NameserverTypeDef],  # (1)
    FIAuthKey: NotRequired[str],
```

1. See [:material-code-braces: NameserverTypeDef](./type_defs.md#nameservertypedef) 
## GetDomainDetailResponseTypeDef

```python
# GetDomainDetailResponseTypeDef definition

class GetDomainDetailResponseTypeDef(TypedDict):
    DomainName: str,
    Nameservers: List[NameserverOutputTypeDef],  # (1)
    AutoRenew: bool,
    AdminContact: ContactDetailOutputTypeDef,  # (2)
    RegistrantContact: ContactDetailOutputTypeDef,  # (2)
    TechContact: ContactDetailOutputTypeDef,  # (2)
    AdminPrivacy: bool,
    RegistrantPrivacy: bool,
    TechPrivacy: bool,
    RegistrarName: str,
    WhoIsServer: str,
    RegistrarUrl: str,
    AbuseContactEmail: str,
    AbuseContactPhone: str,
    RegistryDomainId: str,
    CreationDate: datetime,
    UpdatedDate: datetime,
    ExpirationDate: datetime,
    Reseller: str,
    DnsSec: str,
    StatusList: List[str],
    DnssecKeys: List[DnssecKeyTypeDef],  # (5)
    BillingContact: ContactDetailOutputTypeDef,  # (2)
    BillingPrivacy: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: NameserverOutputTypeDef](./type_defs.md#nameserveroutputtypedef) 
2. See [:material-code-braces: ContactDetailOutputTypeDef](./type_defs.md#contactdetailoutputtypedef) 
3. See [:material-code-braces: ContactDetailOutputTypeDef](./type_defs.md#contactdetailoutputtypedef) 
4. See [:material-code-braces: ContactDetailOutputTypeDef](./type_defs.md#contactdetailoutputtypedef) 
5. See [:material-code-braces: DnssecKeyTypeDef](./type_defs.md#dnsseckeytypedef) 
6. See [:material-code-braces: ContactDetailOutputTypeDef](./type_defs.md#contactdetailoutputtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterDomainRequestRequestTypeDef

```python
# RegisterDomainRequestRequestTypeDef definition

class RegisterDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    DurationInYears: int,
    AdminContact: ContactDetailTypeDef,  # (1)
    RegistrantContact: ContactDetailTypeDef,  # (1)
    TechContact: ContactDetailTypeDef,  # (1)
    IdnLangCode: NotRequired[str],
    AutoRenew: NotRequired[bool],
    PrivacyProtectAdminContact: NotRequired[bool],
    PrivacyProtectRegistrantContact: NotRequired[bool],
    PrivacyProtectTechContact: NotRequired[bool],
    BillingContact: NotRequired[ContactDetailTypeDef],  # (1)
    PrivacyProtectBillingContact: NotRequired[bool],
```

1. See [:material-code-braces: ContactDetailTypeDef](./type_defs.md#contactdetailtypedef) 
2. See [:material-code-braces: ContactDetailTypeDef](./type_defs.md#contactdetailtypedef) 
3. See [:material-code-braces: ContactDetailTypeDef](./type_defs.md#contactdetailtypedef) 
4. See [:material-code-braces: ContactDetailTypeDef](./type_defs.md#contactdetailtypedef) 
## UpdateDomainContactRequestRequestTypeDef

```python
# UpdateDomainContactRequestRequestTypeDef definition

class UpdateDomainContactRequestRequestTypeDef(TypedDict):
    DomainName: str,
    AdminContact: NotRequired[ContactDetailTypeDef],  # (1)
    RegistrantContact: NotRequired[ContactDetailTypeDef],  # (1)
    TechContact: NotRequired[ContactDetailTypeDef],  # (1)
    Consent: NotRequired[ConsentTypeDef],  # (4)
    BillingContact: NotRequired[ContactDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ContactDetailTypeDef](./type_defs.md#contactdetailtypedef) 
2. See [:material-code-braces: ContactDetailTypeDef](./type_defs.md#contactdetailtypedef) 
3. See [:material-code-braces: ContactDetailTypeDef](./type_defs.md#contactdetailtypedef) 
4. See [:material-code-braces: ConsentTypeDef](./type_defs.md#consenttypedef) 
5. See [:material-code-braces: ContactDetailTypeDef](./type_defs.md#contactdetailtypedef) 
## ListPricesResponseTypeDef

```python
# ListPricesResponseTypeDef definition

class ListPricesResponseTypeDef(TypedDict):
    Prices: List[DomainPriceTypeDef],  # (1)
    NextPageMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainPriceTypeDef](./type_defs.md#domainpricetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransferDomainRequestRequestTypeDef

```python
# TransferDomainRequestRequestTypeDef definition

class TransferDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    DurationInYears: int,
    AdminContact: ContactDetailTypeDef,  # (1)
    RegistrantContact: ContactDetailTypeDef,  # (1)
    TechContact: ContactDetailTypeDef,  # (1)
    IdnLangCode: NotRequired[str],
    Nameservers: NotRequired[Sequence[NameserverUnionTypeDef]],  # (4)
    AuthCode: NotRequired[str],
    AutoRenew: NotRequired[bool],
    PrivacyProtectAdminContact: NotRequired[bool],
    PrivacyProtectRegistrantContact: NotRequired[bool],
    PrivacyProtectTechContact: NotRequired[bool],
    BillingContact: NotRequired[ContactDetailTypeDef],  # (1)
    PrivacyProtectBillingContact: NotRequired[bool],
```

1. See [:material-code-braces: ContactDetailTypeDef](./type_defs.md#contactdetailtypedef) 
2. See [:material-code-braces: ContactDetailTypeDef](./type_defs.md#contactdetailtypedef) 
3. See [:material-code-braces: ContactDetailTypeDef](./type_defs.md#contactdetailtypedef) 
4. See [:material-code-braces: NameserverTypeDef](./type_defs.md#nameservertypedef) [:material-code-braces: NameserverOutputTypeDef](./type_defs.md#nameserveroutputtypedef) 
5. See [:material-code-braces: ContactDetailTypeDef](./type_defs.md#contactdetailtypedef) 
