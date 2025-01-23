# Type definitions

> [Index](../README.md) > [Translate](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Translate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#translate)
    type annotations stubs module [types-aiobotocore-translate](https://pypi.org/project/types-aiobotocore-translate/).

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


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## TermTypeDef

```python
# TermTypeDef definition

class TermTypeDef(TypedDict):
    SourceText: NotRequired[str],
    TargetText: NotRequired[str],
```

## EncryptionKeyTypeDef

```python
# EncryptionKeyTypeDef definition

class EncryptionKeyTypeDef(TypedDict):
    Type: EncryptionKeyTypeType,  # (1)
    Id: str,
```

1. See [:material-code-brackets: EncryptionKeyTypeType](./literals.md#encryptionkeytypetype) 
## ParallelDataConfigTypeDef

```python
# ParallelDataConfigTypeDef definition

class ParallelDataConfigTypeDef(TypedDict):
    S3Uri: NotRequired[str],
    Format: NotRequired[ParallelDataFormatType],  # (1)
```

1. See [:material-code-brackets: ParallelDataFormatType](./literals.md#paralleldataformattype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
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

## DeleteParallelDataRequestRequestTypeDef

```python
# DeleteParallelDataRequestRequestTypeDef definition

class DeleteParallelDataRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteTerminologyRequestRequestTypeDef

```python
# DeleteTerminologyRequestRequestTypeDef definition

class DeleteTerminologyRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DescribeTextTranslationJobRequestRequestTypeDef

```python
# DescribeTextTranslationJobRequestRequestTypeDef definition

class DescribeTextTranslationJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## GetParallelDataRequestRequestTypeDef

```python
# GetParallelDataRequestRequestTypeDef definition

class GetParallelDataRequestRequestTypeDef(TypedDict):
    Name: str,
```

## ParallelDataDataLocationTypeDef

```python
# ParallelDataDataLocationTypeDef definition

class ParallelDataDataLocationTypeDef(TypedDict):
    RepositoryType: str,
    Location: str,
```

## GetTerminologyRequestRequestTypeDef

```python
# GetTerminologyRequestRequestTypeDef definition

class GetTerminologyRequestRequestTypeDef(TypedDict):
    Name: str,
    TerminologyDataFormat: NotRequired[TerminologyDataFormatType],  # (1)
```

1. See [:material-code-brackets: TerminologyDataFormatType](./literals.md#terminologydataformattype) 
## TerminologyDataLocationTypeDef

```python
# TerminologyDataLocationTypeDef definition

class TerminologyDataLocationTypeDef(TypedDict):
    RepositoryType: str,
    Location: str,
```

## InputDataConfigTypeDef

```python
# InputDataConfigTypeDef definition

class InputDataConfigTypeDef(TypedDict):
    S3Uri: str,
    ContentType: str,
```

## JobDetailsTypeDef

```python
# JobDetailsTypeDef definition

class JobDetailsTypeDef(TypedDict):
    TranslatedDocumentsCount: NotRequired[int],
    DocumentsWithErrorsCount: NotRequired[int],
    InputDocumentsCount: NotRequired[int],
```

## LanguageTypeDef

```python
# LanguageTypeDef definition

class LanguageTypeDef(TypedDict):
    LanguageName: str,
    LanguageCode: str,
```

## ListLanguagesRequestRequestTypeDef

```python
# ListLanguagesRequestRequestTypeDef definition

class ListLanguagesRequestRequestTypeDef(TypedDict):
    DisplayLanguageCode: NotRequired[DisplayLanguageCodeType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: DisplayLanguageCodeType](./literals.md#displaylanguagecodetype) 
## ListParallelDataRequestRequestTypeDef

```python
# ListParallelDataRequestRequestTypeDef definition

class ListParallelDataRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListTerminologiesRequestRequestTypeDef

```python
# ListTerminologiesRequestRequestTypeDef definition

class ListTerminologiesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## TranslationSettingsTypeDef

```python
# TranslationSettingsTypeDef definition

class TranslationSettingsTypeDef(TypedDict):
    Formality: NotRequired[FormalityType],  # (1)
    Profanity: NotRequired[ProfanityType],  # (2)
    Brevity: NotRequired[BrevityType],  # (3)
```

1. See [:material-code-brackets: FormalityType](./literals.md#formalitytype) 
2. See [:material-code-brackets: ProfanityType](./literals.md#profanitytype) 
3. See [:material-code-brackets: BrevityType](./literals.md#brevitytype) 
## StopTextTranslationJobRequestRequestTypeDef

```python
# StopTextTranslationJobRequestRequestTypeDef definition

class StopTextTranslationJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## TranslatedDocumentTypeDef

```python
# TranslatedDocumentTypeDef definition

class TranslatedDocumentTypeDef(TypedDict):
    Content: bytes,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## AppliedTerminologyTypeDef

```python
# AppliedTerminologyTypeDef definition

class AppliedTerminologyTypeDef(TypedDict):
    Name: NotRequired[str],
    Terms: NotRequired[List[TermTypeDef]],  # (1)
```

1. See [:material-code-braces: TermTypeDef](./type_defs.md#termtypedef) 
## DocumentTypeDef

```python
# DocumentTypeDef definition

class DocumentTypeDef(TypedDict):
    Content: BlobTypeDef,
    ContentType: str,
```

## TerminologyDataTypeDef

```python
# TerminologyDataTypeDef definition

class TerminologyDataTypeDef(TypedDict):
    File: BlobTypeDef,
    Format: TerminologyDataFormatType,  # (1)
    Directionality: NotRequired[DirectionalityType],  # (2)
```

1. See [:material-code-brackets: TerminologyDataFormatType](./literals.md#terminologydataformattype) 
2. See [:material-code-brackets: DirectionalityType](./literals.md#directionalitytype) 
## OutputDataConfigTypeDef

```python
# OutputDataConfigTypeDef definition

class OutputDataConfigTypeDef(TypedDict):
    S3Uri: str,
    EncryptionKey: NotRequired[EncryptionKeyTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef) 
## TerminologyPropertiesTypeDef

```python
# TerminologyPropertiesTypeDef definition

class TerminologyPropertiesTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    Arn: NotRequired[str],
    SourceLanguageCode: NotRequired[str],
    TargetLanguageCodes: NotRequired[List[str]],
    EncryptionKey: NotRequired[EncryptionKeyTypeDef],  # (1)
    SizeBytes: NotRequired[int],
    TermCount: NotRequired[int],
    CreatedAt: NotRequired[datetime],
    LastUpdatedAt: NotRequired[datetime],
    Directionality: NotRequired[DirectionalityType],  # (2)
    Message: NotRequired[str],
    SkippedTermCount: NotRequired[int],
    Format: NotRequired[TerminologyDataFormatType],  # (3)
```

1. See [:material-code-braces: EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef) 
2. See [:material-code-brackets: DirectionalityType](./literals.md#directionalitytype) 
3. See [:material-code-brackets: TerminologyDataFormatType](./literals.md#terminologydataformattype) 
## ParallelDataPropertiesTypeDef

```python
# ParallelDataPropertiesTypeDef definition

class ParallelDataPropertiesTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[ParallelDataStatusType],  # (1)
    SourceLanguageCode: NotRequired[str],
    TargetLanguageCodes: NotRequired[List[str]],
    ParallelDataConfig: NotRequired[ParallelDataConfigTypeDef],  # (2)
    Message: NotRequired[str],
    ImportedDataSize: NotRequired[int],
    ImportedRecordCount: NotRequired[int],
    FailedRecordCount: NotRequired[int],
    SkippedRecordCount: NotRequired[int],
    EncryptionKey: NotRequired[EncryptionKeyTypeDef],  # (3)
    CreatedAt: NotRequired[datetime],
    LastUpdatedAt: NotRequired[datetime],
    LatestUpdateAttemptStatus: NotRequired[ParallelDataStatusType],  # (1)
    LatestUpdateAttemptAt: NotRequired[datetime],
```

1. See [:material-code-brackets: ParallelDataStatusType](./literals.md#paralleldatastatustype) 
2. See [:material-code-braces: ParallelDataConfigTypeDef](./type_defs.md#paralleldataconfigtypedef) 
3. See [:material-code-braces: EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef) 
4. See [:material-code-brackets: ParallelDataStatusType](./literals.md#paralleldatastatustype) 
## UpdateParallelDataRequestRequestTypeDef

```python
# UpdateParallelDataRequestRequestTypeDef definition

class UpdateParallelDataRequestRequestTypeDef(TypedDict):
    Name: str,
    ParallelDataConfig: ParallelDataConfigTypeDef,  # (1)
    ClientToken: str,
    Description: NotRequired[str],
```

1. See [:material-code-braces: ParallelDataConfigTypeDef](./type_defs.md#paralleldataconfigtypedef) 
## CreateParallelDataRequestRequestTypeDef

```python
# CreateParallelDataRequestRequestTypeDef definition

class CreateParallelDataRequestRequestTypeDef(TypedDict):
    Name: str,
    ParallelDataConfig: ParallelDataConfigTypeDef,  # (1)
    ClientToken: str,
    Description: NotRequired[str],
    EncryptionKey: NotRequired[EncryptionKeyTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: ParallelDataConfigTypeDef](./type_defs.md#paralleldataconfigtypedef) 
2. See [:material-code-braces: EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateParallelDataResponseTypeDef

```python
# CreateParallelDataResponseTypeDef definition

class CreateParallelDataResponseTypeDef(TypedDict):
    Name: str,
    Status: ParallelDataStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ParallelDataStatusType](./literals.md#paralleldatastatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteParallelDataResponseTypeDef

```python
# DeleteParallelDataResponseTypeDef definition

class DeleteParallelDataResponseTypeDef(TypedDict):
    Name: str,
    Status: ParallelDataStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ParallelDataStatusType](./literals.md#paralleldatastatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTextTranslationJobResponseTypeDef

```python
# StartTextTranslationJobResponseTypeDef definition

class StartTextTranslationJobResponseTypeDef(TypedDict):
    JobId: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopTextTranslationJobResponseTypeDef

```python
# StopTextTranslationJobResponseTypeDef definition

class StopTextTranslationJobResponseTypeDef(TypedDict):
    JobId: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateParallelDataResponseTypeDef

```python
# UpdateParallelDataResponseTypeDef definition

class UpdateParallelDataResponseTypeDef(TypedDict):
    Name: str,
    Status: ParallelDataStatusType,  # (1)
    LatestUpdateAttemptStatus: ParallelDataStatusType,  # (1)
    LatestUpdateAttemptAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ParallelDataStatusType](./literals.md#paralleldatastatustype) 
2. See [:material-code-brackets: ParallelDataStatusType](./literals.md#paralleldatastatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLanguagesResponseTypeDef

```python
# ListLanguagesResponseTypeDef definition

class ListLanguagesResponseTypeDef(TypedDict):
    Languages: List[LanguageTypeDef],  # (1)
    DisplayLanguageCode: DisplayLanguageCodeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LanguageTypeDef](./type_defs.md#languagetypedef) 
2. See [:material-code-brackets: DisplayLanguageCodeType](./literals.md#displaylanguagecodetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTerminologiesRequestPaginateTypeDef

```python
# ListTerminologiesRequestPaginateTypeDef definition

class ListTerminologiesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## TranslateTextRequestRequestTypeDef

```python
# TranslateTextRequestRequestTypeDef definition

class TranslateTextRequestRequestTypeDef(TypedDict):
    Text: str,
    SourceLanguageCode: str,
    TargetLanguageCode: str,
    TerminologyNames: NotRequired[Sequence[str]],
    Settings: NotRequired[TranslationSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: TranslationSettingsTypeDef](./type_defs.md#translationsettingstypedef) 
## TextTranslationJobFilterTypeDef

```python
# TextTranslationJobFilterTypeDef definition

class TextTranslationJobFilterTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    SubmittedBeforeTime: NotRequired[TimestampTypeDef],
    SubmittedAfterTime: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## TranslateDocumentResponseTypeDef

```python
# TranslateDocumentResponseTypeDef definition

class TranslateDocumentResponseTypeDef(TypedDict):
    TranslatedDocument: TranslatedDocumentTypeDef,  # (1)
    SourceLanguageCode: str,
    TargetLanguageCode: str,
    AppliedTerminologies: List[AppliedTerminologyTypeDef],  # (2)
    AppliedSettings: TranslationSettingsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TranslatedDocumentTypeDef](./type_defs.md#translateddocumenttypedef) 
2. See [:material-code-braces: AppliedTerminologyTypeDef](./type_defs.md#appliedterminologytypedef) 
3. See [:material-code-braces: TranslationSettingsTypeDef](./type_defs.md#translationsettingstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TranslateTextResponseTypeDef

```python
# TranslateTextResponseTypeDef definition

class TranslateTextResponseTypeDef(TypedDict):
    TranslatedText: str,
    SourceLanguageCode: str,
    TargetLanguageCode: str,
    AppliedTerminologies: List[AppliedTerminologyTypeDef],  # (1)
    AppliedSettings: TranslationSettingsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AppliedTerminologyTypeDef](./type_defs.md#appliedterminologytypedef) 
2. See [:material-code-braces: TranslationSettingsTypeDef](./type_defs.md#translationsettingstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TranslateDocumentRequestRequestTypeDef

```python
# TranslateDocumentRequestRequestTypeDef definition

class TranslateDocumentRequestRequestTypeDef(TypedDict):
    Document: DocumentTypeDef,  # (1)
    SourceLanguageCode: str,
    TargetLanguageCode: str,
    TerminologyNames: NotRequired[Sequence[str]],
    Settings: NotRequired[TranslationSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-braces: TranslationSettingsTypeDef](./type_defs.md#translationsettingstypedef) 
## ImportTerminologyRequestRequestTypeDef

```python
# ImportTerminologyRequestRequestTypeDef definition

class ImportTerminologyRequestRequestTypeDef(TypedDict):
    Name: str,
    MergeStrategy: MergeStrategyType,  # (1)
    TerminologyData: TerminologyDataTypeDef,  # (2)
    Description: NotRequired[str],
    EncryptionKey: NotRequired[EncryptionKeyTypeDef],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: MergeStrategyType](./literals.md#mergestrategytype) 
2. See [:material-code-braces: TerminologyDataTypeDef](./type_defs.md#terminologydatatypedef) 
3. See [:material-code-braces: EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartTextTranslationJobRequestRequestTypeDef

```python
# StartTextTranslationJobRequestRequestTypeDef definition

class StartTextTranslationJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    SourceLanguageCode: str,
    TargetLanguageCodes: Sequence[str],
    ClientToken: str,
    JobName: NotRequired[str],
    TerminologyNames: NotRequired[Sequence[str]],
    ParallelDataNames: NotRequired[Sequence[str]],
    Settings: NotRequired[TranslationSettingsTypeDef],  # (3)
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-braces: TranslationSettingsTypeDef](./type_defs.md#translationsettingstypedef) 
## TextTranslationJobPropertiesTypeDef

```python
# TextTranslationJobPropertiesTypeDef definition

class TextTranslationJobPropertiesTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    JobDetails: NotRequired[JobDetailsTypeDef],  # (2)
    SourceLanguageCode: NotRequired[str],
    TargetLanguageCodes: NotRequired[List[str]],
    TerminologyNames: NotRequired[List[str]],
    ParallelDataNames: NotRequired[List[str]],
    Message: NotRequired[str],
    SubmittedTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    InputDataConfig: NotRequired[InputDataConfigTypeDef],  # (3)
    OutputDataConfig: NotRequired[OutputDataConfigTypeDef],  # (4)
    DataAccessRoleArn: NotRequired[str],
    Settings: NotRequired[TranslationSettingsTypeDef],  # (5)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: JobDetailsTypeDef](./type_defs.md#jobdetailstypedef) 
3. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
4. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
5. See [:material-code-braces: TranslationSettingsTypeDef](./type_defs.md#translationsettingstypedef) 
## GetTerminologyResponseTypeDef

```python
# GetTerminologyResponseTypeDef definition

class GetTerminologyResponseTypeDef(TypedDict):
    TerminologyProperties: TerminologyPropertiesTypeDef,  # (1)
    TerminologyDataLocation: TerminologyDataLocationTypeDef,  # (2)
    AuxiliaryDataLocation: TerminologyDataLocationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TerminologyPropertiesTypeDef](./type_defs.md#terminologypropertiestypedef) 
2. See [:material-code-braces: TerminologyDataLocationTypeDef](./type_defs.md#terminologydatalocationtypedef) 
3. See [:material-code-braces: TerminologyDataLocationTypeDef](./type_defs.md#terminologydatalocationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportTerminologyResponseTypeDef

```python
# ImportTerminologyResponseTypeDef definition

class ImportTerminologyResponseTypeDef(TypedDict):
    TerminologyProperties: TerminologyPropertiesTypeDef,  # (1)
    AuxiliaryDataLocation: TerminologyDataLocationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TerminologyPropertiesTypeDef](./type_defs.md#terminologypropertiestypedef) 
2. See [:material-code-braces: TerminologyDataLocationTypeDef](./type_defs.md#terminologydatalocationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTerminologiesResponseTypeDef

```python
# ListTerminologiesResponseTypeDef definition

class ListTerminologiesResponseTypeDef(TypedDict):
    TerminologyPropertiesList: List[TerminologyPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TerminologyPropertiesTypeDef](./type_defs.md#terminologypropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetParallelDataResponseTypeDef

```python
# GetParallelDataResponseTypeDef definition

class GetParallelDataResponseTypeDef(TypedDict):
    ParallelDataProperties: ParallelDataPropertiesTypeDef,  # (1)
    DataLocation: ParallelDataDataLocationTypeDef,  # (2)
    AuxiliaryDataLocation: ParallelDataDataLocationTypeDef,  # (2)
    LatestUpdateAttemptAuxiliaryDataLocation: ParallelDataDataLocationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ParallelDataPropertiesTypeDef](./type_defs.md#paralleldatapropertiestypedef) 
2. See [:material-code-braces: ParallelDataDataLocationTypeDef](./type_defs.md#paralleldatadatalocationtypedef) 
3. See [:material-code-braces: ParallelDataDataLocationTypeDef](./type_defs.md#paralleldatadatalocationtypedef) 
4. See [:material-code-braces: ParallelDataDataLocationTypeDef](./type_defs.md#paralleldatadatalocationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListParallelDataResponseTypeDef

```python
# ListParallelDataResponseTypeDef definition

class ListParallelDataResponseTypeDef(TypedDict):
    ParallelDataPropertiesList: List[ParallelDataPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ParallelDataPropertiesTypeDef](./type_defs.md#paralleldatapropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTextTranslationJobsRequestRequestTypeDef

```python
# ListTextTranslationJobsRequestRequestTypeDef definition

class ListTextTranslationJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[TextTranslationJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: TextTranslationJobFilterTypeDef](./type_defs.md#texttranslationjobfiltertypedef) 
## DescribeTextTranslationJobResponseTypeDef

```python
# DescribeTextTranslationJobResponseTypeDef definition

class DescribeTextTranslationJobResponseTypeDef(TypedDict):
    TextTranslationJobProperties: TextTranslationJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TextTranslationJobPropertiesTypeDef](./type_defs.md#texttranslationjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTextTranslationJobsResponseTypeDef

```python
# ListTextTranslationJobsResponseTypeDef definition

class ListTextTranslationJobsResponseTypeDef(TypedDict):
    TextTranslationJobPropertiesList: List[TextTranslationJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TextTranslationJobPropertiesTypeDef](./type_defs.md#texttranslationjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
