# Type definitions

> [Index](../README.md) > [Comprehend](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Comprehend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
    type annotations stubs module [types-aiobotocore-comprehend](https://pypi.org/project/types-aiobotocore-comprehend/).

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


## AugmentedManifestsListItemUnionTypeDef

```python
# AugmentedManifestsListItemUnionTypeDef definition

AugmentedManifestsListItemUnionTypeDef = Union[
    AugmentedManifestsListItemTypeDef,  # (1)
    AugmentedManifestsListItemOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AugmentedManifestsListItemTypeDef](./type_defs.md#augmentedmanifestslistitemtypedef) 
2. See [:material-code-braces: AugmentedManifestsListItemOutputTypeDef](./type_defs.md#augmentedmanifestslistitemoutputtypedef) 

## VpcConfigUnionTypeDef

```python
# VpcConfigUnionTypeDef definition

VpcConfigUnionTypeDef = Union[
    VpcConfigTypeDef,  # (1)
    VpcConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
2. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 

## DocumentClassificationConfigUnionTypeDef

```python
# DocumentClassificationConfigUnionTypeDef definition

DocumentClassificationConfigUnionTypeDef = Union[
    DocumentClassificationConfigTypeDef,  # (1)
    DocumentClassificationConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentClassificationConfigTypeDef](./type_defs.md#documentclassificationconfigtypedef) 
2. See [:material-code-braces: DocumentClassificationConfigOutputTypeDef](./type_defs.md#documentclassificationconfigoutputtypedef) 

## DocumentReaderConfigUnionTypeDef

```python
# DocumentReaderConfigUnionTypeDef definition

DocumentReaderConfigUnionTypeDef = Union[
    DocumentReaderConfigTypeDef,  # (1)
    DocumentReaderConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentReaderConfigTypeDef](./type_defs.md#documentreaderconfigtypedef) 
2. See [:material-code-braces: DocumentReaderConfigOutputTypeDef](./type_defs.md#documentreaderconfigoutputtypedef) 

## EntityRecognitionConfigUnionTypeDef

```python
# EntityRecognitionConfigUnionTypeDef definition

EntityRecognitionConfigUnionTypeDef = Union[
    EntityRecognitionConfigTypeDef,  # (1)
    EntityRecognitionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EntityRecognitionConfigTypeDef](./type_defs.md#entityrecognitionconfigtypedef) 
2. See [:material-code-braces: EntityRecognitionConfigOutputTypeDef](./type_defs.md#entityrecognitionconfigoutputtypedef) 



## AugmentedManifestsListItemOutputTypeDef

```python
# AugmentedManifestsListItemOutputTypeDef definition

class AugmentedManifestsListItemOutputTypeDef(TypedDict):
    S3Uri: str,
    AttributeNames: List[str],
    Split: NotRequired[SplitType],  # (1)
    AnnotationDataS3Uri: NotRequired[str],
    SourceDocumentsS3Uri: NotRequired[str],
    DocumentType: NotRequired[AugmentedManifestsDocumentTypeFormatType],  # (2)
```

1. See [:material-code-brackets: SplitType](./literals.md#splittype) 
2. See [:material-code-brackets: AugmentedManifestsDocumentTypeFormatType](./literals.md#augmentedmanifestsdocumenttypeformattype) 
## AugmentedManifestsListItemTypeDef

```python
# AugmentedManifestsListItemTypeDef definition

class AugmentedManifestsListItemTypeDef(TypedDict):
    S3Uri: str,
    AttributeNames: Sequence[str],
    Split: NotRequired[SplitType],  # (1)
    AnnotationDataS3Uri: NotRequired[str],
    SourceDocumentsS3Uri: NotRequired[str],
    DocumentType: NotRequired[AugmentedManifestsDocumentTypeFormatType],  # (2)
```

1. See [:material-code-brackets: SplitType](./literals.md#splittype) 
2. See [:material-code-brackets: AugmentedManifestsDocumentTypeFormatType](./literals.md#augmentedmanifestsdocumenttypeformattype) 
## DominantLanguageTypeDef

```python
# DominantLanguageTypeDef definition

class DominantLanguageTypeDef(TypedDict):
    LanguageCode: NotRequired[str],
    Score: NotRequired[float],
```

## BatchDetectDominantLanguageRequestRequestTypeDef

```python
# BatchDetectDominantLanguageRequestRequestTypeDef definition

class BatchDetectDominantLanguageRequestRequestTypeDef(TypedDict):
    TextList: Sequence[str],
```

## BatchItemErrorTypeDef

```python
# BatchItemErrorTypeDef definition

class BatchItemErrorTypeDef(TypedDict):
    Index: NotRequired[int],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
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

## BatchDetectEntitiesRequestRequestTypeDef

```python
# BatchDetectEntitiesRequestRequestTypeDef definition

class BatchDetectEntitiesRequestRequestTypeDef(TypedDict):
    TextList: Sequence[str],
    LanguageCode: LanguageCodeType,  # (1)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## KeyPhraseTypeDef

```python
# KeyPhraseTypeDef definition

class KeyPhraseTypeDef(TypedDict):
    Score: NotRequired[float],
    Text: NotRequired[str],
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
```

## BatchDetectKeyPhrasesRequestRequestTypeDef

```python
# BatchDetectKeyPhrasesRequestRequestTypeDef definition

class BatchDetectKeyPhrasesRequestRequestTypeDef(TypedDict):
    TextList: Sequence[str],
    LanguageCode: LanguageCodeType,  # (1)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## SentimentScoreTypeDef

```python
# SentimentScoreTypeDef definition

class SentimentScoreTypeDef(TypedDict):
    Positive: NotRequired[float],
    Negative: NotRequired[float],
    Neutral: NotRequired[float],
    Mixed: NotRequired[float],
```

## BatchDetectSentimentRequestRequestTypeDef

```python
# BatchDetectSentimentRequestRequestTypeDef definition

class BatchDetectSentimentRequestRequestTypeDef(TypedDict):
    TextList: Sequence[str],
    LanguageCode: LanguageCodeType,  # (1)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## BatchDetectSyntaxRequestRequestTypeDef

```python
# BatchDetectSyntaxRequestRequestTypeDef definition

class BatchDetectSyntaxRequestRequestTypeDef(TypedDict):
    TextList: Sequence[str],
    LanguageCode: SyntaxLanguageCodeType,  # (1)
```

1. See [:material-code-brackets: SyntaxLanguageCodeType](./literals.md#syntaxlanguagecodetype) 
## BatchDetectTargetedSentimentRequestRequestTypeDef

```python
# BatchDetectTargetedSentimentRequestRequestTypeDef definition

class BatchDetectTargetedSentimentRequestRequestTypeDef(TypedDict):
    TextList: Sequence[str],
    LanguageCode: LanguageCodeType,  # (1)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## ChildBlockTypeDef

```python
# ChildBlockTypeDef definition

class ChildBlockTypeDef(TypedDict):
    ChildBlockId: NotRequired[str],
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
```

## RelationshipsListItemTypeDef

```python
# RelationshipsListItemTypeDef definition

class RelationshipsListItemTypeDef(TypedDict):
    Ids: NotRequired[List[str]],
    Type: NotRequired[RelationshipTypeType],  # (1)
```

1. See [:material-code-brackets: RelationshipTypeType](./literals.md#relationshiptypetype) 
## BoundingBoxTypeDef

```python
# BoundingBoxTypeDef definition

class BoundingBoxTypeDef(TypedDict):
    Height: NotRequired[float],
    Left: NotRequired[float],
    Top: NotRequired[float],
    Width: NotRequired[float],
```

## ClassifierEvaluationMetricsTypeDef

```python
# ClassifierEvaluationMetricsTypeDef definition

class ClassifierEvaluationMetricsTypeDef(TypedDict):
    Accuracy: NotRequired[float],
    Precision: NotRequired[float],
    Recall: NotRequired[float],
    F1Score: NotRequired[float],
    MicroPrecision: NotRequired[float],
    MicroRecall: NotRequired[float],
    MicroF1Score: NotRequired[float],
    HammingLoss: NotRequired[float],
```

## DocumentReaderConfigTypeDef

```python
# DocumentReaderConfigTypeDef definition

class DocumentReaderConfigTypeDef(TypedDict):
    DocumentReadAction: DocumentReadActionType,  # (1)
    DocumentReadMode: NotRequired[DocumentReadModeType],  # (2)
    FeatureTypes: NotRequired[Sequence[DocumentReadFeatureTypesType]],  # (3)
```

1. See [:material-code-brackets: DocumentReadActionType](./literals.md#documentreadactiontype) 
2. See [:material-code-brackets: DocumentReadModeType](./literals.md#documentreadmodetype) 
3. See [:material-code-brackets: DocumentReadFeatureTypesType](./literals.md#documentreadfeaturetypestype) 
## DocumentClassTypeDef

```python
# DocumentClassTypeDef definition

class DocumentClassTypeDef(TypedDict):
    Name: NotRequired[str],
    Score: NotRequired[float],
    Page: NotRequired[int],
```

## DocumentLabelTypeDef

```python
# DocumentLabelTypeDef definition

class DocumentLabelTypeDef(TypedDict):
    Name: NotRequired[str],
    Score: NotRequired[float],
    Page: NotRequired[int],
```

## DocumentTypeListItemTypeDef

```python
# DocumentTypeListItemTypeDef definition

class DocumentTypeListItemTypeDef(TypedDict):
    Page: NotRequired[int],
    Type: NotRequired[DocumentTypeType],  # (1)
```

1. See [:material-code-brackets: DocumentTypeType](./literals.md#documenttypetype) 
## ErrorsListItemTypeDef

```python
# ErrorsListItemTypeDef definition

class ErrorsListItemTypeDef(TypedDict):
    Page: NotRequired[int],
    ErrorCode: NotRequired[PageBasedErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: PageBasedErrorCodeType](./literals.md#pagebasederrorcodetype) 
## WarningsListItemTypeDef

```python
# WarningsListItemTypeDef definition

class WarningsListItemTypeDef(TypedDict):
    Page: NotRequired[int],
    WarnCode: NotRequired[PageBasedWarningCodeType],  # (1)
    WarnMessage: NotRequired[str],
```

1. See [:material-code-brackets: PageBasedWarningCodeType](./literals.md#pagebasedwarningcodetype) 
## ContainsPiiEntitiesRequestRequestTypeDef

```python
# ContainsPiiEntitiesRequestRequestTypeDef definition

class ContainsPiiEntitiesRequestRequestTypeDef(TypedDict):
    Text: str,
    LanguageCode: LanguageCodeType,  # (1)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## EntityLabelTypeDef

```python
# EntityLabelTypeDef definition

class EntityLabelTypeDef(TypedDict):
    Name: NotRequired[PiiEntityTypeType],  # (1)
    Score: NotRequired[float],
```

1. See [:material-code-brackets: PiiEntityTypeType](./literals.md#piientitytypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

## DocumentClassifierOutputDataConfigTypeDef

```python
# DocumentClassifierOutputDataConfigTypeDef definition

class DocumentClassifierOutputDataConfigTypeDef(TypedDict):
    S3Uri: NotRequired[str],
    KmsKeyId: NotRequired[str],
    FlywheelStatsS3Prefix: NotRequired[str],
```

## VpcConfigTypeDef

```python
# VpcConfigTypeDef definition

class VpcConfigTypeDef(TypedDict):
    SecurityGroupIds: Sequence[str],
    Subnets: Sequence[str],
```

## VpcConfigOutputTypeDef

```python
# VpcConfigOutputTypeDef definition

class VpcConfigOutputTypeDef(TypedDict):
    SecurityGroupIds: List[str],
    Subnets: List[str],
```

## DatasetAugmentedManifestsListItemTypeDef

```python
# DatasetAugmentedManifestsListItemTypeDef definition

class DatasetAugmentedManifestsListItemTypeDef(TypedDict):
    AttributeNames: Sequence[str],
    S3Uri: str,
    AnnotationDataS3Uri: NotRequired[str],
    SourceDocumentsS3Uri: NotRequired[str],
    DocumentType: NotRequired[AugmentedManifestsDocumentTypeFormatType],  # (1)
```

1. See [:material-code-brackets: AugmentedManifestsDocumentTypeFormatType](./literals.md#augmentedmanifestsdocumenttypeformattype) 
## DatasetDocumentClassifierInputDataConfigTypeDef

```python
# DatasetDocumentClassifierInputDataConfigTypeDef definition

class DatasetDocumentClassifierInputDataConfigTypeDef(TypedDict):
    S3Uri: str,
    LabelDelimiter: NotRequired[str],
```

## DatasetEntityRecognizerAnnotationsTypeDef

```python
# DatasetEntityRecognizerAnnotationsTypeDef definition

class DatasetEntityRecognizerAnnotationsTypeDef(TypedDict):
    S3Uri: str,
```

## DatasetEntityRecognizerDocumentsTypeDef

```python
# DatasetEntityRecognizerDocumentsTypeDef definition

class DatasetEntityRecognizerDocumentsTypeDef(TypedDict):
    S3Uri: str,
    InputFormat: NotRequired[InputFormatType],  # (1)
```

1. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
## DatasetEntityRecognizerEntityListTypeDef

```python
# DatasetEntityRecognizerEntityListTypeDef definition

class DatasetEntityRecognizerEntityListTypeDef(TypedDict):
    S3Uri: str,
```

## DatasetPropertiesTypeDef

```python
# DatasetPropertiesTypeDef definition

class DatasetPropertiesTypeDef(TypedDict):
    DatasetArn: NotRequired[str],
    DatasetName: NotRequired[str],
    DatasetType: NotRequired[DatasetTypeType],  # (1)
    DatasetS3Uri: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[DatasetStatusType],  # (2)
    Message: NotRequired[str],
    NumberOfDocuments: NotRequired[int],
    CreationTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DatasetTypeType](./literals.md#datasettypetype) 
2. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
## DeleteDocumentClassifierRequestRequestTypeDef

```python
# DeleteDocumentClassifierRequestRequestTypeDef definition

class DeleteDocumentClassifierRequestRequestTypeDef(TypedDict):
    DocumentClassifierArn: str,
```

## DeleteEndpointRequestRequestTypeDef

```python
# DeleteEndpointRequestRequestTypeDef definition

class DeleteEndpointRequestRequestTypeDef(TypedDict):
    EndpointArn: str,
```

## DeleteEntityRecognizerRequestRequestTypeDef

```python
# DeleteEntityRecognizerRequestRequestTypeDef definition

class DeleteEntityRecognizerRequestRequestTypeDef(TypedDict):
    EntityRecognizerArn: str,
```

## DeleteFlywheelRequestRequestTypeDef

```python
# DeleteFlywheelRequestRequestTypeDef definition

class DeleteFlywheelRequestRequestTypeDef(TypedDict):
    FlywheelArn: str,
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    PolicyRevisionId: NotRequired[str],
```

## DescribeDatasetRequestRequestTypeDef

```python
# DescribeDatasetRequestRequestTypeDef definition

class DescribeDatasetRequestRequestTypeDef(TypedDict):
    DatasetArn: str,
```

## DescribeDocumentClassificationJobRequestRequestTypeDef

```python
# DescribeDocumentClassificationJobRequestRequestTypeDef definition

class DescribeDocumentClassificationJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribeDocumentClassifierRequestRequestTypeDef

```python
# DescribeDocumentClassifierRequestRequestTypeDef definition

class DescribeDocumentClassifierRequestRequestTypeDef(TypedDict):
    DocumentClassifierArn: str,
```

## DescribeDominantLanguageDetectionJobRequestRequestTypeDef

```python
# DescribeDominantLanguageDetectionJobRequestRequestTypeDef definition

class DescribeDominantLanguageDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribeEndpointRequestRequestTypeDef

```python
# DescribeEndpointRequestRequestTypeDef definition

class DescribeEndpointRequestRequestTypeDef(TypedDict):
    EndpointArn: str,
```

## EndpointPropertiesTypeDef

```python
# EndpointPropertiesTypeDef definition

class EndpointPropertiesTypeDef(TypedDict):
    EndpointArn: NotRequired[str],
    Status: NotRequired[EndpointStatusType],  # (1)
    Message: NotRequired[str],
    ModelArn: NotRequired[str],
    DesiredModelArn: NotRequired[str],
    DesiredInferenceUnits: NotRequired[int],
    CurrentInferenceUnits: NotRequired[int],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    DataAccessRoleArn: NotRequired[str],
    DesiredDataAccessRoleArn: NotRequired[str],
    FlywheelArn: NotRequired[str],
```

1. See [:material-code-brackets: EndpointStatusType](./literals.md#endpointstatustype) 
## DescribeEntitiesDetectionJobRequestRequestTypeDef

```python
# DescribeEntitiesDetectionJobRequestRequestTypeDef definition

class DescribeEntitiesDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribeEntityRecognizerRequestRequestTypeDef

```python
# DescribeEntityRecognizerRequestRequestTypeDef definition

class DescribeEntityRecognizerRequestRequestTypeDef(TypedDict):
    EntityRecognizerArn: str,
```

## DescribeEventsDetectionJobRequestRequestTypeDef

```python
# DescribeEventsDetectionJobRequestRequestTypeDef definition

class DescribeEventsDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribeFlywheelIterationRequestRequestTypeDef

```python
# DescribeFlywheelIterationRequestRequestTypeDef definition

class DescribeFlywheelIterationRequestRequestTypeDef(TypedDict):
    FlywheelArn: str,
    FlywheelIterationId: str,
```

## DescribeFlywheelRequestRequestTypeDef

```python
# DescribeFlywheelRequestRequestTypeDef definition

class DescribeFlywheelRequestRequestTypeDef(TypedDict):
    FlywheelArn: str,
```

## DescribeKeyPhrasesDetectionJobRequestRequestTypeDef

```python
# DescribeKeyPhrasesDetectionJobRequestRequestTypeDef definition

class DescribeKeyPhrasesDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribePiiEntitiesDetectionJobRequestRequestTypeDef

```python
# DescribePiiEntitiesDetectionJobRequestRequestTypeDef definition

class DescribePiiEntitiesDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribeResourcePolicyRequestRequestTypeDef

```python
# DescribeResourcePolicyRequestRequestTypeDef definition

class DescribeResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DescribeSentimentDetectionJobRequestRequestTypeDef

```python
# DescribeSentimentDetectionJobRequestRequestTypeDef definition

class DescribeSentimentDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribeTargetedSentimentDetectionJobRequestRequestTypeDef

```python
# DescribeTargetedSentimentDetectionJobRequestRequestTypeDef definition

class DescribeTargetedSentimentDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribeTopicsDetectionJobRequestRequestTypeDef

```python
# DescribeTopicsDetectionJobRequestRequestTypeDef definition

class DescribeTopicsDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DetectDominantLanguageRequestRequestTypeDef

```python
# DetectDominantLanguageRequestRequestTypeDef definition

class DetectDominantLanguageRequestRequestTypeDef(TypedDict):
    Text: str,
```

## DetectKeyPhrasesRequestRequestTypeDef

```python
# DetectKeyPhrasesRequestRequestTypeDef definition

class DetectKeyPhrasesRequestRequestTypeDef(TypedDict):
    Text: str,
    LanguageCode: LanguageCodeType,  # (1)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## DetectPiiEntitiesRequestRequestTypeDef

```python
# DetectPiiEntitiesRequestRequestTypeDef definition

class DetectPiiEntitiesRequestRequestTypeDef(TypedDict):
    Text: str,
    LanguageCode: LanguageCodeType,  # (1)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## PiiEntityTypeDef

```python
# PiiEntityTypeDef definition

class PiiEntityTypeDef(TypedDict):
    Score: NotRequired[float],
    Type: NotRequired[PiiEntityTypeType],  # (1)
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
```

1. See [:material-code-brackets: PiiEntityTypeType](./literals.md#piientitytypetype) 
## DetectSentimentRequestRequestTypeDef

```python
# DetectSentimentRequestRequestTypeDef definition

class DetectSentimentRequestRequestTypeDef(TypedDict):
    Text: str,
    LanguageCode: LanguageCodeType,  # (1)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## DetectSyntaxRequestRequestTypeDef

```python
# DetectSyntaxRequestRequestTypeDef definition

class DetectSyntaxRequestRequestTypeDef(TypedDict):
    Text: str,
    LanguageCode: SyntaxLanguageCodeType,  # (1)
```

1. See [:material-code-brackets: SyntaxLanguageCodeType](./literals.md#syntaxlanguagecodetype) 
## DetectTargetedSentimentRequestRequestTypeDef

```python
# DetectTargetedSentimentRequestRequestTypeDef definition

class DetectTargetedSentimentRequestRequestTypeDef(TypedDict):
    Text: str,
    LanguageCode: LanguageCodeType,  # (1)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## TextSegmentTypeDef

```python
# TextSegmentTypeDef definition

class TextSegmentTypeDef(TypedDict):
    Text: str,
```

## DocumentClassificationConfigOutputTypeDef

```python
# DocumentClassificationConfigOutputTypeDef definition

class DocumentClassificationConfigOutputTypeDef(TypedDict):
    Mode: DocumentClassifierModeType,  # (1)
    Labels: NotRequired[List[str]],
```

1. See [:material-code-brackets: DocumentClassifierModeType](./literals.md#documentclassifiermodetype) 
## DocumentClassificationConfigTypeDef

```python
# DocumentClassificationConfigTypeDef definition

class DocumentClassificationConfigTypeDef(TypedDict):
    Mode: DocumentClassifierModeType,  # (1)
    Labels: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: DocumentClassifierModeType](./literals.md#documentclassifiermodetype) 
## OutputDataConfigTypeDef

```python
# OutputDataConfigTypeDef definition

class OutputDataConfigTypeDef(TypedDict):
    S3Uri: str,
    KmsKeyId: NotRequired[str],
```

## DocumentClassifierDocumentsTypeDef

```python
# DocumentClassifierDocumentsTypeDef definition

class DocumentClassifierDocumentsTypeDef(TypedDict):
    S3Uri: str,
    TestS3Uri: NotRequired[str],
```

## DocumentReaderConfigOutputTypeDef

```python
# DocumentReaderConfigOutputTypeDef definition

class DocumentReaderConfigOutputTypeDef(TypedDict):
    DocumentReadAction: DocumentReadActionType,  # (1)
    DocumentReadMode: NotRequired[DocumentReadModeType],  # (2)
    FeatureTypes: NotRequired[List[DocumentReadFeatureTypesType]],  # (3)
```

1. See [:material-code-brackets: DocumentReadActionType](./literals.md#documentreadactiontype) 
2. See [:material-code-brackets: DocumentReadModeType](./literals.md#documentreadmodetype) 
3. See [:material-code-brackets: DocumentReadFeatureTypesType](./literals.md#documentreadfeaturetypestype) 
## DocumentClassifierSummaryTypeDef

```python
# DocumentClassifierSummaryTypeDef definition

class DocumentClassifierSummaryTypeDef(TypedDict):
    DocumentClassifierName: NotRequired[str],
    NumberOfVersions: NotRequired[int],
    LatestVersionCreatedAt: NotRequired[datetime],
    LatestVersionName: NotRequired[str],
    LatestVersionStatus: NotRequired[ModelStatusType],  # (1)
```

1. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
## ExtractedCharactersListItemTypeDef

```python
# ExtractedCharactersListItemTypeDef definition

class ExtractedCharactersListItemTypeDef(TypedDict):
    Page: NotRequired[int],
    Count: NotRequired[int],
```

## EntityTypesListItemTypeDef

```python
# EntityTypesListItemTypeDef definition

class EntityTypesListItemTypeDef(TypedDict):
    Type: str,
```

## EntityRecognizerAnnotationsTypeDef

```python
# EntityRecognizerAnnotationsTypeDef definition

class EntityRecognizerAnnotationsTypeDef(TypedDict):
    S3Uri: str,
    TestS3Uri: NotRequired[str],
```

## EntityRecognizerDocumentsTypeDef

```python
# EntityRecognizerDocumentsTypeDef definition

class EntityRecognizerDocumentsTypeDef(TypedDict):
    S3Uri: str,
    TestS3Uri: NotRequired[str],
    InputFormat: NotRequired[InputFormatType],  # (1)
```

1. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
## EntityRecognizerEntityListTypeDef

```python
# EntityRecognizerEntityListTypeDef definition

class EntityRecognizerEntityListTypeDef(TypedDict):
    S3Uri: str,
```

## EntityRecognizerEvaluationMetricsTypeDef

```python
# EntityRecognizerEvaluationMetricsTypeDef definition

class EntityRecognizerEvaluationMetricsTypeDef(TypedDict):
    Precision: NotRequired[float],
    Recall: NotRequired[float],
    F1Score: NotRequired[float],
```

## EntityTypesEvaluationMetricsTypeDef

```python
# EntityTypesEvaluationMetricsTypeDef definition

class EntityTypesEvaluationMetricsTypeDef(TypedDict):
    Precision: NotRequired[float],
    Recall: NotRequired[float],
    F1Score: NotRequired[float],
```

## EntityRecognizerOutputDataConfigTypeDef

```python
# EntityRecognizerOutputDataConfigTypeDef definition

class EntityRecognizerOutputDataConfigTypeDef(TypedDict):
    FlywheelStatsS3Prefix: NotRequired[str],
```

## EntityRecognizerSummaryTypeDef

```python
# EntityRecognizerSummaryTypeDef definition

class EntityRecognizerSummaryTypeDef(TypedDict):
    RecognizerName: NotRequired[str],
    NumberOfVersions: NotRequired[int],
    LatestVersionCreatedAt: NotRequired[datetime],
    LatestVersionName: NotRequired[str],
    LatestVersionStatus: NotRequired[ModelStatusType],  # (1)
```

1. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
## FlywheelModelEvaluationMetricsTypeDef

```python
# FlywheelModelEvaluationMetricsTypeDef definition

class FlywheelModelEvaluationMetricsTypeDef(TypedDict):
    AverageF1Score: NotRequired[float],
    AveragePrecision: NotRequired[float],
    AverageRecall: NotRequired[float],
    AverageAccuracy: NotRequired[float],
```

## FlywheelSummaryTypeDef

```python
# FlywheelSummaryTypeDef definition

class FlywheelSummaryTypeDef(TypedDict):
    FlywheelArn: NotRequired[str],
    ActiveModelArn: NotRequired[str],
    DataLakeS3Uri: NotRequired[str],
    Status: NotRequired[FlywheelStatusType],  # (1)
    ModelType: NotRequired[ModelTypeType],  # (2)
    Message: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    LatestFlywheelIteration: NotRequired[str],
```

1. See [:material-code-brackets: FlywheelStatusType](./literals.md#flywheelstatustype) 
2. See [:material-code-brackets: ModelTypeType](./literals.md#modeltypetype) 
## PointTypeDef

```python
# PointTypeDef definition

class PointTypeDef(TypedDict):
    X: NotRequired[float],
    Y: NotRequired[float],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDocumentClassifierSummariesRequestRequestTypeDef

```python
# ListDocumentClassifierSummariesRequestRequestTypeDef definition

class ListDocumentClassifierSummariesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListEntityRecognizerSummariesRequestRequestTypeDef

```python
# ListEntityRecognizerSummariesRequestRequestTypeDef definition

class ListEntityRecognizerSummariesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## PartOfSpeechTagTypeDef

```python
# PartOfSpeechTagTypeDef definition

class PartOfSpeechTagTypeDef(TypedDict):
    Tag: NotRequired[PartOfSpeechTagTypeType],  # (1)
    Score: NotRequired[float],
```

1. See [:material-code-brackets: PartOfSpeechTagTypeType](./literals.md#partofspeechtagtypetype) 
## PiiOutputDataConfigTypeDef

```python
# PiiOutputDataConfigTypeDef definition

class PiiOutputDataConfigTypeDef(TypedDict):
    S3Uri: str,
    KmsKeyId: NotRequired[str],
```

## RedactionConfigOutputTypeDef

```python
# RedactionConfigOutputTypeDef definition

class RedactionConfigOutputTypeDef(TypedDict):
    PiiEntityTypes: NotRequired[List[PiiEntityTypeType]],  # (1)
    MaskMode: NotRequired[PiiEntitiesDetectionMaskModeType],  # (2)
    MaskCharacter: NotRequired[str],
```

1. See [:material-code-brackets: PiiEntityTypeType](./literals.md#piientitytypetype) 
2. See [:material-code-brackets: PiiEntitiesDetectionMaskModeType](./literals.md#piientitiesdetectionmaskmodetype) 
## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    ResourcePolicy: str,
    PolicyRevisionId: NotRequired[str],
```

## RedactionConfigTypeDef

```python
# RedactionConfigTypeDef definition

class RedactionConfigTypeDef(TypedDict):
    PiiEntityTypes: NotRequired[Sequence[PiiEntityTypeType]],  # (1)
    MaskMode: NotRequired[PiiEntitiesDetectionMaskModeType],  # (2)
    MaskCharacter: NotRequired[str],
```

1. See [:material-code-brackets: PiiEntityTypeType](./literals.md#piientitytypetype) 
2. See [:material-code-brackets: PiiEntitiesDetectionMaskModeType](./literals.md#piientitiesdetectionmaskmodetype) 
## StartFlywheelIterationRequestRequestTypeDef

```python
# StartFlywheelIterationRequestRequestTypeDef definition

class StartFlywheelIterationRequestRequestTypeDef(TypedDict):
    FlywheelArn: str,
    ClientRequestToken: NotRequired[str],
```

## StopDominantLanguageDetectionJobRequestRequestTypeDef

```python
# StopDominantLanguageDetectionJobRequestRequestTypeDef definition

class StopDominantLanguageDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## StopEntitiesDetectionJobRequestRequestTypeDef

```python
# StopEntitiesDetectionJobRequestRequestTypeDef definition

class StopEntitiesDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## StopEventsDetectionJobRequestRequestTypeDef

```python
# StopEventsDetectionJobRequestRequestTypeDef definition

class StopEventsDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## StopKeyPhrasesDetectionJobRequestRequestTypeDef

```python
# StopKeyPhrasesDetectionJobRequestRequestTypeDef definition

class StopKeyPhrasesDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## StopPiiEntitiesDetectionJobRequestRequestTypeDef

```python
# StopPiiEntitiesDetectionJobRequestRequestTypeDef definition

class StopPiiEntitiesDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## StopSentimentDetectionJobRequestRequestTypeDef

```python
# StopSentimentDetectionJobRequestRequestTypeDef definition

class StopSentimentDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## StopTargetedSentimentDetectionJobRequestRequestTypeDef

```python
# StopTargetedSentimentDetectionJobRequestRequestTypeDef definition

class StopTargetedSentimentDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## StopTrainingDocumentClassifierRequestRequestTypeDef

```python
# StopTrainingDocumentClassifierRequestRequestTypeDef definition

class StopTrainingDocumentClassifierRequestRequestTypeDef(TypedDict):
    DocumentClassifierArn: str,
```

## StopTrainingEntityRecognizerRequestRequestTypeDef

```python
# StopTrainingEntityRecognizerRequestRequestTypeDef definition

class StopTrainingEntityRecognizerRequestRequestTypeDef(TypedDict):
    EntityRecognizerArn: str,
```

## ToxicContentTypeDef

```python
# ToxicContentTypeDef definition

class ToxicContentTypeDef(TypedDict):
    Name: NotRequired[ToxicContentTypeType],  # (1)
    Score: NotRequired[float],
```

1. See [:material-code-brackets: ToxicContentTypeType](./literals.md#toxiccontenttypetype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateEndpointRequestRequestTypeDef

```python
# UpdateEndpointRequestRequestTypeDef definition

class UpdateEndpointRequestRequestTypeDef(TypedDict):
    EndpointArn: str,
    DesiredModelArn: NotRequired[str],
    DesiredInferenceUnits: NotRequired[int],
    DesiredDataAccessRoleArn: NotRequired[str],
    FlywheelArn: NotRequired[str],
```

## BatchDetectDominantLanguageItemResultTypeDef

```python
# BatchDetectDominantLanguageItemResultTypeDef definition

class BatchDetectDominantLanguageItemResultTypeDef(TypedDict):
    Index: NotRequired[int],
    Languages: NotRequired[List[DominantLanguageTypeDef]],  # (1)
```

1. See [:material-code-braces: DominantLanguageTypeDef](./type_defs.md#dominantlanguagetypedef) 
## CreateDatasetResponseTypeDef

```python
# CreateDatasetResponseTypeDef definition

class CreateDatasetResponseTypeDef(TypedDict):
    DatasetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDocumentClassifierResponseTypeDef

```python
# CreateDocumentClassifierResponseTypeDef definition

class CreateDocumentClassifierResponseTypeDef(TypedDict):
    DocumentClassifierArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEndpointResponseTypeDef

```python
# CreateEndpointResponseTypeDef definition

class CreateEndpointResponseTypeDef(TypedDict):
    EndpointArn: str,
    ModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEntityRecognizerResponseTypeDef

```python
# CreateEntityRecognizerResponseTypeDef definition

class CreateEntityRecognizerResponseTypeDef(TypedDict):
    EntityRecognizerArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFlywheelResponseTypeDef

```python
# CreateFlywheelResponseTypeDef definition

class CreateFlywheelResponseTypeDef(TypedDict):
    FlywheelArn: str,
    ActiveModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeResourcePolicyResponseTypeDef

```python
# DescribeResourcePolicyResponseTypeDef definition

class DescribeResourcePolicyResponseTypeDef(TypedDict):
    ResourcePolicy: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    PolicyRevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectDominantLanguageResponseTypeDef

```python
# DetectDominantLanguageResponseTypeDef definition

class DetectDominantLanguageResponseTypeDef(TypedDict):
    Languages: List[DominantLanguageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DominantLanguageTypeDef](./type_defs.md#dominantlanguagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportModelResponseTypeDef

```python
# ImportModelResponseTypeDef definition

class ImportModelResponseTypeDef(TypedDict):
    ModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyResponseTypeDef

```python
# PutResourcePolicyResponseTypeDef definition

class PutResourcePolicyResponseTypeDef(TypedDict):
    PolicyRevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDocumentClassificationJobResponseTypeDef

```python
# StartDocumentClassificationJobResponseTypeDef definition

class StartDocumentClassificationJobResponseTypeDef(TypedDict):
    JobId: str,
    JobArn: str,
    JobStatus: JobStatusType,  # (1)
    DocumentClassifierArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDominantLanguageDetectionJobResponseTypeDef

```python
# StartDominantLanguageDetectionJobResponseTypeDef definition

class StartDominantLanguageDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobArn: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartEntitiesDetectionJobResponseTypeDef

```python
# StartEntitiesDetectionJobResponseTypeDef definition

class StartEntitiesDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobArn: str,
    JobStatus: JobStatusType,  # (1)
    EntityRecognizerArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartEventsDetectionJobResponseTypeDef

```python
# StartEventsDetectionJobResponseTypeDef definition

class StartEventsDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobArn: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartFlywheelIterationResponseTypeDef

```python
# StartFlywheelIterationResponseTypeDef definition

class StartFlywheelIterationResponseTypeDef(TypedDict):
    FlywheelArn: str,
    FlywheelIterationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartKeyPhrasesDetectionJobResponseTypeDef

```python
# StartKeyPhrasesDetectionJobResponseTypeDef definition

class StartKeyPhrasesDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobArn: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartPiiEntitiesDetectionJobResponseTypeDef

```python
# StartPiiEntitiesDetectionJobResponseTypeDef definition

class StartPiiEntitiesDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobArn: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSentimentDetectionJobResponseTypeDef

```python
# StartSentimentDetectionJobResponseTypeDef definition

class StartSentimentDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobArn: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTargetedSentimentDetectionJobResponseTypeDef

```python
# StartTargetedSentimentDetectionJobResponseTypeDef definition

class StartTargetedSentimentDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobArn: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTopicsDetectionJobResponseTypeDef

```python
# StartTopicsDetectionJobResponseTypeDef definition

class StartTopicsDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobArn: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopDominantLanguageDetectionJobResponseTypeDef

```python
# StopDominantLanguageDetectionJobResponseTypeDef definition

class StopDominantLanguageDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopEntitiesDetectionJobResponseTypeDef

```python
# StopEntitiesDetectionJobResponseTypeDef definition

class StopEntitiesDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopEventsDetectionJobResponseTypeDef

```python
# StopEventsDetectionJobResponseTypeDef definition

class StopEventsDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopKeyPhrasesDetectionJobResponseTypeDef

```python
# StopKeyPhrasesDetectionJobResponseTypeDef definition

class StopKeyPhrasesDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopPiiEntitiesDetectionJobResponseTypeDef

```python
# StopPiiEntitiesDetectionJobResponseTypeDef definition

class StopPiiEntitiesDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopSentimentDetectionJobResponseTypeDef

```python
# StopSentimentDetectionJobResponseTypeDef definition

class StopSentimentDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopTargetedSentimentDetectionJobResponseTypeDef

```python
# StopTargetedSentimentDetectionJobResponseTypeDef definition

class StopTargetedSentimentDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    JobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEndpointResponseTypeDef

```python
# UpdateEndpointResponseTypeDef definition

class UpdateEndpointResponseTypeDef(TypedDict):
    DesiredModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDetectKeyPhrasesItemResultTypeDef

```python
# BatchDetectKeyPhrasesItemResultTypeDef definition

class BatchDetectKeyPhrasesItemResultTypeDef(TypedDict):
    Index: NotRequired[int],
    KeyPhrases: NotRequired[List[KeyPhraseTypeDef]],  # (1)
```

1. See [:material-code-braces: KeyPhraseTypeDef](./type_defs.md#keyphrasetypedef) 
## DetectKeyPhrasesResponseTypeDef

```python
# DetectKeyPhrasesResponseTypeDef definition

class DetectKeyPhrasesResponseTypeDef(TypedDict):
    KeyPhrases: List[KeyPhraseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyPhraseTypeDef](./type_defs.md#keyphrasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDetectSentimentItemResultTypeDef

```python
# BatchDetectSentimentItemResultTypeDef definition

class BatchDetectSentimentItemResultTypeDef(TypedDict):
    Index: NotRequired[int],
    Sentiment: NotRequired[SentimentTypeType],  # (1)
    SentimentScore: NotRequired[SentimentScoreTypeDef],  # (2)
```

1. See [:material-code-brackets: SentimentTypeType](./literals.md#sentimenttypetype) 
2. See [:material-code-braces: SentimentScoreTypeDef](./type_defs.md#sentimentscoretypedef) 
## DetectSentimentResponseTypeDef

```python
# DetectSentimentResponseTypeDef definition

class DetectSentimentResponseTypeDef(TypedDict):
    Sentiment: SentimentTypeType,  # (1)
    SentimentScore: SentimentScoreTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: SentimentTypeType](./literals.md#sentimenttypetype) 
2. See [:material-code-braces: SentimentScoreTypeDef](./type_defs.md#sentimentscoretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MentionSentimentTypeDef

```python
# MentionSentimentTypeDef definition

class MentionSentimentTypeDef(TypedDict):
    Sentiment: NotRequired[SentimentTypeType],  # (1)
    SentimentScore: NotRequired[SentimentScoreTypeDef],  # (2)
```

1. See [:material-code-brackets: SentimentTypeType](./literals.md#sentimenttypetype) 
2. See [:material-code-braces: SentimentScoreTypeDef](./type_defs.md#sentimentscoretypedef) 
## BlockReferenceTypeDef

```python
# BlockReferenceTypeDef definition

class BlockReferenceTypeDef(TypedDict):
    BlockId: NotRequired[str],
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
    ChildBlocks: NotRequired[List[ChildBlockTypeDef]],  # (1)
```

1. See [:material-code-braces: ChildBlockTypeDef](./type_defs.md#childblocktypedef) 
## ClassifierMetadataTypeDef

```python
# ClassifierMetadataTypeDef definition

class ClassifierMetadataTypeDef(TypedDict):
    NumberOfLabels: NotRequired[int],
    NumberOfTrainedDocuments: NotRequired[int],
    NumberOfTestDocuments: NotRequired[int],
    EvaluationMetrics: NotRequired[ClassifierEvaluationMetricsTypeDef],  # (1)
```

1. See [:material-code-braces: ClassifierEvaluationMetricsTypeDef](./type_defs.md#classifierevaluationmetricstypedef) 
## ClassifyDocumentRequestRequestTypeDef

```python
# ClassifyDocumentRequestRequestTypeDef definition

class ClassifyDocumentRequestRequestTypeDef(TypedDict):
    EndpointArn: str,
    Text: NotRequired[str],
    Bytes: NotRequired[BlobTypeDef],
    DocumentReaderConfig: NotRequired[DocumentReaderConfigTypeDef],  # (1)
```

1. See [:material-code-braces: DocumentReaderConfigTypeDef](./type_defs.md#documentreaderconfigtypedef) 
## DetectEntitiesRequestRequestTypeDef

```python
# DetectEntitiesRequestRequestTypeDef definition

class DetectEntitiesRequestRequestTypeDef(TypedDict):
    Text: NotRequired[str],
    LanguageCode: NotRequired[LanguageCodeType],  # (1)
    EndpointArn: NotRequired[str],
    Bytes: NotRequired[BlobTypeDef],
    DocumentReaderConfig: NotRequired[DocumentReaderConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: DocumentReaderConfigTypeDef](./type_defs.md#documentreaderconfigtypedef) 
## ContainsPiiEntitiesResponseTypeDef

```python
# ContainsPiiEntitiesResponseTypeDef definition

class ContainsPiiEntitiesResponseTypeDef(TypedDict):
    Labels: List[EntityLabelTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntityLabelTypeDef](./type_defs.md#entitylabeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEndpointRequestRequestTypeDef

```python
# CreateEndpointRequestRequestTypeDef definition

class CreateEndpointRequestRequestTypeDef(TypedDict):
    EndpointName: str,
    DesiredInferenceUnits: int,
    ModelArn: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    DataAccessRoleArn: NotRequired[str],
    FlywheelArn: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ImportModelRequestRequestTypeDef

```python
# ImportModelRequestRequestTypeDef definition

class ImportModelRequestRequestTypeDef(TypedDict):
    SourceModelArn: str,
    ModelName: NotRequired[str],
    VersionName: NotRequired[str],
    ModelKmsKeyId: NotRequired[str],
    DataAccessRoleArn: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
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
## DataSecurityConfigOutputTypeDef

```python
# DataSecurityConfigOutputTypeDef definition

class DataSecurityConfigOutputTypeDef(TypedDict):
    ModelKmsKeyId: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    DataLakeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## DatasetEntityRecognizerInputDataConfigTypeDef

```python
# DatasetEntityRecognizerInputDataConfigTypeDef definition

class DatasetEntityRecognizerInputDataConfigTypeDef(TypedDict):
    Documents: DatasetEntityRecognizerDocumentsTypeDef,  # (2)
    Annotations: NotRequired[DatasetEntityRecognizerAnnotationsTypeDef],  # (1)
    EntityList: NotRequired[DatasetEntityRecognizerEntityListTypeDef],  # (3)
```

1. See [:material-code-braces: DatasetEntityRecognizerAnnotationsTypeDef](./type_defs.md#datasetentityrecognizerannotationstypedef) 
2. See [:material-code-braces: DatasetEntityRecognizerDocumentsTypeDef](./type_defs.md#datasetentityrecognizerdocumentstypedef) 
3. See [:material-code-braces: DatasetEntityRecognizerEntityListTypeDef](./type_defs.md#datasetentityrecognizerentitylisttypedef) 
## DatasetFilterTypeDef

```python
# DatasetFilterTypeDef definition

class DatasetFilterTypeDef(TypedDict):
    Status: NotRequired[DatasetStatusType],  # (1)
    DatasetType: NotRequired[DatasetTypeType],  # (2)
    CreationTimeAfter: NotRequired[TimestampTypeDef],
    CreationTimeBefore: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
2. See [:material-code-brackets: DatasetTypeType](./literals.md#datasettypetype) 
## DocumentClassificationJobFilterTypeDef

```python
# DocumentClassificationJobFilterTypeDef definition

class DocumentClassificationJobFilterTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    SubmitTimeBefore: NotRequired[TimestampTypeDef],
    SubmitTimeAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## DocumentClassifierFilterTypeDef

```python
# DocumentClassifierFilterTypeDef definition

class DocumentClassifierFilterTypeDef(TypedDict):
    Status: NotRequired[ModelStatusType],  # (1)
    DocumentClassifierName: NotRequired[str],
    SubmitTimeBefore: NotRequired[TimestampTypeDef],
    SubmitTimeAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
## DominantLanguageDetectionJobFilterTypeDef

```python
# DominantLanguageDetectionJobFilterTypeDef definition

class DominantLanguageDetectionJobFilterTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    SubmitTimeBefore: NotRequired[TimestampTypeDef],
    SubmitTimeAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## EndpointFilterTypeDef

```python
# EndpointFilterTypeDef definition

class EndpointFilterTypeDef(TypedDict):
    ModelArn: NotRequired[str],
    Status: NotRequired[EndpointStatusType],  # (1)
    CreationTimeBefore: NotRequired[TimestampTypeDef],
    CreationTimeAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: EndpointStatusType](./literals.md#endpointstatustype) 
## EntitiesDetectionJobFilterTypeDef

```python
# EntitiesDetectionJobFilterTypeDef definition

class EntitiesDetectionJobFilterTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    SubmitTimeBefore: NotRequired[TimestampTypeDef],
    SubmitTimeAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## EntityRecognizerFilterTypeDef

```python
# EntityRecognizerFilterTypeDef definition

class EntityRecognizerFilterTypeDef(TypedDict):
    Status: NotRequired[ModelStatusType],  # (1)
    RecognizerName: NotRequired[str],
    SubmitTimeBefore: NotRequired[TimestampTypeDef],
    SubmitTimeAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
## EventsDetectionJobFilterTypeDef

```python
# EventsDetectionJobFilterTypeDef definition

class EventsDetectionJobFilterTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    SubmitTimeBefore: NotRequired[TimestampTypeDef],
    SubmitTimeAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## FlywheelFilterTypeDef

```python
# FlywheelFilterTypeDef definition

class FlywheelFilterTypeDef(TypedDict):
    Status: NotRequired[FlywheelStatusType],  # (1)
    CreationTimeAfter: NotRequired[TimestampTypeDef],
    CreationTimeBefore: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: FlywheelStatusType](./literals.md#flywheelstatustype) 
## FlywheelIterationFilterTypeDef

```python
# FlywheelIterationFilterTypeDef definition

class FlywheelIterationFilterTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[TimestampTypeDef],
    CreationTimeBefore: NotRequired[TimestampTypeDef],
```

## KeyPhrasesDetectionJobFilterTypeDef

```python
# KeyPhrasesDetectionJobFilterTypeDef definition

class KeyPhrasesDetectionJobFilterTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    SubmitTimeBefore: NotRequired[TimestampTypeDef],
    SubmitTimeAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## PiiEntitiesDetectionJobFilterTypeDef

```python
# PiiEntitiesDetectionJobFilterTypeDef definition

class PiiEntitiesDetectionJobFilterTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    SubmitTimeBefore: NotRequired[TimestampTypeDef],
    SubmitTimeAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## SentimentDetectionJobFilterTypeDef

```python
# SentimentDetectionJobFilterTypeDef definition

class SentimentDetectionJobFilterTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    SubmitTimeBefore: NotRequired[TimestampTypeDef],
    SubmitTimeAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## TargetedSentimentDetectionJobFilterTypeDef

```python
# TargetedSentimentDetectionJobFilterTypeDef definition

class TargetedSentimentDetectionJobFilterTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    SubmitTimeBefore: NotRequired[TimestampTypeDef],
    SubmitTimeAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## TopicsDetectionJobFilterTypeDef

```python
# TopicsDetectionJobFilterTypeDef definition

class TopicsDetectionJobFilterTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    SubmitTimeBefore: NotRequired[TimestampTypeDef],
    SubmitTimeAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## DescribeDatasetResponseTypeDef

```python
# DescribeDatasetResponseTypeDef definition

class DescribeDatasetResponseTypeDef(TypedDict):
    DatasetProperties: DatasetPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetPropertiesTypeDef](./type_defs.md#datasetpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatasetsResponseTypeDef

```python
# ListDatasetsResponseTypeDef definition

class ListDatasetsResponseTypeDef(TypedDict):
    DatasetPropertiesList: List[DatasetPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DatasetPropertiesTypeDef](./type_defs.md#datasetpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEndpointResponseTypeDef

```python
# DescribeEndpointResponseTypeDef definition

class DescribeEndpointResponseTypeDef(TypedDict):
    EndpointProperties: EndpointPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointPropertiesTypeDef](./type_defs.md#endpointpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEndpointsResponseTypeDef

```python
# ListEndpointsResponseTypeDef definition

class ListEndpointsResponseTypeDef(TypedDict):
    EndpointPropertiesList: List[EndpointPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EndpointPropertiesTypeDef](./type_defs.md#endpointpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectPiiEntitiesResponseTypeDef

```python
# DetectPiiEntitiesResponseTypeDef definition

class DetectPiiEntitiesResponseTypeDef(TypedDict):
    Entities: List[PiiEntityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PiiEntityTypeDef](./type_defs.md#piientitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectToxicContentRequestRequestTypeDef

```python
# DetectToxicContentRequestRequestTypeDef definition

class DetectToxicContentRequestRequestTypeDef(TypedDict):
    TextSegments: Sequence[TextSegmentTypeDef],  # (1)
    LanguageCode: LanguageCodeType,  # (2)
```

1. See [:material-code-braces: TextSegmentTypeDef](./type_defs.md#textsegmenttypedef) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## DocumentClassifierInputDataConfigOutputTypeDef

```python
# DocumentClassifierInputDataConfigOutputTypeDef definition

class DocumentClassifierInputDataConfigOutputTypeDef(TypedDict):
    DataFormat: NotRequired[DocumentClassifierDataFormatType],  # (1)
    S3Uri: NotRequired[str],
    TestS3Uri: NotRequired[str],
    LabelDelimiter: NotRequired[str],
    AugmentedManifests: NotRequired[List[AugmentedManifestsListItemOutputTypeDef]],  # (2)
    DocumentType: NotRequired[DocumentClassifierDocumentTypeFormatType],  # (3)
    Documents: NotRequired[DocumentClassifierDocumentsTypeDef],  # (4)
    DocumentReaderConfig: NotRequired[DocumentReaderConfigOutputTypeDef],  # (5)
```

1. See [:material-code-brackets: DocumentClassifierDataFormatType](./literals.md#documentclassifierdataformattype) 
2. See [:material-code-braces: AugmentedManifestsListItemOutputTypeDef](./type_defs.md#augmentedmanifestslistitemoutputtypedef) 
3. See [:material-code-brackets: DocumentClassifierDocumentTypeFormatType](./literals.md#documentclassifierdocumenttypeformattype) 
4. See [:material-code-braces: DocumentClassifierDocumentsTypeDef](./type_defs.md#documentclassifierdocumentstypedef) 
5. See [:material-code-braces: DocumentReaderConfigOutputTypeDef](./type_defs.md#documentreaderconfigoutputtypedef) 
## InputDataConfigOutputTypeDef

```python
# InputDataConfigOutputTypeDef definition

class InputDataConfigOutputTypeDef(TypedDict):
    S3Uri: str,
    InputFormat: NotRequired[InputFormatType],  # (1)
    DocumentReaderConfig: NotRequired[DocumentReaderConfigOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
2. See [:material-code-braces: DocumentReaderConfigOutputTypeDef](./type_defs.md#documentreaderconfigoutputtypedef) 
## ListDocumentClassifierSummariesResponseTypeDef

```python
# ListDocumentClassifierSummariesResponseTypeDef definition

class ListDocumentClassifierSummariesResponseTypeDef(TypedDict):
    DocumentClassifierSummariesList: List[DocumentClassifierSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentClassifierSummaryTypeDef](./type_defs.md#documentclassifiersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentMetadataTypeDef

```python
# DocumentMetadataTypeDef definition

class DocumentMetadataTypeDef(TypedDict):
    Pages: NotRequired[int],
    ExtractedCharacters: NotRequired[List[ExtractedCharactersListItemTypeDef]],  # (1)
```

1. See [:material-code-braces: ExtractedCharactersListItemTypeDef](./type_defs.md#extractedcharacterslistitemtypedef) 
## EntityRecognitionConfigOutputTypeDef

```python
# EntityRecognitionConfigOutputTypeDef definition

class EntityRecognitionConfigOutputTypeDef(TypedDict):
    EntityTypes: List[EntityTypesListItemTypeDef],  # (1)
```

1. See [:material-code-braces: EntityTypesListItemTypeDef](./type_defs.md#entitytypeslistitemtypedef) 
## EntityRecognitionConfigTypeDef

```python
# EntityRecognitionConfigTypeDef definition

class EntityRecognitionConfigTypeDef(TypedDict):
    EntityTypes: Sequence[EntityTypesListItemTypeDef],  # (1)
```

1. See [:material-code-braces: EntityTypesListItemTypeDef](./type_defs.md#entitytypeslistitemtypedef) 
## EntityRecognizerInputDataConfigOutputTypeDef

```python
# EntityRecognizerInputDataConfigOutputTypeDef definition

class EntityRecognizerInputDataConfigOutputTypeDef(TypedDict):
    EntityTypes: List[EntityTypesListItemTypeDef],  # (2)
    DataFormat: NotRequired[EntityRecognizerDataFormatType],  # (1)
    Documents: NotRequired[EntityRecognizerDocumentsTypeDef],  # (3)
    Annotations: NotRequired[EntityRecognizerAnnotationsTypeDef],  # (4)
    EntityList: NotRequired[EntityRecognizerEntityListTypeDef],  # (5)
    AugmentedManifests: NotRequired[List[AugmentedManifestsListItemOutputTypeDef]],  # (6)
```

1. See [:material-code-brackets: EntityRecognizerDataFormatType](./literals.md#entityrecognizerdataformattype) 
2. See [:material-code-braces: EntityTypesListItemTypeDef](./type_defs.md#entitytypeslistitemtypedef) 
3. See [:material-code-braces: EntityRecognizerDocumentsTypeDef](./type_defs.md#entityrecognizerdocumentstypedef) 
4. See [:material-code-braces: EntityRecognizerAnnotationsTypeDef](./type_defs.md#entityrecognizerannotationstypedef) 
5. See [:material-code-braces: EntityRecognizerEntityListTypeDef](./type_defs.md#entityrecognizerentitylisttypedef) 
6. See [:material-code-braces: AugmentedManifestsListItemOutputTypeDef](./type_defs.md#augmentedmanifestslistitemoutputtypedef) 
## EntityRecognizerMetadataEntityTypesListItemTypeDef

```python
# EntityRecognizerMetadataEntityTypesListItemTypeDef definition

class EntityRecognizerMetadataEntityTypesListItemTypeDef(TypedDict):
    Type: NotRequired[str],
    EvaluationMetrics: NotRequired[EntityTypesEvaluationMetricsTypeDef],  # (1)
    NumberOfTrainMentions: NotRequired[int],
```

1. See [:material-code-braces: EntityTypesEvaluationMetricsTypeDef](./type_defs.md#entitytypesevaluationmetricstypedef) 
## ListEntityRecognizerSummariesResponseTypeDef

```python
# ListEntityRecognizerSummariesResponseTypeDef definition

class ListEntityRecognizerSummariesResponseTypeDef(TypedDict):
    EntityRecognizerSummariesList: List[EntityRecognizerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EntityRecognizerSummaryTypeDef](./type_defs.md#entityrecognizersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FlywheelIterationPropertiesTypeDef

```python
# FlywheelIterationPropertiesTypeDef definition

class FlywheelIterationPropertiesTypeDef(TypedDict):
    FlywheelArn: NotRequired[str],
    FlywheelIterationId: NotRequired[str],
    CreationTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Status: NotRequired[FlywheelIterationStatusType],  # (1)
    Message: NotRequired[str],
    EvaluatedModelArn: NotRequired[str],
    EvaluatedModelMetrics: NotRequired[FlywheelModelEvaluationMetricsTypeDef],  # (2)
    TrainedModelArn: NotRequired[str],
    TrainedModelMetrics: NotRequired[FlywheelModelEvaluationMetricsTypeDef],  # (2)
    EvaluationManifestS3Prefix: NotRequired[str],
```

1. See [:material-code-brackets: FlywheelIterationStatusType](./literals.md#flywheeliterationstatustype) 
2. See [:material-code-braces: FlywheelModelEvaluationMetricsTypeDef](./type_defs.md#flywheelmodelevaluationmetricstypedef) 
3. See [:material-code-braces: FlywheelModelEvaluationMetricsTypeDef](./type_defs.md#flywheelmodelevaluationmetricstypedef) 
## ListFlywheelsResponseTypeDef

```python
# ListFlywheelsResponseTypeDef definition

class ListFlywheelsResponseTypeDef(TypedDict):
    FlywheelSummaryList: List[FlywheelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FlywheelSummaryTypeDef](./type_defs.md#flywheelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GeometryTypeDef

```python
# GeometryTypeDef definition

class GeometryTypeDef(TypedDict):
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (1)
    Polygon: NotRequired[List[PointTypeDef]],  # (2)
```

1. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
2. See [:material-code-braces: PointTypeDef](./type_defs.md#pointtypedef) 
## SyntaxTokenTypeDef

```python
# SyntaxTokenTypeDef definition

class SyntaxTokenTypeDef(TypedDict):
    TokenId: NotRequired[int],
    Text: NotRequired[str],
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
    PartOfSpeech: NotRequired[PartOfSpeechTagTypeDef],  # (1)
```

1. See [:material-code-braces: PartOfSpeechTagTypeDef](./type_defs.md#partofspeechtagtypedef) 
## ToxicLabelsTypeDef

```python
# ToxicLabelsTypeDef definition

class ToxicLabelsTypeDef(TypedDict):
    Labels: NotRequired[List[ToxicContentTypeDef]],  # (1)
    Toxicity: NotRequired[float],
```

1. See [:material-code-braces: ToxicContentTypeDef](./type_defs.md#toxiccontenttypedef) 
## EntityRecognizerInputDataConfigTypeDef

```python
# EntityRecognizerInputDataConfigTypeDef definition

class EntityRecognizerInputDataConfigTypeDef(TypedDict):
    EntityTypes: Sequence[EntityTypesListItemTypeDef],  # (2)
    DataFormat: NotRequired[EntityRecognizerDataFormatType],  # (1)
    Documents: NotRequired[EntityRecognizerDocumentsTypeDef],  # (3)
    Annotations: NotRequired[EntityRecognizerAnnotationsTypeDef],  # (4)
    EntityList: NotRequired[EntityRecognizerEntityListTypeDef],  # (5)
    AugmentedManifests: NotRequired[Sequence[AugmentedManifestsListItemUnionTypeDef]],  # (6)
```

1. See [:material-code-brackets: EntityRecognizerDataFormatType](./literals.md#entityrecognizerdataformattype) 
2. See [:material-code-braces: EntityTypesListItemTypeDef](./type_defs.md#entitytypeslistitemtypedef) 
3. See [:material-code-braces: EntityRecognizerDocumentsTypeDef](./type_defs.md#entityrecognizerdocumentstypedef) 
4. See [:material-code-braces: EntityRecognizerAnnotationsTypeDef](./type_defs.md#entityrecognizerannotationstypedef) 
5. See [:material-code-braces: EntityRecognizerEntityListTypeDef](./type_defs.md#entityrecognizerentitylisttypedef) 
6. See [:material-code-braces: AugmentedManifestsListItemTypeDef](./type_defs.md#augmentedmanifestslistitemtypedef) [:material-code-braces: AugmentedManifestsListItemOutputTypeDef](./type_defs.md#augmentedmanifestslistitemoutputtypedef) 
## BatchDetectDominantLanguageResponseTypeDef

```python
# BatchDetectDominantLanguageResponseTypeDef definition

class BatchDetectDominantLanguageResponseTypeDef(TypedDict):
    ResultList: List[BatchDetectDominantLanguageItemResultTypeDef],  # (1)
    ErrorList: List[BatchItemErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchDetectDominantLanguageItemResultTypeDef](./type_defs.md#batchdetectdominantlanguageitemresulttypedef) 
2. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDetectKeyPhrasesResponseTypeDef

```python
# BatchDetectKeyPhrasesResponseTypeDef definition

class BatchDetectKeyPhrasesResponseTypeDef(TypedDict):
    ResultList: List[BatchDetectKeyPhrasesItemResultTypeDef],  # (1)
    ErrorList: List[BatchItemErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchDetectKeyPhrasesItemResultTypeDef](./type_defs.md#batchdetectkeyphrasesitemresulttypedef) 
2. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDetectSentimentResponseTypeDef

```python
# BatchDetectSentimentResponseTypeDef definition

class BatchDetectSentimentResponseTypeDef(TypedDict):
    ResultList: List[BatchDetectSentimentItemResultTypeDef],  # (1)
    ErrorList: List[BatchItemErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchDetectSentimentItemResultTypeDef](./type_defs.md#batchdetectsentimentitemresulttypedef) 
2. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TargetedSentimentMentionTypeDef

```python
# TargetedSentimentMentionTypeDef definition

class TargetedSentimentMentionTypeDef(TypedDict):
    Score: NotRequired[float],
    GroupScore: NotRequired[float],
    Text: NotRequired[str],
    Type: NotRequired[TargetedSentimentEntityTypeType],  # (1)
    MentionSentiment: NotRequired[MentionSentimentTypeDef],  # (2)
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
```

1. See [:material-code-brackets: TargetedSentimentEntityTypeType](./literals.md#targetedsentimententitytypetype) 
2. See [:material-code-braces: MentionSentimentTypeDef](./type_defs.md#mentionsentimenttypedef) 
## EntityTypeDef

```python
# EntityTypeDef definition

class EntityTypeDef(TypedDict):
    Score: NotRequired[float],
    Type: NotRequired[EntityTypeType],  # (1)
    Text: NotRequired[str],
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
    BlockReferences: NotRequired[List[BlockReferenceTypeDef]],  # (2)
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-braces: BlockReferenceTypeDef](./type_defs.md#blockreferencetypedef) 
## DataSecurityConfigTypeDef

```python
# DataSecurityConfigTypeDef definition

class DataSecurityConfigTypeDef(TypedDict):
    ModelKmsKeyId: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    DataLakeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigUnionTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## UpdateDataSecurityConfigTypeDef

```python
# UpdateDataSecurityConfigTypeDef definition

class UpdateDataSecurityConfigTypeDef(TypedDict):
    ModelKmsKeyId: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigUnionTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## DatasetInputDataConfigTypeDef

```python
# DatasetInputDataConfigTypeDef definition

class DatasetInputDataConfigTypeDef(TypedDict):
    AugmentedManifests: NotRequired[Sequence[DatasetAugmentedManifestsListItemTypeDef]],  # (1)
    DataFormat: NotRequired[DatasetDataFormatType],  # (2)
    DocumentClassifierInputDataConfig: NotRequired[DatasetDocumentClassifierInputDataConfigTypeDef],  # (3)
    EntityRecognizerInputDataConfig: NotRequired[DatasetEntityRecognizerInputDataConfigTypeDef],  # (4)
```

1. See [:material-code-braces: DatasetAugmentedManifestsListItemTypeDef](./type_defs.md#datasetaugmentedmanifestslistitemtypedef) 
2. See [:material-code-brackets: DatasetDataFormatType](./literals.md#datasetdataformattype) 
3. See [:material-code-braces: DatasetDocumentClassifierInputDataConfigTypeDef](./type_defs.md#datasetdocumentclassifierinputdataconfigtypedef) 
4. See [:material-code-braces: DatasetEntityRecognizerInputDataConfigTypeDef](./type_defs.md#datasetentityrecognizerinputdataconfigtypedef) 
## ListDatasetsRequestRequestTypeDef

```python
# ListDatasetsRequestRequestTypeDef definition

class ListDatasetsRequestRequestTypeDef(TypedDict):
    FlywheelArn: NotRequired[str],
    Filter: NotRequired[DatasetFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DatasetFilterTypeDef](./type_defs.md#datasetfiltertypedef) 
## ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef

```python
# ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef definition

class ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef(TypedDict):
    Filter: NotRequired[DocumentClassificationJobFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DocumentClassificationJobFilterTypeDef](./type_defs.md#documentclassificationjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDocumentClassificationJobsRequestRequestTypeDef

```python
# ListDocumentClassificationJobsRequestRequestTypeDef definition

class ListDocumentClassificationJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[DocumentClassificationJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DocumentClassificationJobFilterTypeDef](./type_defs.md#documentclassificationjobfiltertypedef) 
## ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef

```python
# ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef definition

class ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef(TypedDict):
    Filter: NotRequired[DocumentClassifierFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DocumentClassifierFilterTypeDef](./type_defs.md#documentclassifierfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDocumentClassifiersRequestRequestTypeDef

```python
# ListDocumentClassifiersRequestRequestTypeDef definition

class ListDocumentClassifiersRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[DocumentClassifierFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DocumentClassifierFilterTypeDef](./type_defs.md#documentclassifierfiltertypedef) 
## ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef

```python
# ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef definition

class ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef(TypedDict):
    Filter: NotRequired[DominantLanguageDetectionJobFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DominantLanguageDetectionJobFilterTypeDef](./type_defs.md#dominantlanguagedetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDominantLanguageDetectionJobsRequestRequestTypeDef

```python
# ListDominantLanguageDetectionJobsRequestRequestTypeDef definition

class ListDominantLanguageDetectionJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[DominantLanguageDetectionJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DominantLanguageDetectionJobFilterTypeDef](./type_defs.md#dominantlanguagedetectionjobfiltertypedef) 
## ListEndpointsRequestListEndpointsPaginateTypeDef

```python
# ListEndpointsRequestListEndpointsPaginateTypeDef definition

class ListEndpointsRequestListEndpointsPaginateTypeDef(TypedDict):
    Filter: NotRequired[EndpointFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EndpointFilterTypeDef](./type_defs.md#endpointfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEndpointsRequestRequestTypeDef

```python
# ListEndpointsRequestRequestTypeDef definition

class ListEndpointsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[EndpointFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: EndpointFilterTypeDef](./type_defs.md#endpointfiltertypedef) 
## ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef

```python
# ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef definition

class ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef(TypedDict):
    Filter: NotRequired[EntitiesDetectionJobFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EntitiesDetectionJobFilterTypeDef](./type_defs.md#entitiesdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEntitiesDetectionJobsRequestRequestTypeDef

```python
# ListEntitiesDetectionJobsRequestRequestTypeDef definition

class ListEntitiesDetectionJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[EntitiesDetectionJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: EntitiesDetectionJobFilterTypeDef](./type_defs.md#entitiesdetectionjobfiltertypedef) 
## ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef

```python
# ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef definition

class ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef(TypedDict):
    Filter: NotRequired[EntityRecognizerFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EntityRecognizerFilterTypeDef](./type_defs.md#entityrecognizerfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEntityRecognizersRequestRequestTypeDef

```python
# ListEntityRecognizersRequestRequestTypeDef definition

class ListEntityRecognizersRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[EntityRecognizerFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: EntityRecognizerFilterTypeDef](./type_defs.md#entityrecognizerfiltertypedef) 
## ListEventsDetectionJobsRequestRequestTypeDef

```python
# ListEventsDetectionJobsRequestRequestTypeDef definition

class ListEventsDetectionJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[EventsDetectionJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: EventsDetectionJobFilterTypeDef](./type_defs.md#eventsdetectionjobfiltertypedef) 
## ListFlywheelsRequestRequestTypeDef

```python
# ListFlywheelsRequestRequestTypeDef definition

class ListFlywheelsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[FlywheelFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FlywheelFilterTypeDef](./type_defs.md#flywheelfiltertypedef) 
## ListFlywheelIterationHistoryRequestRequestTypeDef

```python
# ListFlywheelIterationHistoryRequestRequestTypeDef definition

class ListFlywheelIterationHistoryRequestRequestTypeDef(TypedDict):
    FlywheelArn: str,
    Filter: NotRequired[FlywheelIterationFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FlywheelIterationFilterTypeDef](./type_defs.md#flywheeliterationfiltertypedef) 
## ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef

```python
# ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef definition

class ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef(TypedDict):
    Filter: NotRequired[KeyPhrasesDetectionJobFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: KeyPhrasesDetectionJobFilterTypeDef](./type_defs.md#keyphrasesdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListKeyPhrasesDetectionJobsRequestRequestTypeDef

```python
# ListKeyPhrasesDetectionJobsRequestRequestTypeDef definition

class ListKeyPhrasesDetectionJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[KeyPhrasesDetectionJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: KeyPhrasesDetectionJobFilterTypeDef](./type_defs.md#keyphrasesdetectionjobfiltertypedef) 
## ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef

```python
# ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef definition

class ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef(TypedDict):
    Filter: NotRequired[PiiEntitiesDetectionJobFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PiiEntitiesDetectionJobFilterTypeDef](./type_defs.md#piientitiesdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPiiEntitiesDetectionJobsRequestRequestTypeDef

```python
# ListPiiEntitiesDetectionJobsRequestRequestTypeDef definition

class ListPiiEntitiesDetectionJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[PiiEntitiesDetectionJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: PiiEntitiesDetectionJobFilterTypeDef](./type_defs.md#piientitiesdetectionjobfiltertypedef) 
## ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef

```python
# ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef definition

class ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef(TypedDict):
    Filter: NotRequired[SentimentDetectionJobFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SentimentDetectionJobFilterTypeDef](./type_defs.md#sentimentdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSentimentDetectionJobsRequestRequestTypeDef

```python
# ListSentimentDetectionJobsRequestRequestTypeDef definition

class ListSentimentDetectionJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[SentimentDetectionJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: SentimentDetectionJobFilterTypeDef](./type_defs.md#sentimentdetectionjobfiltertypedef) 
## ListTargetedSentimentDetectionJobsRequestRequestTypeDef

```python
# ListTargetedSentimentDetectionJobsRequestRequestTypeDef definition

class ListTargetedSentimentDetectionJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[TargetedSentimentDetectionJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: TargetedSentimentDetectionJobFilterTypeDef](./type_defs.md#targetedsentimentdetectionjobfiltertypedef) 
## ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef

```python
# ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef definition

class ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef(TypedDict):
    Filter: NotRequired[TopicsDetectionJobFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TopicsDetectionJobFilterTypeDef](./type_defs.md#topicsdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTopicsDetectionJobsRequestRequestTypeDef

```python
# ListTopicsDetectionJobsRequestRequestTypeDef definition

class ListTopicsDetectionJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[TopicsDetectionJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: TopicsDetectionJobFilterTypeDef](./type_defs.md#topicsdetectionjobfiltertypedef) 
## DocumentClassifierPropertiesTypeDef

```python
# DocumentClassifierPropertiesTypeDef definition

class DocumentClassifierPropertiesTypeDef(TypedDict):
    DocumentClassifierArn: NotRequired[str],
    LanguageCode: NotRequired[LanguageCodeType],  # (1)
    Status: NotRequired[ModelStatusType],  # (2)
    Message: NotRequired[str],
    SubmitTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    TrainingStartTime: NotRequired[datetime],
    TrainingEndTime: NotRequired[datetime],
    InputDataConfig: NotRequired[DocumentClassifierInputDataConfigOutputTypeDef],  # (3)
    OutputDataConfig: NotRequired[DocumentClassifierOutputDataConfigTypeDef],  # (4)
    ClassifierMetadata: NotRequired[ClassifierMetadataTypeDef],  # (5)
    DataAccessRoleArn: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (6)
    Mode: NotRequired[DocumentClassifierModeType],  # (7)
    ModelKmsKeyId: NotRequired[str],
    VersionName: NotRequired[str],
    SourceModelArn: NotRequired[str],
    FlywheelArn: NotRequired[str],
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
3. See [:material-code-braces: DocumentClassifierInputDataConfigOutputTypeDef](./type_defs.md#documentclassifierinputdataconfigoutputtypedef) 
4. See [:material-code-braces: DocumentClassifierOutputDataConfigTypeDef](./type_defs.md#documentclassifieroutputdataconfigtypedef) 
5. See [:material-code-braces: ClassifierMetadataTypeDef](./type_defs.md#classifiermetadatatypedef) 
6. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
7. See [:material-code-brackets: DocumentClassifierModeType](./literals.md#documentclassifiermodetype) 
## DocumentClassifierInputDataConfigTypeDef

```python
# DocumentClassifierInputDataConfigTypeDef definition

class DocumentClassifierInputDataConfigTypeDef(TypedDict):
    DataFormat: NotRequired[DocumentClassifierDataFormatType],  # (1)
    S3Uri: NotRequired[str],
    TestS3Uri: NotRequired[str],
    LabelDelimiter: NotRequired[str],
    AugmentedManifests: NotRequired[Sequence[AugmentedManifestsListItemUnionTypeDef]],  # (2)
    DocumentType: NotRequired[DocumentClassifierDocumentTypeFormatType],  # (3)
    Documents: NotRequired[DocumentClassifierDocumentsTypeDef],  # (4)
    DocumentReaderConfig: NotRequired[DocumentReaderConfigUnionTypeDef],  # (5)
```

1. See [:material-code-brackets: DocumentClassifierDataFormatType](./literals.md#documentclassifierdataformattype) 
2. See [:material-code-braces: AugmentedManifestsListItemTypeDef](./type_defs.md#augmentedmanifestslistitemtypedef) [:material-code-braces: AugmentedManifestsListItemOutputTypeDef](./type_defs.md#augmentedmanifestslistitemoutputtypedef) 
3. See [:material-code-brackets: DocumentClassifierDocumentTypeFormatType](./literals.md#documentclassifierdocumenttypeformattype) 
4. See [:material-code-braces: DocumentClassifierDocumentsTypeDef](./type_defs.md#documentclassifierdocumentstypedef) 
5. See [:material-code-braces: DocumentReaderConfigTypeDef](./type_defs.md#documentreaderconfigtypedef) [:material-code-braces: DocumentReaderConfigOutputTypeDef](./type_defs.md#documentreaderconfigoutputtypedef) 
## InputDataConfigTypeDef

```python
# InputDataConfigTypeDef definition

class InputDataConfigTypeDef(TypedDict):
    S3Uri: str,
    InputFormat: NotRequired[InputFormatType],  # (1)
    DocumentReaderConfig: NotRequired[DocumentReaderConfigUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
2. See [:material-code-braces: DocumentReaderConfigTypeDef](./type_defs.md#documentreaderconfigtypedef) [:material-code-braces: DocumentReaderConfigOutputTypeDef](./type_defs.md#documentreaderconfigoutputtypedef) 
## DocumentClassificationJobPropertiesTypeDef

```python
# DocumentClassificationJobPropertiesTypeDef definition

class DocumentClassificationJobPropertiesTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobArn: NotRequired[str],
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    Message: NotRequired[str],
    SubmitTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    DocumentClassifierArn: NotRequired[str],
    InputDataConfig: NotRequired[InputDataConfigOutputTypeDef],  # (2)
    OutputDataConfig: NotRequired[OutputDataConfigTypeDef],  # (3)
    DataAccessRoleArn: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (4)
    FlywheelArn: NotRequired[str],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: InputDataConfigOutputTypeDef](./type_defs.md#inputdataconfigoutputtypedef) 
3. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
4. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## DominantLanguageDetectionJobPropertiesTypeDef

```python
# DominantLanguageDetectionJobPropertiesTypeDef definition

class DominantLanguageDetectionJobPropertiesTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobArn: NotRequired[str],
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    Message: NotRequired[str],
    SubmitTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    InputDataConfig: NotRequired[InputDataConfigOutputTypeDef],  # (2)
    OutputDataConfig: NotRequired[OutputDataConfigTypeDef],  # (3)
    DataAccessRoleArn: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (4)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: InputDataConfigOutputTypeDef](./type_defs.md#inputdataconfigoutputtypedef) 
3. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
4. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## EntitiesDetectionJobPropertiesTypeDef

```python
# EntitiesDetectionJobPropertiesTypeDef definition

class EntitiesDetectionJobPropertiesTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobArn: NotRequired[str],
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    Message: NotRequired[str],
    SubmitTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    EntityRecognizerArn: NotRequired[str],
    InputDataConfig: NotRequired[InputDataConfigOutputTypeDef],  # (2)
    OutputDataConfig: NotRequired[OutputDataConfigTypeDef],  # (3)
    LanguageCode: NotRequired[LanguageCodeType],  # (4)
    DataAccessRoleArn: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (5)
    FlywheelArn: NotRequired[str],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: InputDataConfigOutputTypeDef](./type_defs.md#inputdataconfigoutputtypedef) 
3. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
5. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## EventsDetectionJobPropertiesTypeDef

```python
# EventsDetectionJobPropertiesTypeDef definition

class EventsDetectionJobPropertiesTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobArn: NotRequired[str],
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    Message: NotRequired[str],
    SubmitTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    InputDataConfig: NotRequired[InputDataConfigOutputTypeDef],  # (2)
    OutputDataConfig: NotRequired[OutputDataConfigTypeDef],  # (3)
    LanguageCode: NotRequired[LanguageCodeType],  # (4)
    DataAccessRoleArn: NotRequired[str],
    TargetEventTypes: NotRequired[List[str]],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: InputDataConfigOutputTypeDef](./type_defs.md#inputdataconfigoutputtypedef) 
3. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## KeyPhrasesDetectionJobPropertiesTypeDef

```python
# KeyPhrasesDetectionJobPropertiesTypeDef definition

class KeyPhrasesDetectionJobPropertiesTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobArn: NotRequired[str],
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    Message: NotRequired[str],
    SubmitTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    InputDataConfig: NotRequired[InputDataConfigOutputTypeDef],  # (2)
    OutputDataConfig: NotRequired[OutputDataConfigTypeDef],  # (3)
    LanguageCode: NotRequired[LanguageCodeType],  # (4)
    DataAccessRoleArn: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (5)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: InputDataConfigOutputTypeDef](./type_defs.md#inputdataconfigoutputtypedef) 
3. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
5. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## PiiEntitiesDetectionJobPropertiesTypeDef

```python
# PiiEntitiesDetectionJobPropertiesTypeDef definition

class PiiEntitiesDetectionJobPropertiesTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobArn: NotRequired[str],
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    Message: NotRequired[str],
    SubmitTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    InputDataConfig: NotRequired[InputDataConfigOutputTypeDef],  # (2)
    OutputDataConfig: NotRequired[PiiOutputDataConfigTypeDef],  # (3)
    RedactionConfig: NotRequired[RedactionConfigOutputTypeDef],  # (4)
    LanguageCode: NotRequired[LanguageCodeType],  # (5)
    DataAccessRoleArn: NotRequired[str],
    Mode: NotRequired[PiiEntitiesDetectionModeType],  # (6)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: InputDataConfigOutputTypeDef](./type_defs.md#inputdataconfigoutputtypedef) 
3. See [:material-code-braces: PiiOutputDataConfigTypeDef](./type_defs.md#piioutputdataconfigtypedef) 
4. See [:material-code-braces: RedactionConfigOutputTypeDef](./type_defs.md#redactionconfigoutputtypedef) 
5. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
6. See [:material-code-brackets: PiiEntitiesDetectionModeType](./literals.md#piientitiesdetectionmodetype) 
## SentimentDetectionJobPropertiesTypeDef

```python
# SentimentDetectionJobPropertiesTypeDef definition

class SentimentDetectionJobPropertiesTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobArn: NotRequired[str],
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    Message: NotRequired[str],
    SubmitTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    InputDataConfig: NotRequired[InputDataConfigOutputTypeDef],  # (2)
    OutputDataConfig: NotRequired[OutputDataConfigTypeDef],  # (3)
    LanguageCode: NotRequired[LanguageCodeType],  # (4)
    DataAccessRoleArn: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (5)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: InputDataConfigOutputTypeDef](./type_defs.md#inputdataconfigoutputtypedef) 
3. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
5. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## TargetedSentimentDetectionJobPropertiesTypeDef

```python
# TargetedSentimentDetectionJobPropertiesTypeDef definition

class TargetedSentimentDetectionJobPropertiesTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobArn: NotRequired[str],
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    Message: NotRequired[str],
    SubmitTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    InputDataConfig: NotRequired[InputDataConfigOutputTypeDef],  # (2)
    OutputDataConfig: NotRequired[OutputDataConfigTypeDef],  # (3)
    LanguageCode: NotRequired[LanguageCodeType],  # (4)
    DataAccessRoleArn: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (5)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: InputDataConfigOutputTypeDef](./type_defs.md#inputdataconfigoutputtypedef) 
3. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
5. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## TopicsDetectionJobPropertiesTypeDef

```python
# TopicsDetectionJobPropertiesTypeDef definition

class TopicsDetectionJobPropertiesTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobArn: NotRequired[str],
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    Message: NotRequired[str],
    SubmitTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    InputDataConfig: NotRequired[InputDataConfigOutputTypeDef],  # (2)
    OutputDataConfig: NotRequired[OutputDataConfigTypeDef],  # (3)
    NumberOfTopics: NotRequired[int],
    DataAccessRoleArn: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (4)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: InputDataConfigOutputTypeDef](./type_defs.md#inputdataconfigoutputtypedef) 
3. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
4. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## ClassifyDocumentResponseTypeDef

```python
# ClassifyDocumentResponseTypeDef definition

class ClassifyDocumentResponseTypeDef(TypedDict):
    Classes: List[DocumentClassTypeDef],  # (1)
    Labels: List[DocumentLabelTypeDef],  # (2)
    DocumentMetadata: DocumentMetadataTypeDef,  # (3)
    DocumentType: List[DocumentTypeListItemTypeDef],  # (4)
    Errors: List[ErrorsListItemTypeDef],  # (5)
    Warnings: List[WarningsListItemTypeDef],  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: DocumentClassTypeDef](./type_defs.md#documentclasstypedef) 
2. See [:material-code-braces: DocumentLabelTypeDef](./type_defs.md#documentlabeltypedef) 
3. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
4. See [:material-code-braces: DocumentTypeListItemTypeDef](./type_defs.md#documenttypelistitemtypedef) 
5. See [:material-code-braces: ErrorsListItemTypeDef](./type_defs.md#errorslistitemtypedef) 
6. See [:material-code-braces: WarningsListItemTypeDef](./type_defs.md#warningslistitemtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TaskConfigOutputTypeDef

```python
# TaskConfigOutputTypeDef definition

class TaskConfigOutputTypeDef(TypedDict):
    LanguageCode: LanguageCodeType,  # (1)
    DocumentClassificationConfig: NotRequired[DocumentClassificationConfigOutputTypeDef],  # (2)
    EntityRecognitionConfig: NotRequired[EntityRecognitionConfigOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: DocumentClassificationConfigOutputTypeDef](./type_defs.md#documentclassificationconfigoutputtypedef) 
3. See [:material-code-braces: EntityRecognitionConfigOutputTypeDef](./type_defs.md#entityrecognitionconfigoutputtypedef) 
## EntityRecognizerMetadataTypeDef

```python
# EntityRecognizerMetadataTypeDef definition

class EntityRecognizerMetadataTypeDef(TypedDict):
    NumberOfTrainedDocuments: NotRequired[int],
    NumberOfTestDocuments: NotRequired[int],
    EvaluationMetrics: NotRequired[EntityRecognizerEvaluationMetricsTypeDef],  # (1)
    EntityTypes: NotRequired[List[EntityRecognizerMetadataEntityTypesListItemTypeDef]],  # (2)
```

1. See [:material-code-braces: EntityRecognizerEvaluationMetricsTypeDef](./type_defs.md#entityrecognizerevaluationmetricstypedef) 
2. See [:material-code-braces: EntityRecognizerMetadataEntityTypesListItemTypeDef](./type_defs.md#entityrecognizermetadataentitytypeslistitemtypedef) 
## DescribeFlywheelIterationResponseTypeDef

```python
# DescribeFlywheelIterationResponseTypeDef definition

class DescribeFlywheelIterationResponseTypeDef(TypedDict):
    FlywheelIterationProperties: FlywheelIterationPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlywheelIterationPropertiesTypeDef](./type_defs.md#flywheeliterationpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFlywheelIterationHistoryResponseTypeDef

```python
# ListFlywheelIterationHistoryResponseTypeDef definition

class ListFlywheelIterationHistoryResponseTypeDef(TypedDict):
    FlywheelIterationPropertiesList: List[FlywheelIterationPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FlywheelIterationPropertiesTypeDef](./type_defs.md#flywheeliterationpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BlockTypeDef

```python
# BlockTypeDef definition

class BlockTypeDef(TypedDict):
    Id: NotRequired[str],
    BlockType: NotRequired[BlockTypeType],  # (1)
    Text: NotRequired[str],
    Page: NotRequired[int],
    Geometry: NotRequired[GeometryTypeDef],  # (2)
    Relationships: NotRequired[List[RelationshipsListItemTypeDef]],  # (3)
```

1. See [:material-code-brackets: BlockTypeType](./literals.md#blocktypetype) 
2. See [:material-code-braces: GeometryTypeDef](./type_defs.md#geometrytypedef) 
3. See [:material-code-braces: RelationshipsListItemTypeDef](./type_defs.md#relationshipslistitemtypedef) 
## BatchDetectSyntaxItemResultTypeDef

```python
# BatchDetectSyntaxItemResultTypeDef definition

class BatchDetectSyntaxItemResultTypeDef(TypedDict):
    Index: NotRequired[int],
    SyntaxTokens: NotRequired[List[SyntaxTokenTypeDef]],  # (1)
```

1. See [:material-code-braces: SyntaxTokenTypeDef](./type_defs.md#syntaxtokentypedef) 
## DetectSyntaxResponseTypeDef

```python
# DetectSyntaxResponseTypeDef definition

class DetectSyntaxResponseTypeDef(TypedDict):
    SyntaxTokens: List[SyntaxTokenTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SyntaxTokenTypeDef](./type_defs.md#syntaxtokentypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectToxicContentResponseTypeDef

```python
# DetectToxicContentResponseTypeDef definition

class DetectToxicContentResponseTypeDef(TypedDict):
    ResultList: List[ToxicLabelsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ToxicLabelsTypeDef](./type_defs.md#toxiclabelstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEntityRecognizerRequestRequestTypeDef

```python
# CreateEntityRecognizerRequestRequestTypeDef definition

class CreateEntityRecognizerRequestRequestTypeDef(TypedDict):
    RecognizerName: str,
    DataAccessRoleArn: str,
    InputDataConfig: EntityRecognizerInputDataConfigTypeDef,  # (1)
    LanguageCode: LanguageCodeType,  # (2)
    VersionName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    ClientRequestToken: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (4)
    ModelKmsKeyId: NotRequired[str],
    ModelPolicy: NotRequired[str],
```

1. See [:material-code-braces: EntityRecognizerInputDataConfigTypeDef](./type_defs.md#entityrecognizerinputdataconfigtypedef) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
## TargetedSentimentEntityTypeDef

```python
# TargetedSentimentEntityTypeDef definition

class TargetedSentimentEntityTypeDef(TypedDict):
    DescriptiveMentionIndex: NotRequired[List[int]],
    Mentions: NotRequired[List[TargetedSentimentMentionTypeDef]],  # (1)
```

1. See [:material-code-braces: TargetedSentimentMentionTypeDef](./type_defs.md#targetedsentimentmentiontypedef) 
## BatchDetectEntitiesItemResultTypeDef

```python
# BatchDetectEntitiesItemResultTypeDef definition

class BatchDetectEntitiesItemResultTypeDef(TypedDict):
    Index: NotRequired[int],
    Entities: NotRequired[List[EntityTypeDef]],  # (1)
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
## UpdateFlywheelRequestRequestTypeDef

```python
# UpdateFlywheelRequestRequestTypeDef definition

class UpdateFlywheelRequestRequestTypeDef(TypedDict):
    FlywheelArn: str,
    ActiveModelArn: NotRequired[str],
    DataAccessRoleArn: NotRequired[str],
    DataSecurityConfig: NotRequired[UpdateDataSecurityConfigTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateDataSecurityConfigTypeDef](./type_defs.md#updatedatasecurityconfigtypedef) 
## CreateDatasetRequestRequestTypeDef

```python
# CreateDatasetRequestRequestTypeDef definition

class CreateDatasetRequestRequestTypeDef(TypedDict):
    FlywheelArn: str,
    DatasetName: str,
    InputDataConfig: DatasetInputDataConfigTypeDef,  # (1)
    DatasetType: NotRequired[DatasetTypeType],  # (2)
    Description: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: DatasetInputDataConfigTypeDef](./type_defs.md#datasetinputdataconfigtypedef) 
2. See [:material-code-brackets: DatasetTypeType](./literals.md#datasettypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeDocumentClassifierResponseTypeDef

```python
# DescribeDocumentClassifierResponseTypeDef definition

class DescribeDocumentClassifierResponseTypeDef(TypedDict):
    DocumentClassifierProperties: DocumentClassifierPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentClassifierPropertiesTypeDef](./type_defs.md#documentclassifierpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDocumentClassifiersResponseTypeDef

```python
# ListDocumentClassifiersResponseTypeDef definition

class ListDocumentClassifiersResponseTypeDef(TypedDict):
    DocumentClassifierPropertiesList: List[DocumentClassifierPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentClassifierPropertiesTypeDef](./type_defs.md#documentclassifierpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDocumentClassifierRequestRequestTypeDef

```python
# CreateDocumentClassifierRequestRequestTypeDef definition

class CreateDocumentClassifierRequestRequestTypeDef(TypedDict):
    DocumentClassifierName: str,
    DataAccessRoleArn: str,
    InputDataConfig: DocumentClassifierInputDataConfigTypeDef,  # (1)
    LanguageCode: LanguageCodeType,  # (2)
    VersionName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    OutputDataConfig: NotRequired[DocumentClassifierOutputDataConfigTypeDef],  # (4)
    ClientRequestToken: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (5)
    Mode: NotRequired[DocumentClassifierModeType],  # (6)
    ModelKmsKeyId: NotRequired[str],
    ModelPolicy: NotRequired[str],
```

1. See [:material-code-braces: DocumentClassifierInputDataConfigTypeDef](./type_defs.md#documentclassifierinputdataconfigtypedef) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: DocumentClassifierOutputDataConfigTypeDef](./type_defs.md#documentclassifieroutputdataconfigtypedef) 
5. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
6. See [:material-code-brackets: DocumentClassifierModeType](./literals.md#documentclassifiermodetype) 
## StartDocumentClassificationJobRequestRequestTypeDef

```python
# StartDocumentClassificationJobRequestRequestTypeDef definition

class StartDocumentClassificationJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    JobName: NotRequired[str],
    DocumentClassifierArn: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    FlywheelArn: NotRequired[str],
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartDominantLanguageDetectionJobRequestRequestTypeDef

```python
# StartDominantLanguageDetectionJobRequestRequestTypeDef definition

class StartDominantLanguageDetectionJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    JobName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartEntitiesDetectionJobRequestRequestTypeDef

```python
# StartEntitiesDetectionJobRequestRequestTypeDef definition

class StartEntitiesDetectionJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    JobName: NotRequired[str],
    EntityRecognizerArn: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
    FlywheelArn: NotRequired[str],
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartEventsDetectionJobRequestRequestTypeDef

```python
# StartEventsDetectionJobRequestRequestTypeDef definition

class StartEventsDetectionJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    TargetEventTypes: Sequence[str],
    JobName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartKeyPhrasesDetectionJobRequestRequestTypeDef

```python
# StartKeyPhrasesDetectionJobRequestRequestTypeDef definition

class StartKeyPhrasesDetectionJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    JobName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartPiiEntitiesDetectionJobRequestRequestTypeDef

```python
# StartPiiEntitiesDetectionJobRequestRequestTypeDef definition

class StartPiiEntitiesDetectionJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    Mode: PiiEntitiesDetectionModeType,  # (3)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (4)
    RedactionConfig: NotRequired[RedactionConfigTypeDef],  # (5)
    JobName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (6)
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: PiiEntitiesDetectionModeType](./literals.md#piientitiesdetectionmodetype) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
5. See [:material-code-braces: RedactionConfigTypeDef](./type_defs.md#redactionconfigtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartSentimentDetectionJobRequestRequestTypeDef

```python
# StartSentimentDetectionJobRequestRequestTypeDef definition

class StartSentimentDetectionJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    JobName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartTargetedSentimentDetectionJobRequestRequestTypeDef

```python
# StartTargetedSentimentDetectionJobRequestRequestTypeDef definition

class StartTargetedSentimentDetectionJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    JobName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartTopicsDetectionJobRequestRequestTypeDef

```python
# StartTopicsDetectionJobRequestRequestTypeDef definition

class StartTopicsDetectionJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    JobName: NotRequired[str],
    NumberOfTopics: NotRequired[int],
    ClientRequestToken: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeDocumentClassificationJobResponseTypeDef

```python
# DescribeDocumentClassificationJobResponseTypeDef definition

class DescribeDocumentClassificationJobResponseTypeDef(TypedDict):
    DocumentClassificationJobProperties: DocumentClassificationJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentClassificationJobPropertiesTypeDef](./type_defs.md#documentclassificationjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDocumentClassificationJobsResponseTypeDef

```python
# ListDocumentClassificationJobsResponseTypeDef definition

class ListDocumentClassificationJobsResponseTypeDef(TypedDict):
    DocumentClassificationJobPropertiesList: List[DocumentClassificationJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentClassificationJobPropertiesTypeDef](./type_defs.md#documentclassificationjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDominantLanguageDetectionJobResponseTypeDef

```python
# DescribeDominantLanguageDetectionJobResponseTypeDef definition

class DescribeDominantLanguageDetectionJobResponseTypeDef(TypedDict):
    DominantLanguageDetectionJobProperties: DominantLanguageDetectionJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DominantLanguageDetectionJobPropertiesTypeDef](./type_defs.md#dominantlanguagedetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDominantLanguageDetectionJobsResponseTypeDef

```python
# ListDominantLanguageDetectionJobsResponseTypeDef definition

class ListDominantLanguageDetectionJobsResponseTypeDef(TypedDict):
    DominantLanguageDetectionJobPropertiesList: List[DominantLanguageDetectionJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DominantLanguageDetectionJobPropertiesTypeDef](./type_defs.md#dominantlanguagedetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEntitiesDetectionJobResponseTypeDef

```python
# DescribeEntitiesDetectionJobResponseTypeDef definition

class DescribeEntitiesDetectionJobResponseTypeDef(TypedDict):
    EntitiesDetectionJobProperties: EntitiesDetectionJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntitiesDetectionJobPropertiesTypeDef](./type_defs.md#entitiesdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEntitiesDetectionJobsResponseTypeDef

```python
# ListEntitiesDetectionJobsResponseTypeDef definition

class ListEntitiesDetectionJobsResponseTypeDef(TypedDict):
    EntitiesDetectionJobPropertiesList: List[EntitiesDetectionJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EntitiesDetectionJobPropertiesTypeDef](./type_defs.md#entitiesdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEventsDetectionJobResponseTypeDef

```python
# DescribeEventsDetectionJobResponseTypeDef definition

class DescribeEventsDetectionJobResponseTypeDef(TypedDict):
    EventsDetectionJobProperties: EventsDetectionJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventsDetectionJobPropertiesTypeDef](./type_defs.md#eventsdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventsDetectionJobsResponseTypeDef

```python
# ListEventsDetectionJobsResponseTypeDef definition

class ListEventsDetectionJobsResponseTypeDef(TypedDict):
    EventsDetectionJobPropertiesList: List[EventsDetectionJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EventsDetectionJobPropertiesTypeDef](./type_defs.md#eventsdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeKeyPhrasesDetectionJobResponseTypeDef

```python
# DescribeKeyPhrasesDetectionJobResponseTypeDef definition

class DescribeKeyPhrasesDetectionJobResponseTypeDef(TypedDict):
    KeyPhrasesDetectionJobProperties: KeyPhrasesDetectionJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyPhrasesDetectionJobPropertiesTypeDef](./type_defs.md#keyphrasesdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKeyPhrasesDetectionJobsResponseTypeDef

```python
# ListKeyPhrasesDetectionJobsResponseTypeDef definition

class ListKeyPhrasesDetectionJobsResponseTypeDef(TypedDict):
    KeyPhrasesDetectionJobPropertiesList: List[KeyPhrasesDetectionJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: KeyPhrasesDetectionJobPropertiesTypeDef](./type_defs.md#keyphrasesdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePiiEntitiesDetectionJobResponseTypeDef

```python
# DescribePiiEntitiesDetectionJobResponseTypeDef definition

class DescribePiiEntitiesDetectionJobResponseTypeDef(TypedDict):
    PiiEntitiesDetectionJobProperties: PiiEntitiesDetectionJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PiiEntitiesDetectionJobPropertiesTypeDef](./type_defs.md#piientitiesdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPiiEntitiesDetectionJobsResponseTypeDef

```python
# ListPiiEntitiesDetectionJobsResponseTypeDef definition

class ListPiiEntitiesDetectionJobsResponseTypeDef(TypedDict):
    PiiEntitiesDetectionJobPropertiesList: List[PiiEntitiesDetectionJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PiiEntitiesDetectionJobPropertiesTypeDef](./type_defs.md#piientitiesdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSentimentDetectionJobResponseTypeDef

```python
# DescribeSentimentDetectionJobResponseTypeDef definition

class DescribeSentimentDetectionJobResponseTypeDef(TypedDict):
    SentimentDetectionJobProperties: SentimentDetectionJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SentimentDetectionJobPropertiesTypeDef](./type_defs.md#sentimentdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSentimentDetectionJobsResponseTypeDef

```python
# ListSentimentDetectionJobsResponseTypeDef definition

class ListSentimentDetectionJobsResponseTypeDef(TypedDict):
    SentimentDetectionJobPropertiesList: List[SentimentDetectionJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SentimentDetectionJobPropertiesTypeDef](./type_defs.md#sentimentdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTargetedSentimentDetectionJobResponseTypeDef

```python
# DescribeTargetedSentimentDetectionJobResponseTypeDef definition

class DescribeTargetedSentimentDetectionJobResponseTypeDef(TypedDict):
    TargetedSentimentDetectionJobProperties: TargetedSentimentDetectionJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetedSentimentDetectionJobPropertiesTypeDef](./type_defs.md#targetedsentimentdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTargetedSentimentDetectionJobsResponseTypeDef

```python
# ListTargetedSentimentDetectionJobsResponseTypeDef definition

class ListTargetedSentimentDetectionJobsResponseTypeDef(TypedDict):
    TargetedSentimentDetectionJobPropertiesList: List[TargetedSentimentDetectionJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TargetedSentimentDetectionJobPropertiesTypeDef](./type_defs.md#targetedsentimentdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTopicsDetectionJobResponseTypeDef

```python
# DescribeTopicsDetectionJobResponseTypeDef definition

class DescribeTopicsDetectionJobResponseTypeDef(TypedDict):
    TopicsDetectionJobProperties: TopicsDetectionJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TopicsDetectionJobPropertiesTypeDef](./type_defs.md#topicsdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTopicsDetectionJobsResponseTypeDef

```python
# ListTopicsDetectionJobsResponseTypeDef definition

class ListTopicsDetectionJobsResponseTypeDef(TypedDict):
    TopicsDetectionJobPropertiesList: List[TopicsDetectionJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TopicsDetectionJobPropertiesTypeDef](./type_defs.md#topicsdetectionjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FlywheelPropertiesTypeDef

```python
# FlywheelPropertiesTypeDef definition

class FlywheelPropertiesTypeDef(TypedDict):
    FlywheelArn: NotRequired[str],
    ActiveModelArn: NotRequired[str],
    DataAccessRoleArn: NotRequired[str],
    TaskConfig: NotRequired[TaskConfigOutputTypeDef],  # (1)
    DataLakeS3Uri: NotRequired[str],
    DataSecurityConfig: NotRequired[DataSecurityConfigOutputTypeDef],  # (2)
    Status: NotRequired[FlywheelStatusType],  # (3)
    ModelType: NotRequired[ModelTypeType],  # (4)
    Message: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    LatestFlywheelIteration: NotRequired[str],
```

1. See [:material-code-braces: TaskConfigOutputTypeDef](./type_defs.md#taskconfigoutputtypedef) 
2. See [:material-code-braces: DataSecurityConfigOutputTypeDef](./type_defs.md#datasecurityconfigoutputtypedef) 
3. See [:material-code-brackets: FlywheelStatusType](./literals.md#flywheelstatustype) 
4. See [:material-code-brackets: ModelTypeType](./literals.md#modeltypetype) 
## TaskConfigTypeDef

```python
# TaskConfigTypeDef definition

class TaskConfigTypeDef(TypedDict):
    LanguageCode: LanguageCodeType,  # (1)
    DocumentClassificationConfig: NotRequired[DocumentClassificationConfigUnionTypeDef],  # (2)
    EntityRecognitionConfig: NotRequired[EntityRecognitionConfigUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: DocumentClassificationConfigTypeDef](./type_defs.md#documentclassificationconfigtypedef) [:material-code-braces: DocumentClassificationConfigOutputTypeDef](./type_defs.md#documentclassificationconfigoutputtypedef) 
3. See [:material-code-braces: EntityRecognitionConfigTypeDef](./type_defs.md#entityrecognitionconfigtypedef) [:material-code-braces: EntityRecognitionConfigOutputTypeDef](./type_defs.md#entityrecognitionconfigoutputtypedef) 
## EntityRecognizerPropertiesTypeDef

```python
# EntityRecognizerPropertiesTypeDef definition

class EntityRecognizerPropertiesTypeDef(TypedDict):
    EntityRecognizerArn: NotRequired[str],
    LanguageCode: NotRequired[LanguageCodeType],  # (1)
    Status: NotRequired[ModelStatusType],  # (2)
    Message: NotRequired[str],
    SubmitTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    TrainingStartTime: NotRequired[datetime],
    TrainingEndTime: NotRequired[datetime],
    InputDataConfig: NotRequired[EntityRecognizerInputDataConfigOutputTypeDef],  # (3)
    RecognizerMetadata: NotRequired[EntityRecognizerMetadataTypeDef],  # (4)
    DataAccessRoleArn: NotRequired[str],
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (5)
    ModelKmsKeyId: NotRequired[str],
    VersionName: NotRequired[str],
    SourceModelArn: NotRequired[str],
    FlywheelArn: NotRequired[str],
    OutputDataConfig: NotRequired[EntityRecognizerOutputDataConfigTypeDef],  # (6)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
3. See [:material-code-braces: EntityRecognizerInputDataConfigOutputTypeDef](./type_defs.md#entityrecognizerinputdataconfigoutputtypedef) 
4. See [:material-code-braces: EntityRecognizerMetadataTypeDef](./type_defs.md#entityrecognizermetadatatypedef) 
5. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
6. See [:material-code-braces: EntityRecognizerOutputDataConfigTypeDef](./type_defs.md#entityrecognizeroutputdataconfigtypedef) 
## DetectEntitiesResponseTypeDef

```python
# DetectEntitiesResponseTypeDef definition

class DetectEntitiesResponseTypeDef(TypedDict):
    Entities: List[EntityTypeDef],  # (1)
    DocumentMetadata: DocumentMetadataTypeDef,  # (2)
    DocumentType: List[DocumentTypeListItemTypeDef],  # (3)
    Blocks: List[BlockTypeDef],  # (4)
    Errors: List[ErrorsListItemTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
2. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
3. See [:material-code-braces: DocumentTypeListItemTypeDef](./type_defs.md#documenttypelistitemtypedef) 
4. See [:material-code-braces: BlockTypeDef](./type_defs.md#blocktypedef) 
5. See [:material-code-braces: ErrorsListItemTypeDef](./type_defs.md#errorslistitemtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDetectSyntaxResponseTypeDef

```python
# BatchDetectSyntaxResponseTypeDef definition

class BatchDetectSyntaxResponseTypeDef(TypedDict):
    ResultList: List[BatchDetectSyntaxItemResultTypeDef],  # (1)
    ErrorList: List[BatchItemErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchDetectSyntaxItemResultTypeDef](./type_defs.md#batchdetectsyntaxitemresulttypedef) 
2. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDetectTargetedSentimentItemResultTypeDef

```python
# BatchDetectTargetedSentimentItemResultTypeDef definition

class BatchDetectTargetedSentimentItemResultTypeDef(TypedDict):
    Index: NotRequired[int],
    Entities: NotRequired[List[TargetedSentimentEntityTypeDef]],  # (1)
```

1. See [:material-code-braces: TargetedSentimentEntityTypeDef](./type_defs.md#targetedsentimententitytypedef) 
## DetectTargetedSentimentResponseTypeDef

```python
# DetectTargetedSentimentResponseTypeDef definition

class DetectTargetedSentimentResponseTypeDef(TypedDict):
    Entities: List[TargetedSentimentEntityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetedSentimentEntityTypeDef](./type_defs.md#targetedsentimententitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDetectEntitiesResponseTypeDef

```python
# BatchDetectEntitiesResponseTypeDef definition

class BatchDetectEntitiesResponseTypeDef(TypedDict):
    ResultList: List[BatchDetectEntitiesItemResultTypeDef],  # (1)
    ErrorList: List[BatchItemErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchDetectEntitiesItemResultTypeDef](./type_defs.md#batchdetectentitiesitemresulttypedef) 
2. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFlywheelResponseTypeDef

```python
# DescribeFlywheelResponseTypeDef definition

class DescribeFlywheelResponseTypeDef(TypedDict):
    FlywheelProperties: FlywheelPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlywheelPropertiesTypeDef](./type_defs.md#flywheelpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFlywheelResponseTypeDef

```python
# UpdateFlywheelResponseTypeDef definition

class UpdateFlywheelResponseTypeDef(TypedDict):
    FlywheelProperties: FlywheelPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlywheelPropertiesTypeDef](./type_defs.md#flywheelpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFlywheelRequestRequestTypeDef

```python
# CreateFlywheelRequestRequestTypeDef definition

class CreateFlywheelRequestRequestTypeDef(TypedDict):
    FlywheelName: str,
    DataAccessRoleArn: str,
    DataLakeS3Uri: str,
    ActiveModelArn: NotRequired[str],
    TaskConfig: NotRequired[TaskConfigTypeDef],  # (1)
    ModelType: NotRequired[ModelTypeType],  # (2)
    DataSecurityConfig: NotRequired[DataSecurityConfigTypeDef],  # (3)
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: TaskConfigTypeDef](./type_defs.md#taskconfigtypedef) 
2. See [:material-code-brackets: ModelTypeType](./literals.md#modeltypetype) 
3. See [:material-code-braces: DataSecurityConfigTypeDef](./type_defs.md#datasecurityconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeEntityRecognizerResponseTypeDef

```python
# DescribeEntityRecognizerResponseTypeDef definition

class DescribeEntityRecognizerResponseTypeDef(TypedDict):
    EntityRecognizerProperties: EntityRecognizerPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntityRecognizerPropertiesTypeDef](./type_defs.md#entityrecognizerpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEntityRecognizersResponseTypeDef

```python
# ListEntityRecognizersResponseTypeDef definition

class ListEntityRecognizersResponseTypeDef(TypedDict):
    EntityRecognizerPropertiesList: List[EntityRecognizerPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EntityRecognizerPropertiesTypeDef](./type_defs.md#entityrecognizerpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDetectTargetedSentimentResponseTypeDef

```python
# BatchDetectTargetedSentimentResponseTypeDef definition

class BatchDetectTargetedSentimentResponseTypeDef(TypedDict):
    ResultList: List[BatchDetectTargetedSentimentItemResultTypeDef],  # (1)
    ErrorList: List[BatchItemErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchDetectTargetedSentimentItemResultTypeDef](./type_defs.md#batchdetecttargetedsentimentitemresulttypedef) 
2. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
