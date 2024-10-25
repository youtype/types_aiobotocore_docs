# Type definitions

> [Index](../README.md) > [Polly](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Polly](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
    type annotations stubs module [types-aiobotocore-polly](https://pypi.org/project/types-aiobotocore-polly/).



## DeleteLexiconInputRequestTypeDef

```python
# DeleteLexiconInputRequestTypeDef definition

class DeleteLexiconInputRequestTypeDef(TypedDict):
    Name: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeVoicesInputRequestTypeDef

```python
# DescribeVoicesInputRequestTypeDef definition

class DescribeVoicesInputRequestTypeDef(TypedDict):
    Engine: NotRequired[EngineType],  # (1)
    LanguageCode: NotRequired[LanguageCodeType],  # (2)
    IncludeAdditionalLanguageCodes: NotRequired[bool],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: EngineType](./literals.md#enginetype) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
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

## VoiceTypeDef

```python
# VoiceTypeDef definition

class VoiceTypeDef(TypedDict):
    Gender: NotRequired[GenderType],  # (1)
    Id: NotRequired[VoiceIdType],  # (2)
    LanguageCode: NotRequired[LanguageCodeType],  # (3)
    LanguageName: NotRequired[str],
    Name: NotRequired[str],
    AdditionalLanguageCodes: NotRequired[List[LanguageCodeType]],  # (4)
    SupportedEngines: NotRequired[List[EngineType]],  # (5)
```

1. See [:material-code-brackets: GenderType](./literals.md#gendertype) 
2. See [:material-code-brackets: VoiceIdType](./literals.md#voiceidtype) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
5. See [:material-code-brackets: EngineType](./literals.md#enginetype) 
## GetLexiconInputRequestTypeDef

```python
# GetLexiconInputRequestTypeDef definition

class GetLexiconInputRequestTypeDef(TypedDict):
    Name: str,
```

## LexiconAttributesTypeDef

```python
# LexiconAttributesTypeDef definition

class LexiconAttributesTypeDef(TypedDict):
    Alphabet: NotRequired[str],
    LanguageCode: NotRequired[LanguageCodeType],  # (1)
    LastModified: NotRequired[datetime],
    LexiconArn: NotRequired[str],
    LexemesCount: NotRequired[int],
    Size: NotRequired[int],
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## LexiconTypeDef

```python
# LexiconTypeDef definition

class LexiconTypeDef(TypedDict):
    Content: NotRequired[str],
    Name: NotRequired[str],
```

## GetSpeechSynthesisTaskInputRequestTypeDef

```python
# GetSpeechSynthesisTaskInputRequestTypeDef definition

class GetSpeechSynthesisTaskInputRequestTypeDef(TypedDict):
    TaskId: str,
```

## SynthesisTaskTypeDef

```python
# SynthesisTaskTypeDef definition

class SynthesisTaskTypeDef(TypedDict):
    Engine: NotRequired[EngineType],  # (1)
    TaskId: NotRequired[str],
    TaskStatus: NotRequired[TaskStatusType],  # (2)
    TaskStatusReason: NotRequired[str],
    OutputUri: NotRequired[str],
    CreationTime: NotRequired[datetime],
    RequestCharacters: NotRequired[int],
    SnsTopicArn: NotRequired[str],
    LexiconNames: NotRequired[List[str]],
    OutputFormat: NotRequired[OutputFormatType],  # (3)
    SampleRate: NotRequired[str],
    SpeechMarkTypes: NotRequired[List[SpeechMarkTypeType]],  # (4)
    TextType: NotRequired[TextTypeType],  # (5)
    VoiceId: NotRequired[VoiceIdType],  # (6)
    LanguageCode: NotRequired[LanguageCodeType],  # (7)
```

1. See [:material-code-brackets: EngineType](./literals.md#enginetype) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
4. See [:material-code-brackets: SpeechMarkTypeType](./literals.md#speechmarktypetype) 
5. See [:material-code-brackets: TextTypeType](./literals.md#texttypetype) 
6. See [:material-code-brackets: VoiceIdType](./literals.md#voiceidtype) 
7. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## ListLexiconsInputRequestTypeDef

```python
# ListLexiconsInputRequestTypeDef definition

class ListLexiconsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## ListSpeechSynthesisTasksInputRequestTypeDef

```python
# ListSpeechSynthesisTasksInputRequestTypeDef definition

class ListSpeechSynthesisTasksInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Status: NotRequired[TaskStatusType],  # (1)
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
## PutLexiconInputRequestTypeDef

```python
# PutLexiconInputRequestTypeDef definition

class PutLexiconInputRequestTypeDef(TypedDict):
    Name: str,
    Content: str,
```

## StartSpeechSynthesisTaskInputRequestTypeDef

```python
# StartSpeechSynthesisTaskInputRequestTypeDef definition

class StartSpeechSynthesisTaskInputRequestTypeDef(TypedDict):
    OutputFormat: OutputFormatType,  # (1)
    OutputS3BucketName: str,
    Text: str,
    VoiceId: VoiceIdType,  # (2)
    Engine: NotRequired[EngineType],  # (3)
    LanguageCode: NotRequired[LanguageCodeType],  # (4)
    LexiconNames: NotRequired[Sequence[str]],
    OutputS3KeyPrefix: NotRequired[str],
    SampleRate: NotRequired[str],
    SnsTopicArn: NotRequired[str],
    SpeechMarkTypes: NotRequired[Sequence[SpeechMarkTypeType]],  # (5)
    TextType: NotRequired[TextTypeType],  # (6)
```

1. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
2. See [:material-code-brackets: VoiceIdType](./literals.md#voiceidtype) 
3. See [:material-code-brackets: EngineType](./literals.md#enginetype) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
5. See [:material-code-brackets: SpeechMarkTypeType](./literals.md#speechmarktypetype) 
6. See [:material-code-brackets: TextTypeType](./literals.md#texttypetype) 
## SynthesizeSpeechInputRequestTypeDef

```python
# SynthesizeSpeechInputRequestTypeDef definition

class SynthesizeSpeechInputRequestTypeDef(TypedDict):
    OutputFormat: OutputFormatType,  # (1)
    Text: str,
    VoiceId: VoiceIdType,  # (2)
    Engine: NotRequired[EngineType],  # (3)
    LanguageCode: NotRequired[LanguageCodeType],  # (4)
    LexiconNames: NotRequired[Sequence[str]],
    SampleRate: NotRequired[str],
    SpeechMarkTypes: NotRequired[Sequence[SpeechMarkTypeType]],  # (5)
    TextType: NotRequired[TextTypeType],  # (6)
```

1. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
2. See [:material-code-brackets: VoiceIdType](./literals.md#voiceidtype) 
3. See [:material-code-brackets: EngineType](./literals.md#enginetype) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
5. See [:material-code-brackets: SpeechMarkTypeType](./literals.md#speechmarktypetype) 
6. See [:material-code-brackets: TextTypeType](./literals.md#texttypetype) 
## DescribeVoicesInputDescribeVoicesPaginateTypeDef

```python
# DescribeVoicesInputDescribeVoicesPaginateTypeDef definition

class DescribeVoicesInputDescribeVoicesPaginateTypeDef(TypedDict):
    Engine: NotRequired[EngineType],  # (1)
    LanguageCode: NotRequired[LanguageCodeType],  # (2)
    IncludeAdditionalLanguageCodes: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: EngineType](./literals.md#enginetype) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLexiconsInputListLexiconsPaginateTypeDef

```python
# ListLexiconsInputListLexiconsPaginateTypeDef definition

class ListLexiconsInputListLexiconsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef

```python
# ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef definition

class ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef(TypedDict):
    Status: NotRequired[TaskStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SynthesizeSpeechOutputTypeDef

```python
# SynthesizeSpeechOutputTypeDef definition

class SynthesizeSpeechOutputTypeDef(TypedDict):
    AudioStream: StreamingBody,
    ContentType: str,
    RequestCharacters: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVoicesOutputTypeDef

```python
# DescribeVoicesOutputTypeDef definition

class DescribeVoicesOutputTypeDef(TypedDict):
    Voices: List[VoiceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VoiceTypeDef](./type_defs.md#voicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LexiconDescriptionTypeDef

```python
# LexiconDescriptionTypeDef definition

class LexiconDescriptionTypeDef(TypedDict):
    Name: NotRequired[str],
    Attributes: NotRequired[LexiconAttributesTypeDef],  # (1)
```

1. See [:material-code-braces: LexiconAttributesTypeDef](./type_defs.md#lexiconattributestypedef) 
## GetLexiconOutputTypeDef

```python
# GetLexiconOutputTypeDef definition

class GetLexiconOutputTypeDef(TypedDict):
    Lexicon: LexiconTypeDef,  # (1)
    LexiconAttributes: LexiconAttributesTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: LexiconTypeDef](./type_defs.md#lexicontypedef) 
2. See [:material-code-braces: LexiconAttributesTypeDef](./type_defs.md#lexiconattributestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSpeechSynthesisTaskOutputTypeDef

```python
# GetSpeechSynthesisTaskOutputTypeDef definition

class GetSpeechSynthesisTaskOutputTypeDef(TypedDict):
    SynthesisTask: SynthesisTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SynthesisTaskTypeDef](./type_defs.md#synthesistasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSpeechSynthesisTasksOutputTypeDef

```python
# ListSpeechSynthesisTasksOutputTypeDef definition

class ListSpeechSynthesisTasksOutputTypeDef(TypedDict):
    SynthesisTasks: List[SynthesisTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SynthesisTaskTypeDef](./type_defs.md#synthesistasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSpeechSynthesisTaskOutputTypeDef

```python
# StartSpeechSynthesisTaskOutputTypeDef definition

class StartSpeechSynthesisTaskOutputTypeDef(TypedDict):
    SynthesisTask: SynthesisTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SynthesisTaskTypeDef](./type_defs.md#synthesistasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLexiconsOutputTypeDef

```python
# ListLexiconsOutputTypeDef definition

class ListLexiconsOutputTypeDef(TypedDict):
    Lexicons: List[LexiconDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LexiconDescriptionTypeDef](./type_defs.md#lexicondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
