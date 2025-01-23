# Type definitions

> [Index](../README.md) > [QApps](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [QApps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#qapps)
    type annotations stubs module [types-aiobotocore-qapps](https://pypi.org/project/types-aiobotocore-qapps/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## FormInputCardMetadataUnionTypeDef

```python
# FormInputCardMetadataUnionTypeDef definition

FormInputCardMetadataUnionTypeDef = Union[
    FormInputCardMetadataTypeDef,  # (1)
    FormInputCardMetadataOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FormInputCardMetadataTypeDef](./type_defs.md#forminputcardmetadatatypedef) 
2. See [:material-code-braces: FormInputCardMetadataOutputTypeDef](./type_defs.md#forminputcardmetadataoutputtypedef) 

## DocumentAttributeValueUnionTypeDef

```python
# DocumentAttributeValueUnionTypeDef definition

DocumentAttributeValueUnionTypeDef = Union[
    DocumentAttributeValueTypeDef,  # (1)
    DocumentAttributeValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef) 
2. See [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 

## FormInputCardInputUnionTypeDef

```python
# FormInputCardInputUnionTypeDef definition

FormInputCardInputUnionTypeDef = Union[
    FormInputCardInputTypeDef,  # (1)
    FormInputCardInputOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FormInputCardInputTypeDef](./type_defs.md#forminputcardinputtypedef) 
2. See [:material-code-braces: FormInputCardInputOutputTypeDef](./type_defs.md#forminputcardinputoutputtypedef) 

## DocumentAttributeUnionTypeDef

```python
# DocumentAttributeUnionTypeDef definition

DocumentAttributeUnionTypeDef = Union[
    DocumentAttributeTypeDef,  # (1)
    DocumentAttributeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
2. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 

## AttributeFilterUnionTypeDef

```python
# AttributeFilterUnionTypeDef definition

AttributeFilterUnionTypeDef = Union[
    AttributeFilterTypeDef,  # (1)
    AttributeFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef) 
2. See [:material-code-braces: AttributeFilterOutputTypeDef](./type_defs.md#attributefilteroutputtypedef) 

## QQueryCardInputUnionTypeDef

```python
# QQueryCardInputUnionTypeDef definition

QQueryCardInputUnionTypeDef = Union[
    QQueryCardInputTypeDef,  # (1)
    QQueryCardInputOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: QQueryCardInputTypeDef](./type_defs.md#qquerycardinputtypedef) 
2. See [:material-code-braces: QQueryCardInputOutputTypeDef](./type_defs.md#qquerycardinputoutputtypedef) 

## CardInputUnionTypeDef

```python
# CardInputUnionTypeDef definition

CardInputUnionTypeDef = Union[
    CardInputTypeDef,  # (1)
    CardInputOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CardInputTypeDef](./type_defs.md#cardinputtypedef) 
2. See [:material-code-braces: CardInputOutputTypeDef](./type_defs.md#cardinputoutputtypedef) 



## AssociateLibraryItemReviewInputRequestTypeDef

```python
# AssociateLibraryItemReviewInputRequestTypeDef definition

class AssociateLibraryItemReviewInputRequestTypeDef(TypedDict):
    instanceId: str,
    libraryItemId: str,
```

## AssociateQAppWithUserInputRequestTypeDef

```python
# AssociateQAppWithUserInputRequestTypeDef definition

class AssociateQAppWithUserInputRequestTypeDef(TypedDict):
    instanceId: str,
    appId: str,
```

## BatchCreateCategoryInputCategoryTypeDef

```python
# BatchCreateCategoryInputCategoryTypeDef definition

class BatchCreateCategoryInputCategoryTypeDef(TypedDict):
    title: str,
    id: NotRequired[str],
    color: NotRequired[str],
```

## BatchDeleteCategoryInputRequestTypeDef

```python
# BatchDeleteCategoryInputRequestTypeDef definition

class BatchDeleteCategoryInputRequestTypeDef(TypedDict):
    instanceId: str,
    categories: Sequence[str],
```

## CategoryInputTypeDef

```python
# CategoryInputTypeDef definition

class CategoryInputTypeDef(TypedDict):
    id: str,
    title: str,
    color: NotRequired[str],
```

## FileUploadCardInputTypeDef

```python
# FileUploadCardInputTypeDef definition

class FileUploadCardInputTypeDef(TypedDict):
    title: str,
    id: str,
    type: CardTypeType,  # (1)
    filename: NotRequired[str],
    fileId: NotRequired[str],
    allowOverride: NotRequired[bool],
```

1. See [:material-code-brackets: CardTypeType](./literals.md#cardtypetype) 
## QPluginCardInputTypeDef

```python
# QPluginCardInputTypeDef definition

class QPluginCardInputTypeDef(TypedDict):
    title: str,
    id: str,
    type: CardTypeType,  # (1)
    prompt: str,
    pluginId: str,
    actionIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: CardTypeType](./literals.md#cardtypetype) 
## TextInputCardInputTypeDef

```python
# TextInputCardInputTypeDef definition

class TextInputCardInputTypeDef(TypedDict):
    title: str,
    id: str,
    type: CardTypeType,  # (1)
    placeholder: NotRequired[str],
    defaultValue: NotRequired[str],
```

1. See [:material-code-brackets: CardTypeType](./literals.md#cardtypetype) 
## SubmissionTypeDef

```python
# SubmissionTypeDef definition

class SubmissionTypeDef(TypedDict):
    value: NotRequired[Dict[str, Any]],
    submissionId: NotRequired[str],
    timestamp: NotRequired[datetime],
```

## FileUploadCardTypeDef

```python
# FileUploadCardTypeDef definition

class FileUploadCardTypeDef(TypedDict):
    id: str,
    title: str,
    dependencies: List[str],
    type: CardTypeType,  # (1)
    filename: NotRequired[str],
    fileId: NotRequired[str],
    allowOverride: NotRequired[bool],
```

1. See [:material-code-brackets: CardTypeType](./literals.md#cardtypetype) 
## QPluginCardTypeDef

```python
# QPluginCardTypeDef definition

class QPluginCardTypeDef(TypedDict):
    id: str,
    title: str,
    dependencies: List[str],
    type: CardTypeType,  # (1)
    prompt: str,
    pluginType: PluginTypeType,  # (2)
    pluginId: str,
    actionIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: CardTypeType](./literals.md#cardtypetype) 
2. See [:material-code-brackets: PluginTypeType](./literals.md#plugintypetype) 
## TextInputCardTypeDef

```python
# TextInputCardTypeDef definition

class TextInputCardTypeDef(TypedDict):
    id: str,
    title: str,
    dependencies: List[str],
    type: CardTypeType,  # (1)
    placeholder: NotRequired[str],
    defaultValue: NotRequired[str],
```

1. See [:material-code-brackets: CardTypeType](./literals.md#cardtypetype) 
## SubmissionMutationTypeDef

```python
# SubmissionMutationTypeDef definition

class SubmissionMutationTypeDef(TypedDict):
    submissionId: str,
    mutationType: SubmissionMutationKindType,  # (1)
```

1. See [:material-code-brackets: SubmissionMutationKindType](./literals.md#submissionmutationkindtype) 
## CategoryTypeDef

```python
# CategoryTypeDef definition

class CategoryTypeDef(TypedDict):
    id: str,
    title: str,
    color: NotRequired[str],
    appCount: NotRequired[int],
```

## ConversationMessageTypeDef

```python
# ConversationMessageTypeDef definition

class ConversationMessageTypeDef(TypedDict):
    body: str,
    type: SenderType,  # (1)
```

1. See [:material-code-brackets: SenderType](./literals.md#sendertype) 
## CreateLibraryItemInputRequestTypeDef

```python
# CreateLibraryItemInputRequestTypeDef definition

class CreateLibraryItemInputRequestTypeDef(TypedDict):
    instanceId: str,
    appId: str,
    appVersion: int,
    categories: Sequence[str],
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

## CreatePresignedUrlInputRequestTypeDef

```python
# CreatePresignedUrlInputRequestTypeDef definition

class CreatePresignedUrlInputRequestTypeDef(TypedDict):
    instanceId: str,
    cardId: str,
    appId: str,
    fileContentsSha256: str,
    fileName: str,
    scope: DocumentScopeType,  # (1)
    sessionId: NotRequired[str],
```

1. See [:material-code-brackets: DocumentScopeType](./literals.md#documentscopetype) 
## DeleteLibraryItemInputRequestTypeDef

```python
# DeleteLibraryItemInputRequestTypeDef definition

class DeleteLibraryItemInputRequestTypeDef(TypedDict):
    instanceId: str,
    libraryItemId: str,
```

## DeleteQAppInputRequestTypeDef

```python
# DeleteQAppInputRequestTypeDef definition

class DeleteQAppInputRequestTypeDef(TypedDict):
    instanceId: str,
    appId: str,
```

## DescribeQAppPermissionsInputRequestTypeDef

```python
# DescribeQAppPermissionsInputRequestTypeDef definition

class DescribeQAppPermissionsInputRequestTypeDef(TypedDict):
    instanceId: str,
    appId: str,
```

## DisassociateLibraryItemReviewInputRequestTypeDef

```python
# DisassociateLibraryItemReviewInputRequestTypeDef definition

class DisassociateLibraryItemReviewInputRequestTypeDef(TypedDict):
    instanceId: str,
    libraryItemId: str,
```

## DisassociateQAppFromUserInputRequestTypeDef

```python
# DisassociateQAppFromUserInputRequestTypeDef definition

class DisassociateQAppFromUserInputRequestTypeDef(TypedDict):
    instanceId: str,
    appId: str,
```

## DocumentAttributeValueOutputTypeDef

```python
# DocumentAttributeValueOutputTypeDef definition

class DocumentAttributeValueOutputTypeDef(TypedDict):
    stringValue: NotRequired[str],
    stringListValue: NotRequired[List[str]],
    longValue: NotRequired[int],
    dateValue: NotRequired[datetime],
```

## ExportQAppSessionDataInputRequestTypeDef

```python
# ExportQAppSessionDataInputRequestTypeDef definition

class ExportQAppSessionDataInputRequestTypeDef(TypedDict):
    instanceId: str,
    sessionId: str,
```

## FormInputCardMetadataOutputTypeDef

```python
# FormInputCardMetadataOutputTypeDef definition

class FormInputCardMetadataOutputTypeDef(TypedDict):
    schema: Dict[str, Any],
```

## FormInputCardMetadataTypeDef

```python
# FormInputCardMetadataTypeDef definition

class FormInputCardMetadataTypeDef(TypedDict):
    schema: Mapping[str, Any],
```

## GetLibraryItemInputRequestTypeDef

```python
# GetLibraryItemInputRequestTypeDef definition

class GetLibraryItemInputRequestTypeDef(TypedDict):
    instanceId: str,
    libraryItemId: str,
    appId: NotRequired[str],
```

## GetQAppInputRequestTypeDef

```python
# GetQAppInputRequestTypeDef definition

class GetQAppInputRequestTypeDef(TypedDict):
    instanceId: str,
    appId: str,
    appVersion: NotRequired[int],
```

## GetQAppSessionInputRequestTypeDef

```python
# GetQAppSessionInputRequestTypeDef definition

class GetQAppSessionInputRequestTypeDef(TypedDict):
    instanceId: str,
    sessionId: str,
```

## GetQAppSessionMetadataInputRequestTypeDef

```python
# GetQAppSessionMetadataInputRequestTypeDef definition

class GetQAppSessionMetadataInputRequestTypeDef(TypedDict):
    instanceId: str,
    sessionId: str,
```

## SessionSharingConfigurationTypeDef

```python
# SessionSharingConfigurationTypeDef definition

class SessionSharingConfigurationTypeDef(TypedDict):
    enabled: bool,
    acceptResponses: NotRequired[bool],
    revealCards: NotRequired[bool],
```

## ImportDocumentInputRequestTypeDef

```python
# ImportDocumentInputRequestTypeDef definition

class ImportDocumentInputRequestTypeDef(TypedDict):
    instanceId: str,
    cardId: str,
    appId: str,
    fileContentsBase64: str,
    fileName: str,
    scope: DocumentScopeType,  # (1)
    sessionId: NotRequired[str],
```

1. See [:material-code-brackets: DocumentScopeType](./literals.md#documentscopetype) 
## ListCategoriesInputRequestTypeDef

```python
# ListCategoriesInputRequestTypeDef definition

class ListCategoriesInputRequestTypeDef(TypedDict):
    instanceId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListLibraryItemsInputRequestTypeDef

```python
# ListLibraryItemsInputRequestTypeDef definition

class ListLibraryItemsInputRequestTypeDef(TypedDict):
    instanceId: str,
    limit: NotRequired[int],
    nextToken: NotRequired[str],
    categoryId: NotRequired[str],
```

## ListQAppSessionDataInputRequestTypeDef

```python
# ListQAppSessionDataInputRequestTypeDef definition

class ListQAppSessionDataInputRequestTypeDef(TypedDict):
    instanceId: str,
    sessionId: str,
```

## ListQAppsInputRequestTypeDef

```python
# ListQAppsInputRequestTypeDef definition

class ListQAppsInputRequestTypeDef(TypedDict):
    instanceId: str,
    limit: NotRequired[int],
    nextToken: NotRequired[str],
```

## UserAppItemTypeDef

```python
# UserAppItemTypeDef definition

class UserAppItemTypeDef(TypedDict):
    appId: str,
    appArn: str,
    title: str,
    createdAt: datetime,
    description: NotRequired[str],
    canEdit: NotRequired[bool],
    status: NotRequired[str],
    isVerified: NotRequired[bool],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
```

## PermissionInputTypeDef

```python
# PermissionInputTypeDef definition

class PermissionInputTypeDef(TypedDict):
    action: PermissionInputActionEnumType,  # (1)
    principal: str,
```

1. See [:material-code-brackets: PermissionInputActionEnumType](./literals.md#permissioninputactionenumtype) 
## PrincipalOutputTypeDef

```python
# PrincipalOutputTypeDef definition

class PrincipalOutputTypeDef(TypedDict):
    userId: NotRequired[str],
    userType: NotRequired[PrincipalOutputUserTypeEnumType],  # (1)
    email: NotRequired[str],
```

1. See [:material-code-brackets: PrincipalOutputUserTypeEnumType](./literals.md#principaloutputusertypeenumtype) 
## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    userId: NotRequired[str],
```

## StopQAppSessionInputRequestTypeDef

```python
# StopQAppSessionInputRequestTypeDef definition

class StopQAppSessionInputRequestTypeDef(TypedDict):
    instanceId: str,
    sessionId: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    tagKeys: Sequence[str],
```

## UpdateLibraryItemInputRequestTypeDef

```python
# UpdateLibraryItemInputRequestTypeDef definition

class UpdateLibraryItemInputRequestTypeDef(TypedDict):
    instanceId: str,
    libraryItemId: str,
    status: NotRequired[LibraryItemStatusType],  # (1)
    categories: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: LibraryItemStatusType](./literals.md#libraryitemstatustype) 
## UpdateLibraryItemMetadataInputRequestTypeDef

```python
# UpdateLibraryItemMetadataInputRequestTypeDef definition

class UpdateLibraryItemMetadataInputRequestTypeDef(TypedDict):
    instanceId: str,
    libraryItemId: str,
    isVerified: NotRequired[bool],
```

## BatchCreateCategoryInputRequestTypeDef

```python
# BatchCreateCategoryInputRequestTypeDef definition

class BatchCreateCategoryInputRequestTypeDef(TypedDict):
    instanceId: str,
    categories: Sequence[BatchCreateCategoryInputCategoryTypeDef],  # (1)
```

1. See [:material-code-braces: BatchCreateCategoryInputCategoryTypeDef](./type_defs.md#batchcreatecategoryinputcategorytypedef) 
## BatchUpdateCategoryInputRequestTypeDef

```python
# BatchUpdateCategoryInputRequestTypeDef definition

class BatchUpdateCategoryInputRequestTypeDef(TypedDict):
    instanceId: str,
    categories: Sequence[CategoryInputTypeDef],  # (1)
```

1. See [:material-code-braces: CategoryInputTypeDef](./type_defs.md#categoryinputtypedef) 
## CardStatusTypeDef

```python
# CardStatusTypeDef definition

class CardStatusTypeDef(TypedDict):
    currentState: ExecutionStatusType,  # (1)
    currentValue: str,
    submissions: NotRequired[List[SubmissionTypeDef]],  # (2)
```

1. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
2. See [:material-code-braces: SubmissionTypeDef](./type_defs.md#submissiontypedef) 
## CardValueTypeDef

```python
# CardValueTypeDef definition

class CardValueTypeDef(TypedDict):
    cardId: str,
    value: str,
    submissionMutation: NotRequired[SubmissionMutationTypeDef],  # (1)
```

1. See [:material-code-braces: SubmissionMutationTypeDef](./type_defs.md#submissionmutationtypedef) 
## LibraryItemMemberTypeDef

```python
# LibraryItemMemberTypeDef definition

class LibraryItemMemberTypeDef(TypedDict):
    libraryItemId: str,
    appId: str,
    appVersion: int,
    categories: List[CategoryTypeDef],  # (1)
    status: str,
    createdAt: datetime,
    createdBy: str,
    ratingCount: int,
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
    isRatedByUser: NotRequired[bool],
    userCount: NotRequired[int],
    isVerified: NotRequired[bool],
```

1. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
## PredictQAppInputOptionsTypeDef

```python
# PredictQAppInputOptionsTypeDef definition

class PredictQAppInputOptionsTypeDef(TypedDict):
    conversation: NotRequired[Sequence[ConversationMessageTypeDef]],  # (1)
    problemStatement: NotRequired[str],
```

1. See [:material-code-braces: ConversationMessageTypeDef](./type_defs.md#conversationmessagetypedef) 
## CreateLibraryItemOutputTypeDef

```python
# CreateLibraryItemOutputTypeDef definition

class CreateLibraryItemOutputTypeDef(TypedDict):
    libraryItemId: str,
    status: str,
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    ratingCount: int,
    isVerified: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePresignedUrlOutputTypeDef

```python
# CreatePresignedUrlOutputTypeDef definition

class CreatePresignedUrlOutputTypeDef(TypedDict):
    fileId: str,
    presignedUrl: str,
    presignedUrlFields: Dict[str, str],
    presignedUrlExpiration: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQAppOutputTypeDef

```python
# CreateQAppOutputTypeDef definition

class CreateQAppOutputTypeDef(TypedDict):
    appId: str,
    appArn: str,
    title: str,
    description: str,
    initialPrompt: str,
    appVersion: int,
    status: AppStatusType,  # (1)
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    requiredCapabilities: List[AppRequiredCapabilityType],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AppStatusType](./literals.md#appstatustype) 
2. See [:material-code-brackets: AppRequiredCapabilityType](./literals.md#apprequiredcapabilitytype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportQAppSessionDataOutputTypeDef

```python
# ExportQAppSessionDataOutputTypeDef definition

class ExportQAppSessionDataOutputTypeDef(TypedDict):
    csvFileLink: str,
    expiresAt: datetime,
    sessionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLibraryItemOutputTypeDef

```python
# GetLibraryItemOutputTypeDef definition

class GetLibraryItemOutputTypeDef(TypedDict):
    libraryItemId: str,
    appId: str,
    appVersion: int,
    categories: List[CategoryTypeDef],  # (1)
    status: str,
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    ratingCount: int,
    isRatedByUser: bool,
    userCount: int,
    isVerified: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportDocumentOutputTypeDef

```python
# ImportDocumentOutputTypeDef definition

class ImportDocumentOutputTypeDef(TypedDict):
    fileId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCategoriesOutputTypeDef

```python
# ListCategoriesOutputTypeDef definition

class ListCategoriesOutputTypeDef(TypedDict):
    categories: List[CategoryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartQAppSessionOutputTypeDef

```python
# StartQAppSessionOutputTypeDef definition

class StartQAppSessionOutputTypeDef(TypedDict):
    sessionId: str,
    sessionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLibraryItemOutputTypeDef

```python
# UpdateLibraryItemOutputTypeDef definition

class UpdateLibraryItemOutputTypeDef(TypedDict):
    libraryItemId: str,
    appId: str,
    appVersion: int,
    categories: List[CategoryTypeDef],  # (1)
    status: str,
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    ratingCount: int,
    isRatedByUser: bool,
    userCount: int,
    isVerified: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateQAppOutputTypeDef

```python
# UpdateQAppOutputTypeDef definition

class UpdateQAppOutputTypeDef(TypedDict):
    appId: str,
    appArn: str,
    title: str,
    description: str,
    initialPrompt: str,
    appVersion: int,
    status: AppStatusType,  # (1)
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    requiredCapabilities: List[AppRequiredCapabilityType],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AppStatusType](./literals.md#appstatustype) 
2. See [:material-code-brackets: AppRequiredCapabilityType](./literals.md#apprequiredcapabilitytype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateQAppSessionOutputTypeDef

```python
# UpdateQAppSessionOutputTypeDef definition

class UpdateQAppSessionOutputTypeDef(TypedDict):
    sessionId: str,
    sessionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentAttributeOutputTypeDef

```python
# DocumentAttributeOutputTypeDef definition

class DocumentAttributeOutputTypeDef(TypedDict):
    name: str,
    value: DocumentAttributeValueOutputTypeDef,  # (1)
```

1. See [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
## DocumentAttributeValueTypeDef

```python
# DocumentAttributeValueTypeDef definition

class DocumentAttributeValueTypeDef(TypedDict):
    stringValue: NotRequired[str],
    stringListValue: NotRequired[Sequence[str]],
    longValue: NotRequired[int],
    dateValue: NotRequired[TimestampTypeDef],
```

## FormInputCardInputOutputTypeDef

```python
# FormInputCardInputOutputTypeDef definition

class FormInputCardInputOutputTypeDef(TypedDict):
    title: str,
    id: str,
    type: CardTypeType,  # (1)
    metadata: FormInputCardMetadataOutputTypeDef,  # (2)
    computeMode: NotRequired[InputCardComputeModeType],  # (3)
```

1. See [:material-code-brackets: CardTypeType](./literals.md#cardtypetype) 
2. See [:material-code-braces: FormInputCardMetadataOutputTypeDef](./type_defs.md#forminputcardmetadataoutputtypedef) 
3. See [:material-code-brackets: InputCardComputeModeType](./literals.md#inputcardcomputemodetype) 
## FormInputCardTypeDef

```python
# FormInputCardTypeDef definition

class FormInputCardTypeDef(TypedDict):
    id: str,
    title: str,
    dependencies: List[str],
    type: CardTypeType,  # (1)
    metadata: FormInputCardMetadataOutputTypeDef,  # (2)
    computeMode: NotRequired[InputCardComputeModeType],  # (3)
```

1. See [:material-code-brackets: CardTypeType](./literals.md#cardtypetype) 
2. See [:material-code-braces: FormInputCardMetadataOutputTypeDef](./type_defs.md#forminputcardmetadataoutputtypedef) 
3. See [:material-code-brackets: InputCardComputeModeType](./literals.md#inputcardcomputemodetype) 
## GetQAppSessionMetadataOutputTypeDef

```python
# GetQAppSessionMetadataOutputTypeDef definition

class GetQAppSessionMetadataOutputTypeDef(TypedDict):
    sessionId: str,
    sessionArn: str,
    sessionName: str,
    sharingConfiguration: SessionSharingConfigurationTypeDef,  # (1)
    sessionOwner: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionSharingConfigurationTypeDef](./type_defs.md#sessionsharingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateQAppSessionMetadataInputRequestTypeDef

```python
# UpdateQAppSessionMetadataInputRequestTypeDef definition

class UpdateQAppSessionMetadataInputRequestTypeDef(TypedDict):
    instanceId: str,
    sessionId: str,
    sharingConfiguration: SessionSharingConfigurationTypeDef,  # (1)
    sessionName: NotRequired[str],
```

1. See [:material-code-braces: SessionSharingConfigurationTypeDef](./type_defs.md#sessionsharingconfigurationtypedef) 
## UpdateQAppSessionMetadataOutputTypeDef

```python
# UpdateQAppSessionMetadataOutputTypeDef definition

class UpdateQAppSessionMetadataOutputTypeDef(TypedDict):
    sessionId: str,
    sessionArn: str,
    sessionName: str,
    sharingConfiguration: SessionSharingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionSharingConfigurationTypeDef](./type_defs.md#sessionsharingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLibraryItemsInputPaginateTypeDef

```python
# ListLibraryItemsInputPaginateTypeDef definition

class ListLibraryItemsInputPaginateTypeDef(TypedDict):
    instanceId: str,
    categoryId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQAppsInputPaginateTypeDef

```python
# ListQAppsInputPaginateTypeDef definition

class ListQAppsInputPaginateTypeDef(TypedDict):
    instanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQAppsOutputTypeDef

```python
# ListQAppsOutputTypeDef definition

class ListQAppsOutputTypeDef(TypedDict):
    apps: List[UserAppItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: UserAppItemTypeDef](./type_defs.md#userappitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateQAppPermissionsInputRequestTypeDef

```python
# UpdateQAppPermissionsInputRequestTypeDef definition

class UpdateQAppPermissionsInputRequestTypeDef(TypedDict):
    instanceId: str,
    appId: str,
    grantPermissions: NotRequired[Sequence[PermissionInputTypeDef]],  # (1)
    revokePermissions: NotRequired[Sequence[PermissionInputTypeDef]],  # (1)
```

1. See [:material-code-braces: PermissionInputTypeDef](./type_defs.md#permissioninputtypedef) 
2. See [:material-code-braces: PermissionInputTypeDef](./type_defs.md#permissioninputtypedef) 
## PermissionOutputTypeDef

```python
# PermissionOutputTypeDef definition

class PermissionOutputTypeDef(TypedDict):
    action: PermissionOutputActionEnumType,  # (1)
    principal: PrincipalOutputTypeDef,  # (2)
```

1. See [:material-code-brackets: PermissionOutputActionEnumType](./literals.md#permissionoutputactionenumtype) 
2. See [:material-code-braces: PrincipalOutputTypeDef](./type_defs.md#principaloutputtypedef) 
## QAppSessionDataTypeDef

```python
# QAppSessionDataTypeDef definition

class QAppSessionDataTypeDef(TypedDict):
    cardId: str,
    user: UserTypeDef,  # (1)
    value: NotRequired[Dict[str, Any]],
    submissionId: NotRequired[str],
    timestamp: NotRequired[datetime],
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
## GetQAppSessionOutputTypeDef

```python
# GetQAppSessionOutputTypeDef definition

class GetQAppSessionOutputTypeDef(TypedDict):
    sessionId: str,
    sessionArn: str,
    sessionName: str,
    appVersion: int,
    latestPublishedAppVersion: int,
    status: ExecutionStatusType,  # (1)
    cardStatus: Dict[str, CardStatusTypeDef],  # (2)
    userIsHost: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
2. See [:material-code-braces: CardStatusTypeDef](./type_defs.md#cardstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartQAppSessionInputRequestTypeDef

```python
# StartQAppSessionInputRequestTypeDef definition

class StartQAppSessionInputRequestTypeDef(TypedDict):
    instanceId: str,
    appId: str,
    appVersion: int,
    initialValues: NotRequired[Sequence[CardValueTypeDef]],  # (1)
    sessionId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CardValueTypeDef](./type_defs.md#cardvaluetypedef) 
## UpdateQAppSessionInputRequestTypeDef

```python
# UpdateQAppSessionInputRequestTypeDef definition

class UpdateQAppSessionInputRequestTypeDef(TypedDict):
    instanceId: str,
    sessionId: str,
    values: NotRequired[Sequence[CardValueTypeDef]],  # (1)
```

1. See [:material-code-braces: CardValueTypeDef](./type_defs.md#cardvaluetypedef) 
## ListLibraryItemsOutputTypeDef

```python
# ListLibraryItemsOutputTypeDef definition

class ListLibraryItemsOutputTypeDef(TypedDict):
    libraryItems: List[LibraryItemMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LibraryItemMemberTypeDef](./type_defs.md#libraryitemmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PredictQAppInputRequestTypeDef

```python
# PredictQAppInputRequestTypeDef definition

class PredictQAppInputRequestTypeDef(TypedDict):
    instanceId: str,
    options: NotRequired[PredictQAppInputOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: PredictQAppInputOptionsTypeDef](./type_defs.md#predictqappinputoptionstypedef) 
## AttributeFilterOutputTypeDef

```python
# AttributeFilterOutputTypeDef definition

class AttributeFilterOutputTypeDef(TypedDict):
    andAllFilters: NotRequired[List[Dict[str, Any]]],
    orAllFilters: NotRequired[List[Dict[str, Any]]],
    notFilter: NotRequired[Dict[str, Any]],
    equalsTo: NotRequired[DocumentAttributeOutputTypeDef],  # (1)
    containsAll: NotRequired[DocumentAttributeOutputTypeDef],  # (1)
    containsAny: NotRequired[DocumentAttributeOutputTypeDef],  # (1)
    greaterThan: NotRequired[DocumentAttributeOutputTypeDef],  # (1)
    greaterThanOrEquals: NotRequired[DocumentAttributeOutputTypeDef],  # (1)
    lessThan: NotRequired[DocumentAttributeOutputTypeDef],  # (1)
    lessThanOrEquals: NotRequired[DocumentAttributeOutputTypeDef],  # (1)
```

1. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
2. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
3. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
4. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
5. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
6. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
7. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
## FormInputCardInputTypeDef

```python
# FormInputCardInputTypeDef definition

class FormInputCardInputTypeDef(TypedDict):
    title: str,
    id: str,
    type: CardTypeType,  # (1)
    metadata: FormInputCardMetadataUnionTypeDef,  # (2)
    computeMode: NotRequired[InputCardComputeModeType],  # (3)
```

1. See [:material-code-brackets: CardTypeType](./literals.md#cardtypetype) 
2. See [:material-code-braces: FormInputCardMetadataTypeDef](./type_defs.md#forminputcardmetadatatypedef) [:material-code-braces: FormInputCardMetadataOutputTypeDef](./type_defs.md#forminputcardmetadataoutputtypedef) 
3. See [:material-code-brackets: InputCardComputeModeType](./literals.md#inputcardcomputemodetype) 
## DescribeQAppPermissionsOutputTypeDef

```python
# DescribeQAppPermissionsOutputTypeDef definition

class DescribeQAppPermissionsOutputTypeDef(TypedDict):
    resourceArn: str,
    appId: str,
    permissions: List[PermissionOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionOutputTypeDef](./type_defs.md#permissionoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateQAppPermissionsOutputTypeDef

```python
# UpdateQAppPermissionsOutputTypeDef definition

class UpdateQAppPermissionsOutputTypeDef(TypedDict):
    resourceArn: str,
    appId: str,
    permissions: List[PermissionOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionOutputTypeDef](./type_defs.md#permissionoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQAppSessionDataOutputTypeDef

```python
# ListQAppSessionDataOutputTypeDef definition

class ListQAppSessionDataOutputTypeDef(TypedDict):
    sessionId: str,
    sessionArn: str,
    sessionData: List[QAppSessionDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QAppSessionDataTypeDef](./type_defs.md#qappsessiondatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QQueryCardInputOutputTypeDef

```python
# QQueryCardInputOutputTypeDef definition

class QQueryCardInputOutputTypeDef(TypedDict):
    title: str,
    id: str,
    type: CardTypeType,  # (1)
    prompt: str,
    outputSource: NotRequired[CardOutputSourceType],  # (2)
    attributeFilter: NotRequired[AttributeFilterOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: CardTypeType](./literals.md#cardtypetype) 
2. See [:material-code-brackets: CardOutputSourceType](./literals.md#cardoutputsourcetype) 
3. See [:material-code-braces: AttributeFilterOutputTypeDef](./type_defs.md#attributefilteroutputtypedef) 
## QQueryCardTypeDef

```python
# QQueryCardTypeDef definition

class QQueryCardTypeDef(TypedDict):
    id: str,
    title: str,
    dependencies: List[str],
    type: CardTypeType,  # (1)
    prompt: str,
    outputSource: CardOutputSourceType,  # (2)
    attributeFilter: NotRequired[AttributeFilterOutputTypeDef],  # (3)
    memoryReferences: NotRequired[List[str]],
```

1. See [:material-code-brackets: CardTypeType](./literals.md#cardtypetype) 
2. See [:material-code-brackets: CardOutputSourceType](./literals.md#cardoutputsourcetype) 
3. See [:material-code-braces: AttributeFilterOutputTypeDef](./type_defs.md#attributefilteroutputtypedef) 
## DocumentAttributeTypeDef

```python
# DocumentAttributeTypeDef definition

class DocumentAttributeTypeDef(TypedDict):
    name: str,
    value: DocumentAttributeValueUnionTypeDef,  # (1)
```

1. See [:material-code-braces: DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef) [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
## CardInputOutputTypeDef

```python
# CardInputOutputTypeDef definition

class CardInputOutputTypeDef(TypedDict):
    textInput: NotRequired[TextInputCardInputTypeDef],  # (1)
    qQuery: NotRequired[QQueryCardInputOutputTypeDef],  # (2)
    qPlugin: NotRequired[QPluginCardInputTypeDef],  # (3)
    fileUpload: NotRequired[FileUploadCardInputTypeDef],  # (4)
    formInput: NotRequired[FormInputCardInputOutputTypeDef],  # (5)
```

1. See [:material-code-braces: TextInputCardInputTypeDef](./type_defs.md#textinputcardinputtypedef) 
2. See [:material-code-braces: QQueryCardInputOutputTypeDef](./type_defs.md#qquerycardinputoutputtypedef) 
3. See [:material-code-braces: QPluginCardInputTypeDef](./type_defs.md#qplugincardinputtypedef) 
4. See [:material-code-braces: FileUploadCardInputTypeDef](./type_defs.md#fileuploadcardinputtypedef) 
5. See [:material-code-braces: FormInputCardInputOutputTypeDef](./type_defs.md#forminputcardinputoutputtypedef) 
## CardTypeDef

```python
# CardTypeDef definition

class CardTypeDef(TypedDict):
    textInput: NotRequired[TextInputCardTypeDef],  # (1)
    qQuery: NotRequired[QQueryCardTypeDef],  # (2)
    qPlugin: NotRequired[QPluginCardTypeDef],  # (3)
    fileUpload: NotRequired[FileUploadCardTypeDef],  # (4)
    formInput: NotRequired[FormInputCardTypeDef],  # (5)
```

1. See [:material-code-braces: TextInputCardTypeDef](./type_defs.md#textinputcardtypedef) 
2. See [:material-code-braces: QQueryCardTypeDef](./type_defs.md#qquerycardtypedef) 
3. See [:material-code-braces: QPluginCardTypeDef](./type_defs.md#qplugincardtypedef) 
4. See [:material-code-braces: FileUploadCardTypeDef](./type_defs.md#fileuploadcardtypedef) 
5. See [:material-code-braces: FormInputCardTypeDef](./type_defs.md#forminputcardtypedef) 
## AppDefinitionInputOutputTypeDef

```python
# AppDefinitionInputOutputTypeDef definition

class AppDefinitionInputOutputTypeDef(TypedDict):
    cards: List[CardInputOutputTypeDef],  # (1)
    initialPrompt: NotRequired[str],
```

1. See [:material-code-braces: CardInputOutputTypeDef](./type_defs.md#cardinputoutputtypedef) 
## AppDefinitionTypeDef

```python
# AppDefinitionTypeDef definition

class AppDefinitionTypeDef(TypedDict):
    appDefinitionVersion: str,
    cards: List[CardTypeDef],  # (1)
    canEdit: NotRequired[bool],
```

1. See [:material-code-braces: CardTypeDef](./type_defs.md#cardtypedef) 
## AttributeFilterTypeDef

```python
# AttributeFilterTypeDef definition

class AttributeFilterTypeDef(TypedDict):
    andAllFilters: NotRequired[Sequence[Mapping[str, Any]]],
    orAllFilters: NotRequired[Sequence[Mapping[str, Any]]],
    notFilter: NotRequired[Mapping[str, Any]],
    equalsTo: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
    containsAll: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
    containsAny: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
    greaterThan: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
    greaterThanOrEquals: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
    lessThan: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
    lessThanOrEquals: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
```

1. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
2. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
3. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
4. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
5. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
6. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
7. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
## PredictAppDefinitionTypeDef

```python
# PredictAppDefinitionTypeDef definition

class PredictAppDefinitionTypeDef(TypedDict):
    title: str,
    appDefinition: AppDefinitionInputOutputTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: AppDefinitionInputOutputTypeDef](./type_defs.md#appdefinitioninputoutputtypedef) 
## GetQAppOutputTypeDef

```python
# GetQAppOutputTypeDef definition

class GetQAppOutputTypeDef(TypedDict):
    appId: str,
    appArn: str,
    title: str,
    description: str,
    initialPrompt: str,
    appVersion: int,
    status: AppStatusType,  # (1)
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    requiredCapabilities: List[AppRequiredCapabilityType],  # (2)
    appDefinition: AppDefinitionTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: AppStatusType](./literals.md#appstatustype) 
2. See [:material-code-brackets: AppRequiredCapabilityType](./literals.md#apprequiredcapabilitytype) 
3. See [:material-code-braces: AppDefinitionTypeDef](./type_defs.md#appdefinitiontypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PredictQAppOutputTypeDef

```python
# PredictQAppOutputTypeDef definition

class PredictQAppOutputTypeDef(TypedDict):
    app: PredictAppDefinitionTypeDef,  # (1)
    problemStatement: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PredictAppDefinitionTypeDef](./type_defs.md#predictappdefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QQueryCardInputTypeDef

```python
# QQueryCardInputTypeDef definition

class QQueryCardInputTypeDef(TypedDict):
    title: str,
    id: str,
    type: CardTypeType,  # (1)
    prompt: str,
    outputSource: NotRequired[CardOutputSourceType],  # (2)
    attributeFilter: NotRequired[AttributeFilterUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: CardTypeType](./literals.md#cardtypetype) 
2. See [:material-code-brackets: CardOutputSourceType](./literals.md#cardoutputsourcetype) 
3. See [:material-code-braces: AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef) [:material-code-braces: AttributeFilterOutputTypeDef](./type_defs.md#attributefilteroutputtypedef) 
## CardInputTypeDef

```python
# CardInputTypeDef definition

class CardInputTypeDef(TypedDict):
    textInput: NotRequired[TextInputCardInputTypeDef],  # (1)
    qQuery: NotRequired[QQueryCardInputUnionTypeDef],  # (2)
    qPlugin: NotRequired[QPluginCardInputTypeDef],  # (3)
    fileUpload: NotRequired[FileUploadCardInputTypeDef],  # (4)
    formInput: NotRequired[FormInputCardInputUnionTypeDef],  # (5)
```

1. See [:material-code-braces: TextInputCardInputTypeDef](./type_defs.md#textinputcardinputtypedef) 
2. See [:material-code-braces: QQueryCardInputTypeDef](./type_defs.md#qquerycardinputtypedef) [:material-code-braces: QQueryCardInputOutputTypeDef](./type_defs.md#qquerycardinputoutputtypedef) 
3. See [:material-code-braces: QPluginCardInputTypeDef](./type_defs.md#qplugincardinputtypedef) 
4. See [:material-code-braces: FileUploadCardInputTypeDef](./type_defs.md#fileuploadcardinputtypedef) 
5. See [:material-code-braces: FormInputCardInputTypeDef](./type_defs.md#forminputcardinputtypedef) [:material-code-braces: FormInputCardInputOutputTypeDef](./type_defs.md#forminputcardinputoutputtypedef) 
## AppDefinitionInputTypeDef

```python
# AppDefinitionInputTypeDef definition

class AppDefinitionInputTypeDef(TypedDict):
    cards: Sequence[CardInputUnionTypeDef],  # (1)
    initialPrompt: NotRequired[str],
```

1. See [:material-code-braces: CardInputTypeDef](./type_defs.md#cardinputtypedef) [:material-code-braces: CardInputOutputTypeDef](./type_defs.md#cardinputoutputtypedef) 
## CreateQAppInputRequestTypeDef

```python
# CreateQAppInputRequestTypeDef definition

class CreateQAppInputRequestTypeDef(TypedDict):
    instanceId: str,
    title: str,
    appDefinition: AppDefinitionInputTypeDef,  # (1)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AppDefinitionInputTypeDef](./type_defs.md#appdefinitioninputtypedef) 
## UpdateQAppInputRequestTypeDef

```python
# UpdateQAppInputRequestTypeDef definition

class UpdateQAppInputRequestTypeDef(TypedDict):
    instanceId: str,
    appId: str,
    title: NotRequired[str],
    description: NotRequired[str],
    appDefinition: NotRequired[AppDefinitionInputTypeDef],  # (1)
```

1. See [:material-code-braces: AppDefinitionInputTypeDef](./type_defs.md#appdefinitioninputtypedef) 
