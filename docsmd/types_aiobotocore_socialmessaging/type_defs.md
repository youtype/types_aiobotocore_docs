# Type definitions

> [Index](../README.md) > [EndUserMessagingSocial](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EndUserMessagingSocial](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging.html#endusermessagingsocial)
    type annotations stubs module [types-aiobotocore-socialmessaging](https://pypi.org/project/types-aiobotocore-socialmessaging/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## WhatsAppSignupCallbackTypeDef

```python
# WhatsAppSignupCallbackTypeDef definition

class WhatsAppSignupCallbackTypeDef(TypedDict):
    accessToken: str,
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

## DeleteWhatsAppMessageMediaInputRequestTypeDef

```python
# DeleteWhatsAppMessageMediaInputRequestTypeDef definition

class DeleteWhatsAppMessageMediaInputRequestTypeDef(TypedDict):
    mediaId: str,
    originationPhoneNumberId: str,
```

## DisassociateWhatsAppBusinessAccountInputRequestTypeDef

```python
# DisassociateWhatsAppBusinessAccountInputRequestTypeDef definition

class DisassociateWhatsAppBusinessAccountInputRequestTypeDef(TypedDict):
    id: str,
```

## GetLinkedWhatsAppBusinessAccountInputRequestTypeDef

```python
# GetLinkedWhatsAppBusinessAccountInputRequestTypeDef definition

class GetLinkedWhatsAppBusinessAccountInputRequestTypeDef(TypedDict):
    id: str,
```

## GetLinkedWhatsAppBusinessAccountPhoneNumberInputRequestTypeDef

```python
# GetLinkedWhatsAppBusinessAccountPhoneNumberInputRequestTypeDef definition

class GetLinkedWhatsAppBusinessAccountPhoneNumberInputRequestTypeDef(TypedDict):
    id: str,
```

## WhatsAppPhoneNumberDetailTypeDef

```python
# WhatsAppPhoneNumberDetailTypeDef definition

class WhatsAppPhoneNumberDetailTypeDef(TypedDict):
    arn: str,
    phoneNumber: str,
    phoneNumberId: str,
    metaPhoneNumberId: str,
    displayPhoneNumberName: str,
    displayPhoneNumber: str,
    qualityRating: str,
```

## S3FileTypeDef

```python
# S3FileTypeDef definition

class S3FileTypeDef(TypedDict):
    bucketName: str,
    key: str,
```

## S3PresignedUrlTypeDef

```python
# S3PresignedUrlTypeDef definition

class S3PresignedUrlTypeDef(TypedDict):
    url: str,
    headers: Mapping[str, str],
```

## WhatsAppBusinessAccountEventDestinationTypeDef

```python
# WhatsAppBusinessAccountEventDestinationTypeDef definition

class WhatsAppBusinessAccountEventDestinationTypeDef(TypedDict):
    eventDestinationArn: str,
    roleArn: NotRequired[str],
```

## WhatsAppPhoneNumberSummaryTypeDef

```python
# WhatsAppPhoneNumberSummaryTypeDef definition

class WhatsAppPhoneNumberSummaryTypeDef(TypedDict):
    arn: str,
    phoneNumber: str,
    phoneNumberId: str,
    metaPhoneNumberId: str,
    displayPhoneNumberName: str,
    displayPhoneNumber: str,
    qualityRating: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListLinkedWhatsAppBusinessAccountsInputRequestTypeDef

```python
# ListLinkedWhatsAppBusinessAccountsInputRequestTypeDef definition

class ListLinkedWhatsAppBusinessAccountsInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: NotRequired[str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## DeleteWhatsAppMessageMediaOutputTypeDef

```python
# DeleteWhatsAppMessageMediaOutputTypeDef definition

class DeleteWhatsAppMessageMediaOutputTypeDef(TypedDict):
    success: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWhatsAppMessageMediaOutputTypeDef

```python
# GetWhatsAppMessageMediaOutputTypeDef definition

class GetWhatsAppMessageMediaOutputTypeDef(TypedDict):
    mimeType: str,
    fileSize: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PostWhatsAppMessageMediaOutputTypeDef

```python
# PostWhatsAppMessageMediaOutputTypeDef definition

class PostWhatsAppMessageMediaOutputTypeDef(TypedDict):
    mediaId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendWhatsAppMessageOutputTypeDef

```python
# SendWhatsAppMessageOutputTypeDef definition

class SendWhatsAppMessageOutputTypeDef(TypedDict):
    messageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceOutputTypeDef

```python
# TagResourceOutputTypeDef definition

class TagResourceOutputTypeDef(TypedDict):
    statusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UntagResourceOutputTypeDef

```python
# UntagResourceOutputTypeDef definition

class UntagResourceOutputTypeDef(TypedDict):
    statusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendWhatsAppMessageInputRequestTypeDef

```python
# SendWhatsAppMessageInputRequestTypeDef definition

class SendWhatsAppMessageInputRequestTypeDef(TypedDict):
    originationPhoneNumberId: str,
    message: BlobTypeDef,
    metaApiVersion: str,
```

## GetLinkedWhatsAppBusinessAccountPhoneNumberOutputTypeDef

```python
# GetLinkedWhatsAppBusinessAccountPhoneNumberOutputTypeDef definition

class GetLinkedWhatsAppBusinessAccountPhoneNumberOutputTypeDef(TypedDict):
    phoneNumber: WhatsAppPhoneNumberDetailTypeDef,  # (1)
    linkedWhatsAppBusinessAccountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WhatsAppPhoneNumberDetailTypeDef](./type_defs.md#whatsappphonenumberdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LinkedWhatsAppBusinessAccountIdMetaDataTypeDef

```python
# LinkedWhatsAppBusinessAccountIdMetaDataTypeDef definition

class LinkedWhatsAppBusinessAccountIdMetaDataTypeDef(TypedDict):
    accountName: NotRequired[str],
    registrationStatus: NotRequired[RegistrationStatusType],  # (1)
    unregisteredWhatsAppPhoneNumbers: NotRequired[List[WhatsAppPhoneNumberDetailTypeDef]],  # (2)
    wabaId: NotRequired[str],
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: WhatsAppPhoneNumberDetailTypeDef](./type_defs.md#whatsappphonenumberdetailtypedef) 
## GetWhatsAppMessageMediaInputRequestTypeDef

```python
# GetWhatsAppMessageMediaInputRequestTypeDef definition

class GetWhatsAppMessageMediaInputRequestTypeDef(TypedDict):
    mediaId: str,
    originationPhoneNumberId: str,
    metadataOnly: NotRequired[bool],
    destinationS3PresignedUrl: NotRequired[S3PresignedUrlTypeDef],  # (1)
    destinationS3File: NotRequired[S3FileTypeDef],  # (2)
```

1. See [:material-code-braces: S3PresignedUrlTypeDef](./type_defs.md#s3presignedurltypedef) 
2. See [:material-code-braces: S3FileTypeDef](./type_defs.md#s3filetypedef) 
## PostWhatsAppMessageMediaInputRequestTypeDef

```python
# PostWhatsAppMessageMediaInputRequestTypeDef definition

class PostWhatsAppMessageMediaInputRequestTypeDef(TypedDict):
    originationPhoneNumberId: str,
    sourceS3PresignedUrl: NotRequired[S3PresignedUrlTypeDef],  # (1)
    sourceS3File: NotRequired[S3FileTypeDef],  # (2)
```

1. See [:material-code-braces: S3PresignedUrlTypeDef](./type_defs.md#s3presignedurltypedef) 
2. See [:material-code-braces: S3FileTypeDef](./type_defs.md#s3filetypedef) 
## LinkedWhatsAppBusinessAccountSummaryTypeDef

```python
# LinkedWhatsAppBusinessAccountSummaryTypeDef definition

class LinkedWhatsAppBusinessAccountSummaryTypeDef(TypedDict):
    arn: str,
    id: str,
    wabaId: str,
    registrationStatus: RegistrationStatusType,  # (1)
    linkDate: datetime,
    wabaName: str,
    eventDestinations: List[WhatsAppBusinessAccountEventDestinationTypeDef],  # (2)
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: WhatsAppBusinessAccountEventDestinationTypeDef](./type_defs.md#whatsappbusinessaccounteventdestinationtypedef) 
## PutWhatsAppBusinessAccountEventDestinationsInputRequestTypeDef

```python
# PutWhatsAppBusinessAccountEventDestinationsInputRequestTypeDef definition

class PutWhatsAppBusinessAccountEventDestinationsInputRequestTypeDef(TypedDict):
    id: str,
    eventDestinations: Sequence[WhatsAppBusinessAccountEventDestinationTypeDef],  # (1)
```

1. See [:material-code-braces: WhatsAppBusinessAccountEventDestinationTypeDef](./type_defs.md#whatsappbusinessaccounteventdestinationtypedef) 
## LinkedWhatsAppBusinessAccountTypeDef

```python
# LinkedWhatsAppBusinessAccountTypeDef definition

class LinkedWhatsAppBusinessAccountTypeDef(TypedDict):
    arn: str,
    id: str,
    wabaId: str,
    registrationStatus: RegistrationStatusType,  # (1)
    linkDate: datetime,
    wabaName: str,
    eventDestinations: List[WhatsAppBusinessAccountEventDestinationTypeDef],  # (2)
    phoneNumbers: List[WhatsAppPhoneNumberSummaryTypeDef],  # (3)
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: WhatsAppBusinessAccountEventDestinationTypeDef](./type_defs.md#whatsappbusinessaccounteventdestinationtypedef) 
3. See [:material-code-braces: WhatsAppPhoneNumberSummaryTypeDef](./type_defs.md#whatsappphonenumbersummarytypedef) 
## ListLinkedWhatsAppBusinessAccountsInputPaginateTypeDef

```python
# ListLinkedWhatsAppBusinessAccountsInputPaginateTypeDef definition

class ListLinkedWhatsAppBusinessAccountsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    statusCode: int,
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## WabaPhoneNumberSetupFinalizationTypeDef

```python
# WabaPhoneNumberSetupFinalizationTypeDef definition

class WabaPhoneNumberSetupFinalizationTypeDef(TypedDict):
    id: str,
    twoFactorPin: str,
    dataLocalizationRegion: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## WabaSetupFinalizationTypeDef

```python
# WabaSetupFinalizationTypeDef definition

class WabaSetupFinalizationTypeDef(TypedDict):
    id: NotRequired[str],
    eventDestinations: NotRequired[Sequence[WhatsAppBusinessAccountEventDestinationTypeDef]],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: WhatsAppBusinessAccountEventDestinationTypeDef](./type_defs.md#whatsappbusinessaccounteventdestinationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## WhatsAppSignupCallbackResultTypeDef

```python
# WhatsAppSignupCallbackResultTypeDef definition

class WhatsAppSignupCallbackResultTypeDef(TypedDict):
    associateInProgressToken: NotRequired[str],
    linkedAccountsWithIncompleteSetup: NotRequired[Dict[str, LinkedWhatsAppBusinessAccountIdMetaDataTypeDef]],  # (1)
```

1. See [:material-code-braces: LinkedWhatsAppBusinessAccountIdMetaDataTypeDef](./type_defs.md#linkedwhatsappbusinessaccountidmetadatatypedef) 
## ListLinkedWhatsAppBusinessAccountsOutputTypeDef

```python
# ListLinkedWhatsAppBusinessAccountsOutputTypeDef definition

class ListLinkedWhatsAppBusinessAccountsOutputTypeDef(TypedDict):
    linkedAccounts: List[LinkedWhatsAppBusinessAccountSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LinkedWhatsAppBusinessAccountSummaryTypeDef](./type_defs.md#linkedwhatsappbusinessaccountsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLinkedWhatsAppBusinessAccountOutputTypeDef

```python
# GetLinkedWhatsAppBusinessAccountOutputTypeDef definition

class GetLinkedWhatsAppBusinessAccountOutputTypeDef(TypedDict):
    account: LinkedWhatsAppBusinessAccountTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LinkedWhatsAppBusinessAccountTypeDef](./type_defs.md#linkedwhatsappbusinessaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WhatsAppSetupFinalizationTypeDef

```python
# WhatsAppSetupFinalizationTypeDef definition

class WhatsAppSetupFinalizationTypeDef(TypedDict):
    associateInProgressToken: str,
    phoneNumbers: Sequence[WabaPhoneNumberSetupFinalizationTypeDef],  # (1)
    phoneNumberParent: NotRequired[str],
    waba: NotRequired[WabaSetupFinalizationTypeDef],  # (2)
```

1. See [:material-code-braces: WabaPhoneNumberSetupFinalizationTypeDef](./type_defs.md#wabaphonenumbersetupfinalizationtypedef) 
2. See [:material-code-braces: WabaSetupFinalizationTypeDef](./type_defs.md#wabasetupfinalizationtypedef) 
## AssociateWhatsAppBusinessAccountOutputTypeDef

```python
# AssociateWhatsAppBusinessAccountOutputTypeDef definition

class AssociateWhatsAppBusinessAccountOutputTypeDef(TypedDict):
    signupCallbackResult: WhatsAppSignupCallbackResultTypeDef,  # (1)
    statusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WhatsAppSignupCallbackResultTypeDef](./type_defs.md#whatsappsignupcallbackresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateWhatsAppBusinessAccountInputRequestTypeDef

```python
# AssociateWhatsAppBusinessAccountInputRequestTypeDef definition

class AssociateWhatsAppBusinessAccountInputRequestTypeDef(TypedDict):
    signupCallback: NotRequired[WhatsAppSignupCallbackTypeDef],  # (1)
    setupFinalization: NotRequired[WhatsAppSetupFinalizationTypeDef],  # (2)
```

1. See [:material-code-braces: WhatsAppSignupCallbackTypeDef](./type_defs.md#whatsappsignupcallbacktypedef) 
2. See [:material-code-braces: WhatsAppSetupFinalizationTypeDef](./type_defs.md#whatsappsetupfinalizationtypedef) 
