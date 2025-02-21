# Type definitions

> [Index](../README.md) > [EndUserMessagingSocial](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EndUserMessagingSocial](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging.html#endusermessagingsocial)
    type annotations stubs module [types-aiobotocore-socialmessaging](https://pypi.org/project/types-aiobotocore-socialmessaging/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_socialmessaging.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


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
# WhatsAppSignupCallbackTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import WhatsAppSignupCallbackTypeDef


def get_value() -> WhatsAppSignupCallbackTypeDef:
    return {
        "accessToken": ...,
    }


# WhatsAppSignupCallbackTypeDef definition

class WhatsAppSignupCallbackTypeDef(TypedDict):
    accessToken: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import ResponseMetadataTypeDef


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

## DeleteWhatsAppMessageMediaInputTypeDef

```python
# DeleteWhatsAppMessageMediaInputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import DeleteWhatsAppMessageMediaInputTypeDef


def get_value() -> DeleteWhatsAppMessageMediaInputTypeDef:
    return {
        "mediaId": ...,
    }


# DeleteWhatsAppMessageMediaInputTypeDef definition

class DeleteWhatsAppMessageMediaInputTypeDef(TypedDict):
    mediaId: str,
    originationPhoneNumberId: str,
```

## DisassociateWhatsAppBusinessAccountInputTypeDef

```python
# DisassociateWhatsAppBusinessAccountInputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import DisassociateWhatsAppBusinessAccountInputTypeDef


def get_value() -> DisassociateWhatsAppBusinessAccountInputTypeDef:
    return {
        "id": ...,
    }


# DisassociateWhatsAppBusinessAccountInputTypeDef definition

class DisassociateWhatsAppBusinessAccountInputTypeDef(TypedDict):
    id: str,
```

## GetLinkedWhatsAppBusinessAccountInputTypeDef

```python
# GetLinkedWhatsAppBusinessAccountInputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import GetLinkedWhatsAppBusinessAccountInputTypeDef


def get_value() -> GetLinkedWhatsAppBusinessAccountInputTypeDef:
    return {
        "id": ...,
    }


# GetLinkedWhatsAppBusinessAccountInputTypeDef definition

class GetLinkedWhatsAppBusinessAccountInputTypeDef(TypedDict):
    id: str,
```

## GetLinkedWhatsAppBusinessAccountPhoneNumberInputTypeDef

```python
# GetLinkedWhatsAppBusinessAccountPhoneNumberInputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import GetLinkedWhatsAppBusinessAccountPhoneNumberInputTypeDef


def get_value() -> GetLinkedWhatsAppBusinessAccountPhoneNumberInputTypeDef:
    return {
        "id": ...,
    }


# GetLinkedWhatsAppBusinessAccountPhoneNumberInputTypeDef definition

class GetLinkedWhatsAppBusinessAccountPhoneNumberInputTypeDef(TypedDict):
    id: str,
```

## WhatsAppPhoneNumberDetailTypeDef

```python
# WhatsAppPhoneNumberDetailTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import WhatsAppPhoneNumberDetailTypeDef


def get_value() -> WhatsAppPhoneNumberDetailTypeDef:
    return {
        "arn": ...,
    }


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
# S3FileTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import S3FileTypeDef


def get_value() -> S3FileTypeDef:
    return {
        "bucketName": ...,
    }


# S3FileTypeDef definition

class S3FileTypeDef(TypedDict):
    bucketName: str,
    key: str,
```

## S3PresignedUrlTypeDef

```python
# S3PresignedUrlTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import S3PresignedUrlTypeDef


def get_value() -> S3PresignedUrlTypeDef:
    return {
        "url": ...,
    }


# S3PresignedUrlTypeDef definition

class S3PresignedUrlTypeDef(TypedDict):
    url: str,
    headers: Mapping[str, str],
```

## WhatsAppBusinessAccountEventDestinationTypeDef

```python
# WhatsAppBusinessAccountEventDestinationTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import WhatsAppBusinessAccountEventDestinationTypeDef


def get_value() -> WhatsAppBusinessAccountEventDestinationTypeDef:
    return {
        "eventDestinationArn": ...,
    }


# WhatsAppBusinessAccountEventDestinationTypeDef definition

class WhatsAppBusinessAccountEventDestinationTypeDef(TypedDict):
    eventDestinationArn: str,
    roleArn: NotRequired[str],
```

## WhatsAppPhoneNumberSummaryTypeDef

```python
# WhatsAppPhoneNumberSummaryTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import WhatsAppPhoneNumberSummaryTypeDef


def get_value() -> WhatsAppPhoneNumberSummaryTypeDef:
    return {
        "arn": ...,
    }


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
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import PaginatorConfigTypeDef


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

## ListLinkedWhatsAppBusinessAccountsInputTypeDef

```python
# ListLinkedWhatsAppBusinessAccountsInputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import ListLinkedWhatsAppBusinessAccountsInputTypeDef


def get_value() -> ListLinkedWhatsAppBusinessAccountsInputTypeDef:
    return {
        "nextToken": ...,
    }


# ListLinkedWhatsAppBusinessAccountsInputTypeDef definition

class ListLinkedWhatsAppBusinessAccountsInputTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceInputTypeDef

```python
# ListTagsForResourceInputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import ListTagsForResourceInputTypeDef


def get_value() -> ListTagsForResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceInputTypeDef definition

class ListTagsForResourceInputTypeDef(TypedDict):
    resourceArn: str,
```

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: NotRequired[str],
```

## UntagResourceInputTypeDef

```python
# UntagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import UntagResourceInputTypeDef


def get_value() -> UntagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceInputTypeDef definition

class UntagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## DeleteWhatsAppMessageMediaOutputTypeDef

```python
# DeleteWhatsAppMessageMediaOutputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import DeleteWhatsAppMessageMediaOutputTypeDef


def get_value() -> DeleteWhatsAppMessageMediaOutputTypeDef:
    return {
        "success": ...,
    }


# DeleteWhatsAppMessageMediaOutputTypeDef definition

class DeleteWhatsAppMessageMediaOutputTypeDef(TypedDict):
    success: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWhatsAppMessageMediaOutputTypeDef

```python
# GetWhatsAppMessageMediaOutputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import GetWhatsAppMessageMediaOutputTypeDef


def get_value() -> GetWhatsAppMessageMediaOutputTypeDef:
    return {
        "mimeType": ...,
    }


# GetWhatsAppMessageMediaOutputTypeDef definition

class GetWhatsAppMessageMediaOutputTypeDef(TypedDict):
    mimeType: str,
    fileSize: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PostWhatsAppMessageMediaOutputTypeDef

```python
# PostWhatsAppMessageMediaOutputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import PostWhatsAppMessageMediaOutputTypeDef


def get_value() -> PostWhatsAppMessageMediaOutputTypeDef:
    return {
        "mediaId": ...,
    }


# PostWhatsAppMessageMediaOutputTypeDef definition

class PostWhatsAppMessageMediaOutputTypeDef(TypedDict):
    mediaId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendWhatsAppMessageOutputTypeDef

```python
# SendWhatsAppMessageOutputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import SendWhatsAppMessageOutputTypeDef


def get_value() -> SendWhatsAppMessageOutputTypeDef:
    return {
        "messageId": ...,
    }


# SendWhatsAppMessageOutputTypeDef definition

class SendWhatsAppMessageOutputTypeDef(TypedDict):
    messageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceOutputTypeDef

```python
# TagResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import TagResourceOutputTypeDef


def get_value() -> TagResourceOutputTypeDef:
    return {
        "statusCode": ...,
    }


# TagResourceOutputTypeDef definition

class TagResourceOutputTypeDef(TypedDict):
    statusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UntagResourceOutputTypeDef

```python
# UntagResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import UntagResourceOutputTypeDef


def get_value() -> UntagResourceOutputTypeDef:
    return {
        "statusCode": ...,
    }


# UntagResourceOutputTypeDef definition

class UntagResourceOutputTypeDef(TypedDict):
    statusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendWhatsAppMessageInputTypeDef

```python
# SendWhatsAppMessageInputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import SendWhatsAppMessageInputTypeDef


def get_value() -> SendWhatsAppMessageInputTypeDef:
    return {
        "originationPhoneNumberId": ...,
    }


# SendWhatsAppMessageInputTypeDef definition

class SendWhatsAppMessageInputTypeDef(TypedDict):
    originationPhoneNumberId: str,
    message: BlobTypeDef,
    metaApiVersion: str,
```

## GetLinkedWhatsAppBusinessAccountPhoneNumberOutputTypeDef

```python
# GetLinkedWhatsAppBusinessAccountPhoneNumberOutputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import GetLinkedWhatsAppBusinessAccountPhoneNumberOutputTypeDef


def get_value() -> GetLinkedWhatsAppBusinessAccountPhoneNumberOutputTypeDef:
    return {
        "phoneNumber": ...,
    }


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
# LinkedWhatsAppBusinessAccountIdMetaDataTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import LinkedWhatsAppBusinessAccountIdMetaDataTypeDef


def get_value() -> LinkedWhatsAppBusinessAccountIdMetaDataTypeDef:
    return {
        "accountName": ...,
    }


# LinkedWhatsAppBusinessAccountIdMetaDataTypeDef definition

class LinkedWhatsAppBusinessAccountIdMetaDataTypeDef(TypedDict):
    accountName: NotRequired[str],
    registrationStatus: NotRequired[RegistrationStatusType],  # (1)
    unregisteredWhatsAppPhoneNumbers: NotRequired[List[WhatsAppPhoneNumberDetailTypeDef]],  # (2)
    wabaId: NotRequired[str],
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: WhatsAppPhoneNumberDetailTypeDef](./type_defs.md#whatsappphonenumberdetailtypedef) 
## GetWhatsAppMessageMediaInputTypeDef

```python
# GetWhatsAppMessageMediaInputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import GetWhatsAppMessageMediaInputTypeDef


def get_value() -> GetWhatsAppMessageMediaInputTypeDef:
    return {
        "mediaId": ...,
    }


# GetWhatsAppMessageMediaInputTypeDef definition

class GetWhatsAppMessageMediaInputTypeDef(TypedDict):
    mediaId: str,
    originationPhoneNumberId: str,
    metadataOnly: NotRequired[bool],
    destinationS3PresignedUrl: NotRequired[S3PresignedUrlTypeDef],  # (1)
    destinationS3File: NotRequired[S3FileTypeDef],  # (2)
```

1. See [:material-code-braces: S3PresignedUrlTypeDef](./type_defs.md#s3presignedurltypedef) 
2. See [:material-code-braces: S3FileTypeDef](./type_defs.md#s3filetypedef) 
## PostWhatsAppMessageMediaInputTypeDef

```python
# PostWhatsAppMessageMediaInputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import PostWhatsAppMessageMediaInputTypeDef


def get_value() -> PostWhatsAppMessageMediaInputTypeDef:
    return {
        "originationPhoneNumberId": ...,
    }


# PostWhatsAppMessageMediaInputTypeDef definition

class PostWhatsAppMessageMediaInputTypeDef(TypedDict):
    originationPhoneNumberId: str,
    sourceS3PresignedUrl: NotRequired[S3PresignedUrlTypeDef],  # (1)
    sourceS3File: NotRequired[S3FileTypeDef],  # (2)
```

1. See [:material-code-braces: S3PresignedUrlTypeDef](./type_defs.md#s3presignedurltypedef) 
2. See [:material-code-braces: S3FileTypeDef](./type_defs.md#s3filetypedef) 
## LinkedWhatsAppBusinessAccountSummaryTypeDef

```python
# LinkedWhatsAppBusinessAccountSummaryTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import LinkedWhatsAppBusinessAccountSummaryTypeDef


def get_value() -> LinkedWhatsAppBusinessAccountSummaryTypeDef:
    return {
        "arn": ...,
    }


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
## PutWhatsAppBusinessAccountEventDestinationsInputTypeDef

```python
# PutWhatsAppBusinessAccountEventDestinationsInputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import PutWhatsAppBusinessAccountEventDestinationsInputTypeDef


def get_value() -> PutWhatsAppBusinessAccountEventDestinationsInputTypeDef:
    return {
        "id": ...,
    }


# PutWhatsAppBusinessAccountEventDestinationsInputTypeDef definition

class PutWhatsAppBusinessAccountEventDestinationsInputTypeDef(TypedDict):
    id: str,
    eventDestinations: Sequence[WhatsAppBusinessAccountEventDestinationTypeDef],  # (1)
```

1. See [:material-code-braces: WhatsAppBusinessAccountEventDestinationTypeDef](./type_defs.md#whatsappbusinessaccounteventdestinationtypedef) 
## LinkedWhatsAppBusinessAccountTypeDef

```python
# LinkedWhatsAppBusinessAccountTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import LinkedWhatsAppBusinessAccountTypeDef


def get_value() -> LinkedWhatsAppBusinessAccountTypeDef:
    return {
        "arn": ...,
    }


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
# ListLinkedWhatsAppBusinessAccountsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import ListLinkedWhatsAppBusinessAccountsInputPaginateTypeDef


def get_value() -> ListLinkedWhatsAppBusinessAccountsInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListLinkedWhatsAppBusinessAccountsInputPaginateTypeDef definition

class ListLinkedWhatsAppBusinessAccountsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import ListTagsForResourceOutputTypeDef


def get_value() -> ListTagsForResourceOutputTypeDef:
    return {
        "statusCode": ...,
    }


# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    statusCode: int,
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceInputTypeDef

```python
# TagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import TagResourceInputTypeDef


def get_value() -> TagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceInputTypeDef definition

class TagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## WabaPhoneNumberSetupFinalizationTypeDef

```python
# WabaPhoneNumberSetupFinalizationTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import WabaPhoneNumberSetupFinalizationTypeDef


def get_value() -> WabaPhoneNumberSetupFinalizationTypeDef:
    return {
        "id": ...,
    }


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
# WabaSetupFinalizationTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import WabaSetupFinalizationTypeDef


def get_value() -> WabaSetupFinalizationTypeDef:
    return {
        "id": ...,
    }


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
# WhatsAppSignupCallbackResultTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import WhatsAppSignupCallbackResultTypeDef


def get_value() -> WhatsAppSignupCallbackResultTypeDef:
    return {
        "associateInProgressToken": ...,
    }


# WhatsAppSignupCallbackResultTypeDef definition

class WhatsAppSignupCallbackResultTypeDef(TypedDict):
    associateInProgressToken: NotRequired[str],
    linkedAccountsWithIncompleteSetup: NotRequired[Dict[str, LinkedWhatsAppBusinessAccountIdMetaDataTypeDef]],  # (1)
```

1. See [:material-code-braces: LinkedWhatsAppBusinessAccountIdMetaDataTypeDef](./type_defs.md#linkedwhatsappbusinessaccountidmetadatatypedef) 
## ListLinkedWhatsAppBusinessAccountsOutputTypeDef

```python
# ListLinkedWhatsAppBusinessAccountsOutputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import ListLinkedWhatsAppBusinessAccountsOutputTypeDef


def get_value() -> ListLinkedWhatsAppBusinessAccountsOutputTypeDef:
    return {
        "linkedAccounts": ...,
    }


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
# GetLinkedWhatsAppBusinessAccountOutputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import GetLinkedWhatsAppBusinessAccountOutputTypeDef


def get_value() -> GetLinkedWhatsAppBusinessAccountOutputTypeDef:
    return {
        "account": ...,
    }


# GetLinkedWhatsAppBusinessAccountOutputTypeDef definition

class GetLinkedWhatsAppBusinessAccountOutputTypeDef(TypedDict):
    account: LinkedWhatsAppBusinessAccountTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LinkedWhatsAppBusinessAccountTypeDef](./type_defs.md#linkedwhatsappbusinessaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WhatsAppSetupFinalizationTypeDef

```python
# WhatsAppSetupFinalizationTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import WhatsAppSetupFinalizationTypeDef


def get_value() -> WhatsAppSetupFinalizationTypeDef:
    return {
        "associateInProgressToken": ...,
    }


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
# AssociateWhatsAppBusinessAccountOutputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import AssociateWhatsAppBusinessAccountOutputTypeDef


def get_value() -> AssociateWhatsAppBusinessAccountOutputTypeDef:
    return {
        "signupCallbackResult": ...,
    }


# AssociateWhatsAppBusinessAccountOutputTypeDef definition

class AssociateWhatsAppBusinessAccountOutputTypeDef(TypedDict):
    signupCallbackResult: WhatsAppSignupCallbackResultTypeDef,  # (1)
    statusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WhatsAppSignupCallbackResultTypeDef](./type_defs.md#whatsappsignupcallbackresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateWhatsAppBusinessAccountInputTypeDef

```python
# AssociateWhatsAppBusinessAccountInputTypeDef TypedDict usage example

from types_aiobotocore_socialmessaging.type_defs import AssociateWhatsAppBusinessAccountInputTypeDef


def get_value() -> AssociateWhatsAppBusinessAccountInputTypeDef:
    return {
        "signupCallback": ...,
    }


# AssociateWhatsAppBusinessAccountInputTypeDef definition

class AssociateWhatsAppBusinessAccountInputTypeDef(TypedDict):
    signupCallback: NotRequired[WhatsAppSignupCallbackTypeDef],  # (1)
    setupFinalization: NotRequired[WhatsAppSetupFinalizationTypeDef],  # (2)
```

1. See [:material-code-braces: WhatsAppSignupCallbackTypeDef](./type_defs.md#whatsappsignupcallbacktypedef) 
2. See [:material-code-braces: WhatsAppSetupFinalizationTypeDef](./type_defs.md#whatsappsetupfinalizationtypedef) 
