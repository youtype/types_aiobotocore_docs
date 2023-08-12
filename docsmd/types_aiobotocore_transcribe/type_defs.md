# Type definitions

> [Index](../README.md) > [TranscribeService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [TranscribeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
    type annotations stubs module [types-aiobotocore-transcribe](https://pypi.org/project/types-aiobotocore-transcribe/).



## AbsoluteTimeRangeTypeDef

```python
# AbsoluteTimeRangeTypeDef definition

class AbsoluteTimeRangeTypeDef(TypedDict):
    StartTime: NotRequired[int],
    EndTime: NotRequired[int],
    First: NotRequired[int],
    Last: NotRequired[int],
```

## ContentRedactionTypeDef

```python
# ContentRedactionTypeDef definition

class ContentRedactionTypeDef(TypedDict):
    RedactionType: RedactionTypeType,  # (1)
    RedactionOutput: RedactionOutputType,  # (2)
    PiiEntityTypes: NotRequired[List[PiiEntityTypeType]],  # (3)
```

1. See [:material-code-brackets: RedactionTypeType](./literals.md#redactiontypetype) 
2. See [:material-code-brackets: RedactionOutputType](./literals.md#redactionoutputtype) 
3. See [:material-code-brackets: PiiEntityTypeType](./literals.md#piientitytypetype) 
## LanguageIdSettingsTypeDef

```python
# LanguageIdSettingsTypeDef definition

class LanguageIdSettingsTypeDef(TypedDict):
    VocabularyName: NotRequired[str],
    VocabularyFilterName: NotRequired[str],
    LanguageModelName: NotRequired[str],
```

## CallAnalyticsJobSummaryTypeDef

```python
# CallAnalyticsJobSummaryTypeDef definition

class CallAnalyticsJobSummaryTypeDef(TypedDict):
    CallAnalyticsJobName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    StartTime: NotRequired[datetime],
    CompletionTime: NotRequired[datetime],
    LanguageCode: NotRequired[LanguageCodeType],  # (1)
    CallAnalyticsJobStatus: NotRequired[CallAnalyticsJobStatusType],  # (2)
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-brackets: CallAnalyticsJobStatusType](./literals.md#callanalyticsjobstatustype) 
## ChannelDefinitionTypeDef

```python
# ChannelDefinitionTypeDef definition

class ChannelDefinitionTypeDef(TypedDict):
    ChannelId: NotRequired[int],
    ParticipantRole: NotRequired[ParticipantRoleType],  # (1)
```

1. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
## MediaTypeDef

```python
# MediaTypeDef definition

class MediaTypeDef(TypedDict):
    MediaFileUri: NotRequired[str],
    RedactedMediaFileUri: NotRequired[str],
```

## TranscriptTypeDef

```python
# TranscriptTypeDef definition

class TranscriptTypeDef(TypedDict):
    TranscriptFileUri: NotRequired[str],
    RedactedTranscriptFileUri: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## InputDataConfigTypeDef

```python
# InputDataConfigTypeDef definition

class InputDataConfigTypeDef(TypedDict):
    S3Uri: str,
    DataAccessRoleArn: str,
    TuningDataS3Uri: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DeleteCallAnalyticsCategoryRequestRequestTypeDef

```python
# DeleteCallAnalyticsCategoryRequestRequestTypeDef definition

class DeleteCallAnalyticsCategoryRequestRequestTypeDef(TypedDict):
    CategoryName: str,
```

## DeleteCallAnalyticsJobRequestRequestTypeDef

```python
# DeleteCallAnalyticsJobRequestRequestTypeDef definition

class DeleteCallAnalyticsJobRequestRequestTypeDef(TypedDict):
    CallAnalyticsJobName: str,
```

## DeleteLanguageModelRequestRequestTypeDef

```python
# DeleteLanguageModelRequestRequestTypeDef definition

class DeleteLanguageModelRequestRequestTypeDef(TypedDict):
    ModelName: str,
```

## DeleteMedicalTranscriptionJobRequestRequestTypeDef

```python
# DeleteMedicalTranscriptionJobRequestRequestTypeDef definition

class DeleteMedicalTranscriptionJobRequestRequestTypeDef(TypedDict):
    MedicalTranscriptionJobName: str,
```

## DeleteMedicalVocabularyRequestRequestTypeDef

```python
# DeleteMedicalVocabularyRequestRequestTypeDef definition

class DeleteMedicalVocabularyRequestRequestTypeDef(TypedDict):
    VocabularyName: str,
```

## DeleteTranscriptionJobRequestRequestTypeDef

```python
# DeleteTranscriptionJobRequestRequestTypeDef definition

class DeleteTranscriptionJobRequestRequestTypeDef(TypedDict):
    TranscriptionJobName: str,
```

## DeleteVocabularyFilterRequestRequestTypeDef

```python
# DeleteVocabularyFilterRequestRequestTypeDef definition

class DeleteVocabularyFilterRequestRequestTypeDef(TypedDict):
    VocabularyFilterName: str,
```

## DeleteVocabularyRequestRequestTypeDef

```python
# DeleteVocabularyRequestRequestTypeDef definition

class DeleteVocabularyRequestRequestTypeDef(TypedDict):
    VocabularyName: str,
```

## DescribeLanguageModelRequestRequestTypeDef

```python
# DescribeLanguageModelRequestRequestTypeDef definition

class DescribeLanguageModelRequestRequestTypeDef(TypedDict):
    ModelName: str,
```

## GetCallAnalyticsCategoryRequestRequestTypeDef

```python
# GetCallAnalyticsCategoryRequestRequestTypeDef definition

class GetCallAnalyticsCategoryRequestRequestTypeDef(TypedDict):
    CategoryName: str,
```

## GetCallAnalyticsJobRequestRequestTypeDef

```python
# GetCallAnalyticsJobRequestRequestTypeDef definition

class GetCallAnalyticsJobRequestRequestTypeDef(TypedDict):
    CallAnalyticsJobName: str,
```

## GetMedicalTranscriptionJobRequestRequestTypeDef

```python
# GetMedicalTranscriptionJobRequestRequestTypeDef definition

class GetMedicalTranscriptionJobRequestRequestTypeDef(TypedDict):
    MedicalTranscriptionJobName: str,
```

## GetMedicalVocabularyRequestRequestTypeDef

```python
# GetMedicalVocabularyRequestRequestTypeDef definition

class GetMedicalVocabularyRequestRequestTypeDef(TypedDict):
    VocabularyName: str,
```

## GetTranscriptionJobRequestRequestTypeDef

```python
# GetTranscriptionJobRequestRequestTypeDef definition

class GetTranscriptionJobRequestRequestTypeDef(TypedDict):
    TranscriptionJobName: str,
```

## GetVocabularyFilterRequestRequestTypeDef

```python
# GetVocabularyFilterRequestRequestTypeDef definition

class GetVocabularyFilterRequestRequestTypeDef(TypedDict):
    VocabularyFilterName: str,
```

## GetVocabularyRequestRequestTypeDef

```python
# GetVocabularyRequestRequestTypeDef definition

class GetVocabularyRequestRequestTypeDef(TypedDict):
    VocabularyName: str,
```

## RelativeTimeRangeTypeDef

```python
# RelativeTimeRangeTypeDef definition

class RelativeTimeRangeTypeDef(TypedDict):
    StartPercentage: NotRequired[int],
    EndPercentage: NotRequired[int],
    First: NotRequired[int],
    Last: NotRequired[int],
```

## JobExecutionSettingsTypeDef

```python
# JobExecutionSettingsTypeDef definition

class JobExecutionSettingsTypeDef(TypedDict):
    AllowDeferredExecution: NotRequired[bool],
    DataAccessRoleArn: NotRequired[str],
```

## LanguageCodeItemTypeDef

```python
# LanguageCodeItemTypeDef definition

class LanguageCodeItemTypeDef(TypedDict):
    LanguageCode: NotRequired[LanguageCodeType],  # (1)
    DurationInSeconds: NotRequired[float],
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## ListCallAnalyticsCategoriesRequestRequestTypeDef

```python
# ListCallAnalyticsCategoriesRequestRequestTypeDef definition

class ListCallAnalyticsCategoriesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListCallAnalyticsJobsRequestRequestTypeDef

```python
# ListCallAnalyticsJobsRequestRequestTypeDef definition

class ListCallAnalyticsJobsRequestRequestTypeDef(TypedDict):
    Status: NotRequired[CallAnalyticsJobStatusType],  # (1)
    JobNameContains: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: CallAnalyticsJobStatusType](./literals.md#callanalyticsjobstatustype) 
## ListLanguageModelsRequestRequestTypeDef

```python
# ListLanguageModelsRequestRequestTypeDef definition

class ListLanguageModelsRequestRequestTypeDef(TypedDict):
    StatusEquals: NotRequired[ModelStatusType],  # (1)
    NameContains: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
## ListMedicalTranscriptionJobsRequestRequestTypeDef

```python
# ListMedicalTranscriptionJobsRequestRequestTypeDef definition

class ListMedicalTranscriptionJobsRequestRequestTypeDef(TypedDict):
    Status: NotRequired[TranscriptionJobStatusType],  # (1)
    JobNameContains: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: TranscriptionJobStatusType](./literals.md#transcriptionjobstatustype) 
## MedicalTranscriptionJobSummaryTypeDef

```python
# MedicalTranscriptionJobSummaryTypeDef definition

class MedicalTranscriptionJobSummaryTypeDef(TypedDict):
    MedicalTranscriptionJobName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    StartTime: NotRequired[datetime],
    CompletionTime: NotRequired[datetime],
    LanguageCode: NotRequired[LanguageCodeType],  # (1)
    TranscriptionJobStatus: NotRequired[TranscriptionJobStatusType],  # (2)
    FailureReason: NotRequired[str],
    OutputLocationType: NotRequired[OutputLocationTypeType],  # (3)
    Specialty: NotRequired[SpecialtyType],  # (4)
    ContentIdentificationType: NotRequired[MedicalContentIdentificationTypeType],  # (5)
    Type: NotRequired[TypeType],  # (6)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-brackets: TranscriptionJobStatusType](./literals.md#transcriptionjobstatustype) 
3. See [:material-code-brackets: OutputLocationTypeType](./literals.md#outputlocationtypetype) 
4. See [:material-code-brackets: SpecialtyType](./literals.md#specialtytype) 
5. See [:material-code-brackets: MedicalContentIdentificationTypeType](./literals.md#medicalcontentidentificationtypetype) 
6. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## ListMedicalVocabulariesRequestRequestTypeDef

```python
# ListMedicalVocabulariesRequestRequestTypeDef definition

class ListMedicalVocabulariesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    StateEquals: NotRequired[VocabularyStateType],  # (1)
    NameContains: NotRequired[str],
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
## VocabularyInfoTypeDef

```python
# VocabularyInfoTypeDef definition

class VocabularyInfoTypeDef(TypedDict):
    VocabularyName: NotRequired[str],
    LanguageCode: NotRequired[LanguageCodeType],  # (1)
    LastModifiedTime: NotRequired[datetime],
    VocabularyState: NotRequired[VocabularyStateType],  # (2)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListTranscriptionJobsRequestRequestTypeDef

```python
# ListTranscriptionJobsRequestRequestTypeDef definition

class ListTranscriptionJobsRequestRequestTypeDef(TypedDict):
    Status: NotRequired[TranscriptionJobStatusType],  # (1)
    JobNameContains: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: TranscriptionJobStatusType](./literals.md#transcriptionjobstatustype) 
## ListVocabulariesRequestRequestTypeDef

```python
# ListVocabulariesRequestRequestTypeDef definition

class ListVocabulariesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    StateEquals: NotRequired[VocabularyStateType],  # (1)
    NameContains: NotRequired[str],
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
## ListVocabularyFiltersRequestRequestTypeDef

```python
# ListVocabularyFiltersRequestRequestTypeDef definition

class ListVocabularyFiltersRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
```

## VocabularyFilterInfoTypeDef

```python
# VocabularyFilterInfoTypeDef definition

class VocabularyFilterInfoTypeDef(TypedDict):
    VocabularyFilterName: NotRequired[str],
    LanguageCode: NotRequired[LanguageCodeType],  # (1)
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## MedicalTranscriptTypeDef

```python
# MedicalTranscriptTypeDef definition

class MedicalTranscriptTypeDef(TypedDict):
    TranscriptFileUri: NotRequired[str],
```

## MedicalTranscriptionSettingTypeDef

```python
# MedicalTranscriptionSettingTypeDef definition

class MedicalTranscriptionSettingTypeDef(TypedDict):
    ShowSpeakerLabels: NotRequired[bool],
    MaxSpeakerLabels: NotRequired[int],
    ChannelIdentification: NotRequired[bool],
    ShowAlternatives: NotRequired[bool],
    MaxAlternatives: NotRequired[int],
    VocabularyName: NotRequired[str],
```

## ModelSettingsTypeDef

```python
# ModelSettingsTypeDef definition

class ModelSettingsTypeDef(TypedDict):
    LanguageModelName: NotRequired[str],
```

## SettingsTypeDef

```python
# SettingsTypeDef definition

class SettingsTypeDef(TypedDict):
    VocabularyName: NotRequired[str],
    ShowSpeakerLabels: NotRequired[bool],
    MaxSpeakerLabels: NotRequired[int],
    ChannelIdentification: NotRequired[bool],
    ShowAlternatives: NotRequired[bool],
    MaxAlternatives: NotRequired[int],
    VocabularyFilterName: NotRequired[str],
    VocabularyFilterMethod: NotRequired[VocabularyFilterMethodType],  # (1)
```

1. See [:material-code-brackets: VocabularyFilterMethodType](./literals.md#vocabularyfiltermethodtype) 
## SubtitlesTypeDef

```python
# SubtitlesTypeDef definition

class SubtitlesTypeDef(TypedDict):
    Formats: NotRequired[Sequence[SubtitleFormatType]],  # (1)
    OutputStartIndex: NotRequired[int],
```

1. See [:material-code-brackets: SubtitleFormatType](./literals.md#subtitleformattype) 
## ToxicityDetectionSettingsTypeDef

```python
# ToxicityDetectionSettingsTypeDef definition

class ToxicityDetectionSettingsTypeDef(TypedDict):
    ToxicityCategories: List[ToxicityCategoryType],  # (1)
```

1. See [:material-code-brackets: ToxicityCategoryType](./literals.md#toxicitycategorytype) 
## SubtitlesOutputTypeDef

```python
# SubtitlesOutputTypeDef definition

class SubtitlesOutputTypeDef(TypedDict):
    Formats: NotRequired[List[SubtitleFormatType]],  # (1)
    SubtitleFileUris: NotRequired[List[str]],
    OutputStartIndex: NotRequired[int],
```

1. See [:material-code-brackets: SubtitleFormatType](./literals.md#subtitleformattype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateMedicalVocabularyRequestRequestTypeDef

```python
# UpdateMedicalVocabularyRequestRequestTypeDef definition

class UpdateMedicalVocabularyRequestRequestTypeDef(TypedDict):
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    VocabularyFileUri: str,
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## UpdateVocabularyFilterRequestRequestTypeDef

```python
# UpdateVocabularyFilterRequestRequestTypeDef definition

class UpdateVocabularyFilterRequestRequestTypeDef(TypedDict):
    VocabularyFilterName: str,
    Words: NotRequired[Sequence[str]],
    VocabularyFilterFileUri: NotRequired[str],
    DataAccessRoleArn: NotRequired[str],
```

## UpdateVocabularyRequestRequestTypeDef

```python
# UpdateVocabularyRequestRequestTypeDef definition

class UpdateVocabularyRequestRequestTypeDef(TypedDict):
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    Phrases: NotRequired[Sequence[str]],
    VocabularyFileUri: NotRequired[str],
    DataAccessRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## CallAnalyticsJobSettingsTypeDef

```python
# CallAnalyticsJobSettingsTypeDef definition

class CallAnalyticsJobSettingsTypeDef(TypedDict):
    VocabularyName: NotRequired[str],
    VocabularyFilterName: NotRequired[str],
    VocabularyFilterMethod: NotRequired[VocabularyFilterMethodType],  # (1)
    LanguageModelName: NotRequired[str],
    ContentRedaction: NotRequired[ContentRedactionTypeDef],  # (2)
    LanguageOptions: NotRequired[List[LanguageCodeType]],  # (3)
    LanguageIdSettings: NotRequired[Dict[LanguageCodeType, LanguageIdSettingsTypeDef]],  # (4)
```

1. See [:material-code-brackets: VocabularyFilterMethodType](./literals.md#vocabularyfiltermethodtype) 
2. See [:material-code-braces: ContentRedactionTypeDef](./type_defs.md#contentredactiontypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) [:material-code-braces: LanguageIdSettingsTypeDef](./type_defs.md#languageidsettingstypedef) 
## CreateMedicalVocabularyResponseTypeDef

```python
# CreateMedicalVocabularyResponseTypeDef definition

class CreateMedicalVocabularyResponseTypeDef(TypedDict):
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    VocabularyState: VocabularyStateType,  # (2)
    LastModifiedTime: datetime,
    FailureReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVocabularyFilterResponseTypeDef

```python
# CreateVocabularyFilterResponseTypeDef definition

class CreateVocabularyFilterResponseTypeDef(TypedDict):
    VocabularyFilterName: str,
    LanguageCode: LanguageCodeType,  # (1)
    LastModifiedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVocabularyResponseTypeDef

```python
# CreateVocabularyResponseTypeDef definition

class CreateVocabularyResponseTypeDef(TypedDict):
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    VocabularyState: VocabularyStateType,  # (2)
    LastModifiedTime: datetime,
    FailureReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMedicalVocabularyResponseTypeDef

```python
# GetMedicalVocabularyResponseTypeDef definition

class GetMedicalVocabularyResponseTypeDef(TypedDict):
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    VocabularyState: VocabularyStateType,  # (2)
    LastModifiedTime: datetime,
    FailureReason: str,
    DownloadUri: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVocabularyFilterResponseTypeDef

```python
# GetVocabularyFilterResponseTypeDef definition

class GetVocabularyFilterResponseTypeDef(TypedDict):
    VocabularyFilterName: str,
    LanguageCode: LanguageCodeType,  # (1)
    LastModifiedTime: datetime,
    DownloadUri: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVocabularyResponseTypeDef

```python
# GetVocabularyResponseTypeDef definition

class GetVocabularyResponseTypeDef(TypedDict):
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    VocabularyState: VocabularyStateType,  # (2)
    LastModifiedTime: datetime,
    FailureReason: str,
    DownloadUri: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCallAnalyticsJobsResponseTypeDef

```python
# ListCallAnalyticsJobsResponseTypeDef definition

class ListCallAnalyticsJobsResponseTypeDef(TypedDict):
    Status: CallAnalyticsJobStatusType,  # (1)
    NextToken: str,
    CallAnalyticsJobSummaries: List[CallAnalyticsJobSummaryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: CallAnalyticsJobStatusType](./literals.md#callanalyticsjobstatustype) 
2. See [:material-code-braces: CallAnalyticsJobSummaryTypeDef](./type_defs.md#callanalyticsjobsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMedicalVocabularyResponseTypeDef

```python
# UpdateMedicalVocabularyResponseTypeDef definition

class UpdateMedicalVocabularyResponseTypeDef(TypedDict):
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    LastModifiedTime: datetime,
    VocabularyState: VocabularyStateType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVocabularyFilterResponseTypeDef

```python
# UpdateVocabularyFilterResponseTypeDef definition

class UpdateVocabularyFilterResponseTypeDef(TypedDict):
    VocabularyFilterName: str,
    LanguageCode: LanguageCodeType,  # (1)
    LastModifiedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVocabularyResponseTypeDef

```python
# UpdateVocabularyResponseTypeDef definition

class UpdateVocabularyResponseTypeDef(TypedDict):
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    LastModifiedTime: datetime,
    VocabularyState: VocabularyStateType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLanguageModelResponseTypeDef

```python
# CreateLanguageModelResponseTypeDef definition

class CreateLanguageModelResponseTypeDef(TypedDict):
    LanguageCode: CLMLanguageCodeType,  # (1)
    BaseModelName: BaseModelNameType,  # (2)
    ModelName: str,
    InputDataConfig: InputDataConfigTypeDef,  # (3)
    ModelStatus: ModelStatusType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: CLMLanguageCodeType](./literals.md#clmlanguagecodetype) 
2. See [:material-code-brackets: BaseModelNameType](./literals.md#basemodelnametype) 
3. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
4. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LanguageModelTypeDef

```python
# LanguageModelTypeDef definition

class LanguageModelTypeDef(TypedDict):
    ModelName: NotRequired[str],
    CreateTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    LanguageCode: NotRequired[CLMLanguageCodeType],  # (1)
    BaseModelName: NotRequired[BaseModelNameType],  # (2)
    ModelStatus: NotRequired[ModelStatusType],  # (3)
    UpgradeAvailability: NotRequired[bool],
    FailureReason: NotRequired[str],
    InputDataConfig: NotRequired[InputDataConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: CLMLanguageCodeType](./literals.md#clmlanguagecodetype) 
2. See [:material-code-brackets: BaseModelNameType](./literals.md#basemodelnametype) 
3. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
4. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
## CreateLanguageModelRequestRequestTypeDef

```python
# CreateLanguageModelRequestRequestTypeDef definition

class CreateLanguageModelRequestRequestTypeDef(TypedDict):
    LanguageCode: CLMLanguageCodeType,  # (1)
    BaseModelName: BaseModelNameType,  # (2)
    ModelName: str,
    InputDataConfig: InputDataConfigTypeDef,  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: CLMLanguageCodeType](./literals.md#clmlanguagecodetype) 
2. See [:material-code-brackets: BaseModelNameType](./literals.md#basemodelnametype) 
3. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateMedicalVocabularyRequestRequestTypeDef

```python
# CreateMedicalVocabularyRequestRequestTypeDef definition

class CreateMedicalVocabularyRequestRequestTypeDef(TypedDict):
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    VocabularyFileUri: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateVocabularyFilterRequestRequestTypeDef

```python
# CreateVocabularyFilterRequestRequestTypeDef definition

class CreateVocabularyFilterRequestRequestTypeDef(TypedDict):
    VocabularyFilterName: str,
    LanguageCode: LanguageCodeType,  # (1)
    Words: NotRequired[Sequence[str]],
    VocabularyFilterFileUri: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    DataAccessRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateVocabularyRequestRequestTypeDef

```python
# CreateVocabularyRequestRequestTypeDef definition

class CreateVocabularyRequestRequestTypeDef(TypedDict):
    VocabularyName: str,
    LanguageCode: LanguageCodeType,  # (1)
    Phrases: NotRequired[Sequence[str]],
    VocabularyFileUri: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    DataAccessRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    ResourceArn: str,
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## InterruptionFilterTypeDef

```python
# InterruptionFilterTypeDef definition

class InterruptionFilterTypeDef(TypedDict):
    Threshold: NotRequired[int],
    ParticipantRole: NotRequired[ParticipantRoleType],  # (1)
    AbsoluteTimeRange: NotRequired[AbsoluteTimeRangeTypeDef],  # (2)
    RelativeTimeRange: NotRequired[RelativeTimeRangeTypeDef],  # (3)
    Negate: NotRequired[bool],
```

1. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
2. See [:material-code-braces: AbsoluteTimeRangeTypeDef](./type_defs.md#absolutetimerangetypedef) 
3. See [:material-code-braces: RelativeTimeRangeTypeDef](./type_defs.md#relativetimerangetypedef) 
## NonTalkTimeFilterTypeDef

```python
# NonTalkTimeFilterTypeDef definition

class NonTalkTimeFilterTypeDef(TypedDict):
    Threshold: NotRequired[int],
    AbsoluteTimeRange: NotRequired[AbsoluteTimeRangeTypeDef],  # (1)
    RelativeTimeRange: NotRequired[RelativeTimeRangeTypeDef],  # (2)
    Negate: NotRequired[bool],
```

1. See [:material-code-braces: AbsoluteTimeRangeTypeDef](./type_defs.md#absolutetimerangetypedef) 
2. See [:material-code-braces: RelativeTimeRangeTypeDef](./type_defs.md#relativetimerangetypedef) 
## SentimentFilterTypeDef

```python
# SentimentFilterTypeDef definition

class SentimentFilterTypeDef(TypedDict):
    Sentiments: Sequence[SentimentValueType],  # (1)
    AbsoluteTimeRange: NotRequired[AbsoluteTimeRangeTypeDef],  # (2)
    RelativeTimeRange: NotRequired[RelativeTimeRangeTypeDef],  # (3)
    ParticipantRole: NotRequired[ParticipantRoleType],  # (4)
    Negate: NotRequired[bool],
```

1. See [:material-code-brackets: SentimentValueType](./literals.md#sentimentvaluetype) 
2. See [:material-code-braces: AbsoluteTimeRangeTypeDef](./type_defs.md#absolutetimerangetypedef) 
3. See [:material-code-braces: RelativeTimeRangeTypeDef](./type_defs.md#relativetimerangetypedef) 
4. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
## TranscriptFilterTypeDef

```python
# TranscriptFilterTypeDef definition

class TranscriptFilterTypeDef(TypedDict):
    TranscriptFilterType: TranscriptFilterTypeType,  # (1)
    Targets: Sequence[str],
    AbsoluteTimeRange: NotRequired[AbsoluteTimeRangeTypeDef],  # (2)
    RelativeTimeRange: NotRequired[RelativeTimeRangeTypeDef],  # (3)
    ParticipantRole: NotRequired[ParticipantRoleType],  # (4)
    Negate: NotRequired[bool],
```

1. See [:material-code-brackets: TranscriptFilterTypeType](./literals.md#transcriptfiltertypetype) 
2. See [:material-code-braces: AbsoluteTimeRangeTypeDef](./type_defs.md#absolutetimerangetypedef) 
3. See [:material-code-braces: RelativeTimeRangeTypeDef](./type_defs.md#relativetimerangetypedef) 
4. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
## ListMedicalTranscriptionJobsResponseTypeDef

```python
# ListMedicalTranscriptionJobsResponseTypeDef definition

class ListMedicalTranscriptionJobsResponseTypeDef(TypedDict):
    Status: TranscriptionJobStatusType,  # (1)
    NextToken: str,
    MedicalTranscriptionJobSummaries: List[MedicalTranscriptionJobSummaryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TranscriptionJobStatusType](./literals.md#transcriptionjobstatustype) 
2. See [:material-code-braces: MedicalTranscriptionJobSummaryTypeDef](./type_defs.md#medicaltranscriptionjobsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMedicalVocabulariesResponseTypeDef

```python
# ListMedicalVocabulariesResponseTypeDef definition

class ListMedicalVocabulariesResponseTypeDef(TypedDict):
    Status: VocabularyStateType,  # (1)
    NextToken: str,
    Vocabularies: List[VocabularyInfoTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-braces: VocabularyInfoTypeDef](./type_defs.md#vocabularyinfotypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVocabulariesResponseTypeDef

```python
# ListVocabulariesResponseTypeDef definition

class ListVocabulariesResponseTypeDef(TypedDict):
    Status: VocabularyStateType,  # (1)
    NextToken: str,
    Vocabularies: List[VocabularyInfoTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-braces: VocabularyInfoTypeDef](./type_defs.md#vocabularyinfotypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVocabularyFiltersResponseTypeDef

```python
# ListVocabularyFiltersResponseTypeDef definition

class ListVocabularyFiltersResponseTypeDef(TypedDict):
    NextToken: str,
    VocabularyFilters: List[VocabularyFilterInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VocabularyFilterInfoTypeDef](./type_defs.md#vocabularyfilterinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MedicalTranscriptionJobTypeDef

```python
# MedicalTranscriptionJobTypeDef definition

class MedicalTranscriptionJobTypeDef(TypedDict):
    MedicalTranscriptionJobName: NotRequired[str],
    TranscriptionJobStatus: NotRequired[TranscriptionJobStatusType],  # (1)
    LanguageCode: NotRequired[LanguageCodeType],  # (2)
    MediaSampleRateHertz: NotRequired[int],
    MediaFormat: NotRequired[MediaFormatType],  # (3)
    Media: NotRequired[MediaTypeDef],  # (4)
    Transcript: NotRequired[MedicalTranscriptTypeDef],  # (5)
    StartTime: NotRequired[datetime],
    CreationTime: NotRequired[datetime],
    CompletionTime: NotRequired[datetime],
    FailureReason: NotRequired[str],
    Settings: NotRequired[MedicalTranscriptionSettingTypeDef],  # (6)
    ContentIdentificationType: NotRequired[MedicalContentIdentificationTypeType],  # (7)
    Specialty: NotRequired[SpecialtyType],  # (8)
    Type: NotRequired[TypeType],  # (9)
    Tags: NotRequired[List[TagTypeDef]],  # (10)
```

1. See [:material-code-brackets: TranscriptionJobStatusType](./literals.md#transcriptionjobstatustype) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
3. See [:material-code-brackets: MediaFormatType](./literals.md#mediaformattype) 
4. See [:material-code-braces: MediaTypeDef](./type_defs.md#mediatypedef) 
5. See [:material-code-braces: MedicalTranscriptTypeDef](./type_defs.md#medicaltranscripttypedef) 
6. See [:material-code-braces: MedicalTranscriptionSettingTypeDef](./type_defs.md#medicaltranscriptionsettingtypedef) 
7. See [:material-code-brackets: MedicalContentIdentificationTypeType](./literals.md#medicalcontentidentificationtypetype) 
8. See [:material-code-brackets: SpecialtyType](./literals.md#specialtytype) 
9. See [:material-code-brackets: TypeType](./literals.md#typetype) 
10. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartMedicalTranscriptionJobRequestRequestTypeDef

```python
# StartMedicalTranscriptionJobRequestRequestTypeDef definition

class StartMedicalTranscriptionJobRequestRequestTypeDef(TypedDict):
    MedicalTranscriptionJobName: str,
    LanguageCode: LanguageCodeType,  # (1)
    Media: MediaTypeDef,  # (2)
    OutputBucketName: str,
    Specialty: SpecialtyType,  # (3)
    Type: TypeType,  # (4)
    MediaSampleRateHertz: NotRequired[int],
    MediaFormat: NotRequired[MediaFormatType],  # (5)
    OutputKey: NotRequired[str],
    OutputEncryptionKMSKeyId: NotRequired[str],
    KMSEncryptionContext: NotRequired[Mapping[str, str]],
    Settings: NotRequired[MedicalTranscriptionSettingTypeDef],  # (6)
    ContentIdentificationType: NotRequired[MedicalContentIdentificationTypeType],  # (7)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (8)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: MediaTypeDef](./type_defs.md#mediatypedef) 
3. See [:material-code-brackets: SpecialtyType](./literals.md#specialtytype) 
4. See [:material-code-brackets: TypeType](./literals.md#typetype) 
5. See [:material-code-brackets: MediaFormatType](./literals.md#mediaformattype) 
6. See [:material-code-braces: MedicalTranscriptionSettingTypeDef](./type_defs.md#medicaltranscriptionsettingtypedef) 
7. See [:material-code-brackets: MedicalContentIdentificationTypeType](./literals.md#medicalcontentidentificationtypetype) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartTranscriptionJobRequestRequestTypeDef

```python
# StartTranscriptionJobRequestRequestTypeDef definition

class StartTranscriptionJobRequestRequestTypeDef(TypedDict):
    TranscriptionJobName: str,
    Media: MediaTypeDef,  # (1)
    LanguageCode: NotRequired[LanguageCodeType],  # (2)
    MediaSampleRateHertz: NotRequired[int],
    MediaFormat: NotRequired[MediaFormatType],  # (3)
    OutputBucketName: NotRequired[str],
    OutputKey: NotRequired[str],
    OutputEncryptionKMSKeyId: NotRequired[str],
    KMSEncryptionContext: NotRequired[Mapping[str, str]],
    Settings: NotRequired[SettingsTypeDef],  # (4)
    ModelSettings: NotRequired[ModelSettingsTypeDef],  # (5)
    JobExecutionSettings: NotRequired[JobExecutionSettingsTypeDef],  # (6)
    ContentRedaction: NotRequired[ContentRedactionTypeDef],  # (7)
    IdentifyLanguage: NotRequired[bool],
    IdentifyMultipleLanguages: NotRequired[bool],
    LanguageOptions: NotRequired[Sequence[LanguageCodeType]],  # (8)
    Subtitles: NotRequired[SubtitlesTypeDef],  # (9)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (10)
    LanguageIdSettings: NotRequired[Mapping[LanguageCodeType, LanguageIdSettingsTypeDef]],  # (11)
    ToxicityDetection: NotRequired[Sequence[ToxicityDetectionSettingsTypeDef]],  # (12)
```

1. See [:material-code-braces: MediaTypeDef](./type_defs.md#mediatypedef) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
3. See [:material-code-brackets: MediaFormatType](./literals.md#mediaformattype) 
4. See [:material-code-braces: SettingsTypeDef](./type_defs.md#settingstypedef) 
5. See [:material-code-braces: ModelSettingsTypeDef](./type_defs.md#modelsettingstypedef) 
6. See [:material-code-braces: JobExecutionSettingsTypeDef](./type_defs.md#jobexecutionsettingstypedef) 
7. See [:material-code-braces: ContentRedactionTypeDef](./type_defs.md#contentredactiontypedef) 
8. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
9. See [:material-code-braces: SubtitlesTypeDef](./type_defs.md#subtitlestypedef) 
10. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
11. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) [:material-code-braces: LanguageIdSettingsTypeDef](./type_defs.md#languageidsettingstypedef) 
12. See [:material-code-braces: ToxicityDetectionSettingsTypeDef](./type_defs.md#toxicitydetectionsettingstypedef) 
## TranscriptionJobSummaryTypeDef

```python
# TranscriptionJobSummaryTypeDef definition

class TranscriptionJobSummaryTypeDef(TypedDict):
    TranscriptionJobName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    StartTime: NotRequired[datetime],
    CompletionTime: NotRequired[datetime],
    LanguageCode: NotRequired[LanguageCodeType],  # (1)
    TranscriptionJobStatus: NotRequired[TranscriptionJobStatusType],  # (2)
    FailureReason: NotRequired[str],
    OutputLocationType: NotRequired[OutputLocationTypeType],  # (3)
    ContentRedaction: NotRequired[ContentRedactionTypeDef],  # (4)
    ModelSettings: NotRequired[ModelSettingsTypeDef],  # (5)
    IdentifyLanguage: NotRequired[bool],
    IdentifyMultipleLanguages: NotRequired[bool],
    IdentifiedLanguageScore: NotRequired[float],
    LanguageCodes: NotRequired[List[LanguageCodeItemTypeDef]],  # (6)
    ToxicityDetection: NotRequired[List[ToxicityDetectionSettingsTypeDef]],  # (7)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-brackets: TranscriptionJobStatusType](./literals.md#transcriptionjobstatustype) 
3. See [:material-code-brackets: OutputLocationTypeType](./literals.md#outputlocationtypetype) 
4. See [:material-code-braces: ContentRedactionTypeDef](./type_defs.md#contentredactiontypedef) 
5. See [:material-code-braces: ModelSettingsTypeDef](./type_defs.md#modelsettingstypedef) 
6. See [:material-code-braces: LanguageCodeItemTypeDef](./type_defs.md#languagecodeitemtypedef) 
7. See [:material-code-braces: ToxicityDetectionSettingsTypeDef](./type_defs.md#toxicitydetectionsettingstypedef) 
## TranscriptionJobTypeDef

```python
# TranscriptionJobTypeDef definition

class TranscriptionJobTypeDef(TypedDict):
    TranscriptionJobName: NotRequired[str],
    TranscriptionJobStatus: NotRequired[TranscriptionJobStatusType],  # (1)
    LanguageCode: NotRequired[LanguageCodeType],  # (2)
    MediaSampleRateHertz: NotRequired[int],
    MediaFormat: NotRequired[MediaFormatType],  # (3)
    Media: NotRequired[MediaTypeDef],  # (4)
    Transcript: NotRequired[TranscriptTypeDef],  # (5)
    StartTime: NotRequired[datetime],
    CreationTime: NotRequired[datetime],
    CompletionTime: NotRequired[datetime],
    FailureReason: NotRequired[str],
    Settings: NotRequired[SettingsTypeDef],  # (6)
    ModelSettings: NotRequired[ModelSettingsTypeDef],  # (7)
    JobExecutionSettings: NotRequired[JobExecutionSettingsTypeDef],  # (8)
    ContentRedaction: NotRequired[ContentRedactionTypeDef],  # (9)
    IdentifyLanguage: NotRequired[bool],
    IdentifyMultipleLanguages: NotRequired[bool],
    LanguageOptions: NotRequired[List[LanguageCodeType]],  # (10)
    IdentifiedLanguageScore: NotRequired[float],
    LanguageCodes: NotRequired[List[LanguageCodeItemTypeDef]],  # (11)
    Tags: NotRequired[List[TagTypeDef]],  # (12)
    Subtitles: NotRequired[SubtitlesOutputTypeDef],  # (13)
    LanguageIdSettings: NotRequired[Dict[LanguageCodeType, LanguageIdSettingsTypeDef]],  # (14)
    ToxicityDetection: NotRequired[List[ToxicityDetectionSettingsTypeDef]],  # (15)
```

1. See [:material-code-brackets: TranscriptionJobStatusType](./literals.md#transcriptionjobstatustype) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
3. See [:material-code-brackets: MediaFormatType](./literals.md#mediaformattype) 
4. See [:material-code-braces: MediaTypeDef](./type_defs.md#mediatypedef) 
5. See [:material-code-braces: TranscriptTypeDef](./type_defs.md#transcripttypedef) 
6. See [:material-code-braces: SettingsTypeDef](./type_defs.md#settingstypedef) 
7. See [:material-code-braces: ModelSettingsTypeDef](./type_defs.md#modelsettingstypedef) 
8. See [:material-code-braces: JobExecutionSettingsTypeDef](./type_defs.md#jobexecutionsettingstypedef) 
9. See [:material-code-braces: ContentRedactionTypeDef](./type_defs.md#contentredactiontypedef) 
10. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
11. See [:material-code-braces: LanguageCodeItemTypeDef](./type_defs.md#languagecodeitemtypedef) 
12. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
13. See [:material-code-braces: SubtitlesOutputTypeDef](./type_defs.md#subtitlesoutputtypedef) 
14. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) [:material-code-braces: LanguageIdSettingsTypeDef](./type_defs.md#languageidsettingstypedef) 
15. See [:material-code-braces: ToxicityDetectionSettingsTypeDef](./type_defs.md#toxicitydetectionsettingstypedef) 
## CallAnalyticsJobTypeDef

```python
# CallAnalyticsJobTypeDef definition

class CallAnalyticsJobTypeDef(TypedDict):
    CallAnalyticsJobName: NotRequired[str],
    CallAnalyticsJobStatus: NotRequired[CallAnalyticsJobStatusType],  # (1)
    LanguageCode: NotRequired[LanguageCodeType],  # (2)
    MediaSampleRateHertz: NotRequired[int],
    MediaFormat: NotRequired[MediaFormatType],  # (3)
    Media: NotRequired[MediaTypeDef],  # (4)
    Transcript: NotRequired[TranscriptTypeDef],  # (5)
    StartTime: NotRequired[datetime],
    CreationTime: NotRequired[datetime],
    CompletionTime: NotRequired[datetime],
    FailureReason: NotRequired[str],
    DataAccessRoleArn: NotRequired[str],
    IdentifiedLanguageScore: NotRequired[float],
    Settings: NotRequired[CallAnalyticsJobSettingsTypeDef],  # (6)
    ChannelDefinitions: NotRequired[List[ChannelDefinitionTypeDef]],  # (7)
```

1. See [:material-code-brackets: CallAnalyticsJobStatusType](./literals.md#callanalyticsjobstatustype) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
3. See [:material-code-brackets: MediaFormatType](./literals.md#mediaformattype) 
4. See [:material-code-braces: MediaTypeDef](./type_defs.md#mediatypedef) 
5. See [:material-code-braces: TranscriptTypeDef](./type_defs.md#transcripttypedef) 
6. See [:material-code-braces: CallAnalyticsJobSettingsTypeDef](./type_defs.md#callanalyticsjobsettingstypedef) 
7. See [:material-code-braces: ChannelDefinitionTypeDef](./type_defs.md#channeldefinitiontypedef) 
## StartCallAnalyticsJobRequestRequestTypeDef

```python
# StartCallAnalyticsJobRequestRequestTypeDef definition

class StartCallAnalyticsJobRequestRequestTypeDef(TypedDict):
    CallAnalyticsJobName: str,
    Media: MediaTypeDef,  # (1)
    OutputLocation: NotRequired[str],
    OutputEncryptionKMSKeyId: NotRequired[str],
    DataAccessRoleArn: NotRequired[str],
    Settings: NotRequired[CallAnalyticsJobSettingsTypeDef],  # (2)
    ChannelDefinitions: NotRequired[Sequence[ChannelDefinitionTypeDef]],  # (3)
```

1. See [:material-code-braces: MediaTypeDef](./type_defs.md#mediatypedef) 
2. See [:material-code-braces: CallAnalyticsJobSettingsTypeDef](./type_defs.md#callanalyticsjobsettingstypedef) 
3. See [:material-code-braces: ChannelDefinitionTypeDef](./type_defs.md#channeldefinitiontypedef) 
## DescribeLanguageModelResponseTypeDef

```python
# DescribeLanguageModelResponseTypeDef definition

class DescribeLanguageModelResponseTypeDef(TypedDict):
    LanguageModel: LanguageModelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LanguageModelTypeDef](./type_defs.md#languagemodeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLanguageModelsResponseTypeDef

```python
# ListLanguageModelsResponseTypeDef definition

class ListLanguageModelsResponseTypeDef(TypedDict):
    NextToken: str,
    Models: List[LanguageModelTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LanguageModelTypeDef](./type_defs.md#languagemodeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    NonTalkTimeFilter: NotRequired[NonTalkTimeFilterTypeDef],  # (1)
    InterruptionFilter: NotRequired[InterruptionFilterTypeDef],  # (2)
    TranscriptFilter: NotRequired[TranscriptFilterTypeDef],  # (3)
    SentimentFilter: NotRequired[SentimentFilterTypeDef],  # (4)
```

1. See [:material-code-braces: NonTalkTimeFilterTypeDef](./type_defs.md#nontalktimefiltertypedef) 
2. See [:material-code-braces: InterruptionFilterTypeDef](./type_defs.md#interruptionfiltertypedef) 
3. See [:material-code-braces: TranscriptFilterTypeDef](./type_defs.md#transcriptfiltertypedef) 
4. See [:material-code-braces: SentimentFilterTypeDef](./type_defs.md#sentimentfiltertypedef) 
## GetMedicalTranscriptionJobResponseTypeDef

```python
# GetMedicalTranscriptionJobResponseTypeDef definition

class GetMedicalTranscriptionJobResponseTypeDef(TypedDict):
    MedicalTranscriptionJob: MedicalTranscriptionJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MedicalTranscriptionJobTypeDef](./type_defs.md#medicaltranscriptionjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMedicalTranscriptionJobResponseTypeDef

```python
# StartMedicalTranscriptionJobResponseTypeDef definition

class StartMedicalTranscriptionJobResponseTypeDef(TypedDict):
    MedicalTranscriptionJob: MedicalTranscriptionJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MedicalTranscriptionJobTypeDef](./type_defs.md#medicaltranscriptionjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTranscriptionJobsResponseTypeDef

```python
# ListTranscriptionJobsResponseTypeDef definition

class ListTranscriptionJobsResponseTypeDef(TypedDict):
    Status: TranscriptionJobStatusType,  # (1)
    NextToken: str,
    TranscriptionJobSummaries: List[TranscriptionJobSummaryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TranscriptionJobStatusType](./literals.md#transcriptionjobstatustype) 
2. See [:material-code-braces: TranscriptionJobSummaryTypeDef](./type_defs.md#transcriptionjobsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTranscriptionJobResponseTypeDef

```python
# GetTranscriptionJobResponseTypeDef definition

class GetTranscriptionJobResponseTypeDef(TypedDict):
    TranscriptionJob: TranscriptionJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TranscriptionJobTypeDef](./type_defs.md#transcriptionjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTranscriptionJobResponseTypeDef

```python
# StartTranscriptionJobResponseTypeDef definition

class StartTranscriptionJobResponseTypeDef(TypedDict):
    TranscriptionJob: TranscriptionJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TranscriptionJobTypeDef](./type_defs.md#transcriptionjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCallAnalyticsJobResponseTypeDef

```python
# GetCallAnalyticsJobResponseTypeDef definition

class GetCallAnalyticsJobResponseTypeDef(TypedDict):
    CallAnalyticsJob: CallAnalyticsJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CallAnalyticsJobTypeDef](./type_defs.md#callanalyticsjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCallAnalyticsJobResponseTypeDef

```python
# StartCallAnalyticsJobResponseTypeDef definition

class StartCallAnalyticsJobResponseTypeDef(TypedDict):
    CallAnalyticsJob: CallAnalyticsJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CallAnalyticsJobTypeDef](./type_defs.md#callanalyticsjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CategoryPropertiesTypeDef

```python
# CategoryPropertiesTypeDef definition

class CategoryPropertiesTypeDef(TypedDict):
    CategoryName: NotRequired[str],
    Rules: NotRequired[List[RuleTypeDef]],  # (1)
    CreateTime: NotRequired[datetime],
    LastUpdateTime: NotRequired[datetime],
    InputType: NotRequired[InputTypeType],  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-brackets: InputTypeType](./literals.md#inputtypetype) 
## CreateCallAnalyticsCategoryRequestRequestTypeDef

```python
# CreateCallAnalyticsCategoryRequestRequestTypeDef definition

class CreateCallAnalyticsCategoryRequestRequestTypeDef(TypedDict):
    CategoryName: str,
    Rules: Sequence[RuleTypeDef],  # (1)
    InputType: NotRequired[InputTypeType],  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-brackets: InputTypeType](./literals.md#inputtypetype) 
## UpdateCallAnalyticsCategoryRequestRequestTypeDef

```python
# UpdateCallAnalyticsCategoryRequestRequestTypeDef definition

class UpdateCallAnalyticsCategoryRequestRequestTypeDef(TypedDict):
    CategoryName: str,
    Rules: Sequence[RuleTypeDef],  # (1)
    InputType: NotRequired[InputTypeType],  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-brackets: InputTypeType](./literals.md#inputtypetype) 
## CreateCallAnalyticsCategoryResponseTypeDef

```python
# CreateCallAnalyticsCategoryResponseTypeDef definition

class CreateCallAnalyticsCategoryResponseTypeDef(TypedDict):
    CategoryProperties: CategoryPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CategoryPropertiesTypeDef](./type_defs.md#categorypropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCallAnalyticsCategoryResponseTypeDef

```python
# GetCallAnalyticsCategoryResponseTypeDef definition

class GetCallAnalyticsCategoryResponseTypeDef(TypedDict):
    CategoryProperties: CategoryPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CategoryPropertiesTypeDef](./type_defs.md#categorypropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCallAnalyticsCategoriesResponseTypeDef

```python
# ListCallAnalyticsCategoriesResponseTypeDef definition

class ListCallAnalyticsCategoriesResponseTypeDef(TypedDict):
    NextToken: str,
    Categories: List[CategoryPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CategoryPropertiesTypeDef](./type_defs.md#categorypropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCallAnalyticsCategoryResponseTypeDef

```python
# UpdateCallAnalyticsCategoryResponseTypeDef definition

class UpdateCallAnalyticsCategoryResponseTypeDef(TypedDict):
    CategoryProperties: CategoryPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CategoryPropertiesTypeDef](./type_defs.md#categorypropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
