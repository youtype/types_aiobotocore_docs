# Type definitions

> [Index](../README.md) > [Textract](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Textract](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#textract)
    type annotations stubs module [types-aiobotocore-textract](https://pypi.org/project/types-aiobotocore-textract/).

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


## QueryUnionTypeDef

```python
# QueryUnionTypeDef definition

QueryUnionTypeDef = Union[
    QueryTypeDef,  # (1)
    QueryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: QueryTypeDef](./type_defs.md#querytypedef) 
2. See [:material-code-braces: QueryOutputTypeDef](./type_defs.md#queryoutputtypedef) 



## AdapterOverviewTypeDef

```python
# AdapterOverviewTypeDef definition

class AdapterOverviewTypeDef(TypedDict):
    AdapterId: NotRequired[str],
    AdapterName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    FeatureTypes: NotRequired[List[FeatureTypeType]],  # (1)
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
## AdapterTypeDef

```python
# AdapterTypeDef definition

class AdapterTypeDef(TypedDict):
    AdapterId: str,
    Version: str,
    Pages: NotRequired[Sequence[str]],
```

## S3ObjectTypeDef

```python
# S3ObjectTypeDef definition

class S3ObjectTypeDef(TypedDict):
    Bucket: NotRequired[str],
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## EvaluationMetricTypeDef

```python
# EvaluationMetricTypeDef definition

class EvaluationMetricTypeDef(TypedDict):
    F1Score: NotRequired[float],
    Precision: NotRequired[float],
    Recall: NotRequired[float],
```

## AdapterVersionOverviewTypeDef

```python
# AdapterVersionOverviewTypeDef definition

class AdapterVersionOverviewTypeDef(TypedDict):
    AdapterId: NotRequired[str],
    AdapterVersion: NotRequired[str],
    CreationTime: NotRequired[datetime],
    FeatureTypes: NotRequired[List[FeatureTypeType]],  # (1)
    Status: NotRequired[AdapterVersionStatusType],  # (2)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
2. See [:material-code-brackets: AdapterVersionStatusType](./literals.md#adapterversionstatustype) 
## DocumentMetadataTypeDef

```python
# DocumentMetadataTypeDef definition

class DocumentMetadataTypeDef(TypedDict):
    Pages: NotRequired[int],
```

## HumanLoopActivationOutputTypeDef

```python
# HumanLoopActivationOutputTypeDef definition

class HumanLoopActivationOutputTypeDef(TypedDict):
    HumanLoopArn: NotRequired[str],
    HumanLoopActivationReasons: NotRequired[List[str]],
    HumanLoopActivationConditionsEvaluationResults: NotRequired[str],
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

## NormalizedValueTypeDef

```python
# NormalizedValueTypeDef definition

class NormalizedValueTypeDef(TypedDict):
    Value: NotRequired[str],
    ValueType: NotRequired[ValueTypeType],  # (1)
```

1. See [:material-code-brackets: ValueTypeType](./literals.md#valuetypetype) 
## QueryOutputTypeDef

```python
# QueryOutputTypeDef definition

class QueryOutputTypeDef(TypedDict):
    Text: str,
    Alias: NotRequired[str],
    Pages: NotRequired[List[str]],
```

## RelationshipTypeDef

```python
# RelationshipTypeDef definition

class RelationshipTypeDef(TypedDict):
    Type: NotRequired[RelationshipTypeType],  # (1)
    Ids: NotRequired[List[str]],
```

1. See [:material-code-brackets: RelationshipTypeType](./literals.md#relationshiptypetype) 
## BoundingBoxTypeDef

```python
# BoundingBoxTypeDef definition

class BoundingBoxTypeDef(TypedDict):
    Width: NotRequired[float],
    Height: NotRequired[float],
    Left: NotRequired[float],
    Top: NotRequired[float],
```

## CreateAdapterRequestRequestTypeDef

```python
# CreateAdapterRequestRequestTypeDef definition

class CreateAdapterRequestRequestTypeDef(TypedDict):
    AdapterName: str,
    FeatureTypes: Sequence[FeatureTypeType],  # (1)
    ClientRequestToken: NotRequired[str],
    Description: NotRequired[str],
    AutoUpdate: NotRequired[AutoUpdateType],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
2. See [:material-code-brackets: AutoUpdateType](./literals.md#autoupdatetype) 
## OutputConfigTypeDef

```python
# OutputConfigTypeDef definition

class OutputConfigTypeDef(TypedDict):
    S3Bucket: str,
    S3Prefix: NotRequired[str],
```

## DeleteAdapterRequestRequestTypeDef

```python
# DeleteAdapterRequestRequestTypeDef definition

class DeleteAdapterRequestRequestTypeDef(TypedDict):
    AdapterId: str,
```

## DeleteAdapterVersionRequestRequestTypeDef

```python
# DeleteAdapterVersionRequestRequestTypeDef definition

class DeleteAdapterVersionRequestRequestTypeDef(TypedDict):
    AdapterId: str,
    AdapterVersion: str,
```

## DetectedSignatureTypeDef

```python
# DetectedSignatureTypeDef definition

class DetectedSignatureTypeDef(TypedDict):
    Page: NotRequired[int],
```

## SplitDocumentTypeDef

```python
# SplitDocumentTypeDef definition

class SplitDocumentTypeDef(TypedDict):
    Index: NotRequired[int],
    Pages: NotRequired[List[int]],
```

## UndetectedSignatureTypeDef

```python
# UndetectedSignatureTypeDef definition

class UndetectedSignatureTypeDef(TypedDict):
    Page: NotRequired[int],
```

## ExpenseCurrencyTypeDef

```python
# ExpenseCurrencyTypeDef definition

class ExpenseCurrencyTypeDef(TypedDict):
    Code: NotRequired[str],
    Confidence: NotRequired[float],
```

## ExpenseGroupPropertyTypeDef

```python
# ExpenseGroupPropertyTypeDef definition

class ExpenseGroupPropertyTypeDef(TypedDict):
    Types: NotRequired[List[str]],
    Id: NotRequired[str],
```

## ExpenseTypeTypeDef

```python
# ExpenseTypeTypeDef definition

class ExpenseTypeTypeDef(TypedDict):
    Text: NotRequired[str],
    Confidence: NotRequired[float],
```

## PointTypeDef

```python
# PointTypeDef definition

class PointTypeDef(TypedDict):
    X: NotRequired[float],
    Y: NotRequired[float],
```

## GetAdapterRequestRequestTypeDef

```python
# GetAdapterRequestRequestTypeDef definition

class GetAdapterRequestRequestTypeDef(TypedDict):
    AdapterId: str,
```

## GetAdapterVersionRequestRequestTypeDef

```python
# GetAdapterVersionRequestRequestTypeDef definition

class GetAdapterVersionRequestRequestTypeDef(TypedDict):
    AdapterId: str,
    AdapterVersion: str,
```

## GetDocumentAnalysisRequestRequestTypeDef

```python
# GetDocumentAnalysisRequestRequestTypeDef definition

class GetDocumentAnalysisRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## WarningTypeDef

```python
# WarningTypeDef definition

class WarningTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    Pages: NotRequired[List[int]],
```

## GetDocumentTextDetectionRequestRequestTypeDef

```python
# GetDocumentTextDetectionRequestRequestTypeDef definition

class GetDocumentTextDetectionRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetExpenseAnalysisRequestRequestTypeDef

```python
# GetExpenseAnalysisRequestRequestTypeDef definition

class GetExpenseAnalysisRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetLendingAnalysisRequestRequestTypeDef

```python
# GetLendingAnalysisRequestRequestTypeDef definition

class GetLendingAnalysisRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetLendingAnalysisSummaryRequestRequestTypeDef

```python
# GetLendingAnalysisSummaryRequestRequestTypeDef definition

class GetLendingAnalysisSummaryRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## HumanLoopDataAttributesTypeDef

```python
# HumanLoopDataAttributesTypeDef definition

class HumanLoopDataAttributesTypeDef(TypedDict):
    ContentClassifiers: NotRequired[Sequence[ContentClassifierType]],  # (1)
```

1. See [:material-code-brackets: ContentClassifierType](./literals.md#contentclassifiertype) 
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
    ResourceARN: str,
```

## NotificationChannelTypeDef

```python
# NotificationChannelTypeDef definition

class NotificationChannelTypeDef(TypedDict):
    SNSTopicArn: str,
    RoleArn: str,
```

## PredictionTypeDef

```python
# PredictionTypeDef definition

class PredictionTypeDef(TypedDict):
    Value: NotRequired[str],
    Confidence: NotRequired[float],
```

## QueryTypeDef

```python
# QueryTypeDef definition

class QueryTypeDef(TypedDict):
    Text: str,
    Alias: NotRequired[str],
    Pages: NotRequired[Sequence[str]],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateAdapterRequestRequestTypeDef

```python
# UpdateAdapterRequestRequestTypeDef definition

class UpdateAdapterRequestRequestTypeDef(TypedDict):
    AdapterId: str,
    Description: NotRequired[str],
    AdapterName: NotRequired[str],
    AutoUpdate: NotRequired[AutoUpdateType],  # (1)
```

1. See [:material-code-brackets: AutoUpdateType](./literals.md#autoupdatetype) 
## AdaptersConfigTypeDef

```python
# AdaptersConfigTypeDef definition

class AdaptersConfigTypeDef(TypedDict):
    Adapters: Sequence[AdapterTypeDef],  # (1)
```

1. See [:material-code-braces: AdapterTypeDef](./type_defs.md#adaptertypedef) 
## AdapterVersionDatasetConfigTypeDef

```python
# AdapterVersionDatasetConfigTypeDef definition

class AdapterVersionDatasetConfigTypeDef(TypedDict):
    ManifestS3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## DocumentLocationTypeDef

```python
# DocumentLocationTypeDef definition

class DocumentLocationTypeDef(TypedDict):
    S3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## AdapterVersionEvaluationMetricTypeDef

```python
# AdapterVersionEvaluationMetricTypeDef definition

class AdapterVersionEvaluationMetricTypeDef(TypedDict):
    Baseline: NotRequired[EvaluationMetricTypeDef],  # (1)
    AdapterVersion: NotRequired[EvaluationMetricTypeDef],  # (1)
    FeatureType: NotRequired[FeatureTypeType],  # (3)
```

1. See [:material-code-braces: EvaluationMetricTypeDef](./type_defs.md#evaluationmetrictypedef) 
2. See [:material-code-braces: EvaluationMetricTypeDef](./type_defs.md#evaluationmetrictypedef) 
3. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
## CreateAdapterResponseTypeDef

```python
# CreateAdapterResponseTypeDef definition

class CreateAdapterResponseTypeDef(TypedDict):
    AdapterId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAdapterVersionResponseTypeDef

```python
# CreateAdapterVersionResponseTypeDef definition

class CreateAdapterVersionResponseTypeDef(TypedDict):
    AdapterId: str,
    AdapterVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAdapterResponseTypeDef

```python
# GetAdapterResponseTypeDef definition

class GetAdapterResponseTypeDef(TypedDict):
    AdapterId: str,
    AdapterName: str,
    CreationTime: datetime,
    Description: str,
    FeatureTypes: List[FeatureTypeType],  # (1)
    AutoUpdate: AutoUpdateType,  # (2)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
2. See [:material-code-brackets: AutoUpdateType](./literals.md#autoupdatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAdapterVersionsResponseTypeDef

```python
# ListAdapterVersionsResponseTypeDef definition

class ListAdapterVersionsResponseTypeDef(TypedDict):
    AdapterVersions: List[AdapterVersionOverviewTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AdapterVersionOverviewTypeDef](./type_defs.md#adapterversionoverviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAdaptersResponseTypeDef

```python
# ListAdaptersResponseTypeDef definition

class ListAdaptersResponseTypeDef(TypedDict):
    Adapters: List[AdapterOverviewTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AdapterOverviewTypeDef](./type_defs.md#adapteroverviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDocumentAnalysisResponseTypeDef

```python
# StartDocumentAnalysisResponseTypeDef definition

class StartDocumentAnalysisResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDocumentTextDetectionResponseTypeDef

```python
# StartDocumentTextDetectionResponseTypeDef definition

class StartDocumentTextDetectionResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartExpenseAnalysisResponseTypeDef

```python
# StartExpenseAnalysisResponseTypeDef definition

class StartExpenseAnalysisResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartLendingAnalysisResponseTypeDef

```python
# StartLendingAnalysisResponseTypeDef definition

class StartLendingAnalysisResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAdapterResponseTypeDef

```python
# UpdateAdapterResponseTypeDef definition

class UpdateAdapterResponseTypeDef(TypedDict):
    AdapterId: str,
    AdapterName: str,
    CreationTime: datetime,
    Description: str,
    FeatureTypes: List[FeatureTypeType],  # (1)
    AutoUpdate: AutoUpdateType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
2. See [:material-code-brackets: AutoUpdateType](./literals.md#autoupdatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AnalyzeIDDetectionsTypeDef

```python
# AnalyzeIDDetectionsTypeDef definition

class AnalyzeIDDetectionsTypeDef(TypedDict):
    Text: str,
    NormalizedValue: NotRequired[NormalizedValueTypeDef],  # (1)
    Confidence: NotRequired[float],
```

1. See [:material-code-braces: NormalizedValueTypeDef](./type_defs.md#normalizedvaluetypedef) 
## DocumentTypeDef

```python
# DocumentTypeDef definition

class DocumentTypeDef(TypedDict):
    Bytes: NotRequired[BlobTypeDef],
    S3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## DocumentGroupTypeDef

```python
# DocumentGroupTypeDef definition

class DocumentGroupTypeDef(TypedDict):
    Type: NotRequired[str],
    SplitDocuments: NotRequired[List[SplitDocumentTypeDef]],  # (1)
    DetectedSignatures: NotRequired[List[DetectedSignatureTypeDef]],  # (2)
    UndetectedSignatures: NotRequired[List[UndetectedSignatureTypeDef]],  # (3)
```

1. See [:material-code-braces: SplitDocumentTypeDef](./type_defs.md#splitdocumenttypedef) 
2. See [:material-code-braces: DetectedSignatureTypeDef](./type_defs.md#detectedsignaturetypedef) 
3. See [:material-code-braces: UndetectedSignatureTypeDef](./type_defs.md#undetectedsignaturetypedef) 
## GeometryTypeDef

```python
# GeometryTypeDef definition

class GeometryTypeDef(TypedDict):
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (1)
    Polygon: NotRequired[List[PointTypeDef]],  # (2)
```

1. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
2. See [:material-code-braces: PointTypeDef](./type_defs.md#pointtypedef) 
## HumanLoopConfigTypeDef

```python
# HumanLoopConfigTypeDef definition

class HumanLoopConfigTypeDef(TypedDict):
    HumanLoopName: str,
    FlowDefinitionArn: str,
    DataAttributes: NotRequired[HumanLoopDataAttributesTypeDef],  # (1)
```

1. See [:material-code-braces: HumanLoopDataAttributesTypeDef](./type_defs.md#humanloopdataattributestypedef) 
## ListAdapterVersionsRequestPaginateTypeDef

```python
# ListAdapterVersionsRequestPaginateTypeDef definition

class ListAdapterVersionsRequestPaginateTypeDef(TypedDict):
    AdapterId: NotRequired[str],
    AfterCreationTime: NotRequired[TimestampTypeDef],
    BeforeCreationTime: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAdapterVersionsRequestRequestTypeDef

```python
# ListAdapterVersionsRequestRequestTypeDef definition

class ListAdapterVersionsRequestRequestTypeDef(TypedDict):
    AdapterId: NotRequired[str],
    AfterCreationTime: NotRequired[TimestampTypeDef],
    BeforeCreationTime: NotRequired[TimestampTypeDef],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAdaptersRequestPaginateTypeDef

```python
# ListAdaptersRequestPaginateTypeDef definition

class ListAdaptersRequestPaginateTypeDef(TypedDict):
    AfterCreationTime: NotRequired[TimestampTypeDef],
    BeforeCreationTime: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAdaptersRequestRequestTypeDef

```python
# ListAdaptersRequestRequestTypeDef definition

class ListAdaptersRequestRequestTypeDef(TypedDict):
    AfterCreationTime: NotRequired[TimestampTypeDef],
    BeforeCreationTime: NotRequired[TimestampTypeDef],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PageClassificationTypeDef

```python
# PageClassificationTypeDef definition

class PageClassificationTypeDef(TypedDict):
    PageType: List[PredictionTypeDef],  # (1)
    PageNumber: List[PredictionTypeDef],  # (1)
```

1. See [:material-code-braces: PredictionTypeDef](./type_defs.md#predictiontypedef) 
2. See [:material-code-braces: PredictionTypeDef](./type_defs.md#predictiontypedef) 
## CreateAdapterVersionRequestRequestTypeDef

```python
# CreateAdapterVersionRequestRequestTypeDef definition

class CreateAdapterVersionRequestRequestTypeDef(TypedDict):
    AdapterId: str,
    DatasetConfig: AdapterVersionDatasetConfigTypeDef,  # (1)
    OutputConfig: OutputConfigTypeDef,  # (2)
    ClientRequestToken: NotRequired[str],
    KMSKeyId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AdapterVersionDatasetConfigTypeDef](./type_defs.md#adapterversiondatasetconfigtypedef) 
2. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
## StartDocumentTextDetectionRequestRequestTypeDef

```python
# StartDocumentTextDetectionRequestRequestTypeDef definition

class StartDocumentTextDetectionRequestRequestTypeDef(TypedDict):
    DocumentLocation: DocumentLocationTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
    JobTag: NotRequired[str],
    NotificationChannel: NotRequired[NotificationChannelTypeDef],  # (2)
    OutputConfig: NotRequired[OutputConfigTypeDef],  # (3)
    KMSKeyId: NotRequired[str],
```

1. See [:material-code-braces: DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
3. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
## StartExpenseAnalysisRequestRequestTypeDef

```python
# StartExpenseAnalysisRequestRequestTypeDef definition

class StartExpenseAnalysisRequestRequestTypeDef(TypedDict):
    DocumentLocation: DocumentLocationTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
    JobTag: NotRequired[str],
    NotificationChannel: NotRequired[NotificationChannelTypeDef],  # (2)
    OutputConfig: NotRequired[OutputConfigTypeDef],  # (3)
    KMSKeyId: NotRequired[str],
```

1. See [:material-code-braces: DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
3. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
## StartLendingAnalysisRequestRequestTypeDef

```python
# StartLendingAnalysisRequestRequestTypeDef definition

class StartLendingAnalysisRequestRequestTypeDef(TypedDict):
    DocumentLocation: DocumentLocationTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
    JobTag: NotRequired[str],
    NotificationChannel: NotRequired[NotificationChannelTypeDef],  # (2)
    OutputConfig: NotRequired[OutputConfigTypeDef],  # (3)
    KMSKeyId: NotRequired[str],
```

1. See [:material-code-braces: DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
3. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
## GetAdapterVersionResponseTypeDef

```python
# GetAdapterVersionResponseTypeDef definition

class GetAdapterVersionResponseTypeDef(TypedDict):
    AdapterId: str,
    AdapterVersion: str,
    CreationTime: datetime,
    FeatureTypes: List[FeatureTypeType],  # (1)
    Status: AdapterVersionStatusType,  # (2)
    StatusMessage: str,
    DatasetConfig: AdapterVersionDatasetConfigTypeDef,  # (3)
    KMSKeyId: str,
    OutputConfig: OutputConfigTypeDef,  # (4)
    EvaluationMetrics: List[AdapterVersionEvaluationMetricTypeDef],  # (5)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
2. See [:material-code-brackets: AdapterVersionStatusType](./literals.md#adapterversionstatustype) 
3. See [:material-code-braces: AdapterVersionDatasetConfigTypeDef](./type_defs.md#adapterversiondatasetconfigtypedef) 
4. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
5. See [:material-code-braces: AdapterVersionEvaluationMetricTypeDef](./type_defs.md#adapterversionevaluationmetrictypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IdentityDocumentFieldTypeDef

```python
# IdentityDocumentFieldTypeDef definition

class IdentityDocumentFieldTypeDef(TypedDict):
    Type: NotRequired[AnalyzeIDDetectionsTypeDef],  # (1)
    ValueDetection: NotRequired[AnalyzeIDDetectionsTypeDef],  # (1)
```

1. See [:material-code-braces: AnalyzeIDDetectionsTypeDef](./type_defs.md#analyzeiddetectionstypedef) 
2. See [:material-code-braces: AnalyzeIDDetectionsTypeDef](./type_defs.md#analyzeiddetectionstypedef) 
## AnalyzeExpenseRequestRequestTypeDef

```python
# AnalyzeExpenseRequestRequestTypeDef definition

class AnalyzeExpenseRequestRequestTypeDef(TypedDict):
    Document: DocumentTypeDef,  # (1)
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
## AnalyzeIDRequestRequestTypeDef

```python
# AnalyzeIDRequestRequestTypeDef definition

class AnalyzeIDRequestRequestTypeDef(TypedDict):
    DocumentPages: Sequence[DocumentTypeDef],  # (1)
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
## DetectDocumentTextRequestRequestTypeDef

```python
# DetectDocumentTextRequestRequestTypeDef definition

class DetectDocumentTextRequestRequestTypeDef(TypedDict):
    Document: DocumentTypeDef,  # (1)
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
## LendingSummaryTypeDef

```python
# LendingSummaryTypeDef definition

class LendingSummaryTypeDef(TypedDict):
    DocumentGroups: NotRequired[List[DocumentGroupTypeDef]],  # (1)
    UndetectedDocumentTypes: NotRequired[List[str]],
```

1. See [:material-code-braces: DocumentGroupTypeDef](./type_defs.md#documentgrouptypedef) 
## BlockTypeDef

```python
# BlockTypeDef definition

class BlockTypeDef(TypedDict):
    BlockType: NotRequired[BlockTypeType],  # (1)
    Confidence: NotRequired[float],
    Text: NotRequired[str],
    TextType: NotRequired[TextTypeType],  # (2)
    RowIndex: NotRequired[int],
    ColumnIndex: NotRequired[int],
    RowSpan: NotRequired[int],
    ColumnSpan: NotRequired[int],
    Geometry: NotRequired[GeometryTypeDef],  # (3)
    Id: NotRequired[str],
    Relationships: NotRequired[List[RelationshipTypeDef]],  # (4)
    EntityTypes: NotRequired[List[EntityTypeType]],  # (5)
    SelectionStatus: NotRequired[SelectionStatusType],  # (6)
    Page: NotRequired[int],
    Query: NotRequired[QueryOutputTypeDef],  # (7)
```

1. See [:material-code-brackets: BlockTypeType](./literals.md#blocktypetype) 
2. See [:material-code-brackets: TextTypeType](./literals.md#texttypetype) 
3. See [:material-code-braces: GeometryTypeDef](./type_defs.md#geometrytypedef) 
4. See [:material-code-braces: RelationshipTypeDef](./type_defs.md#relationshiptypedef) 
5. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
6. See [:material-code-brackets: SelectionStatusType](./literals.md#selectionstatustype) 
7. See [:material-code-braces: QueryOutputTypeDef](./type_defs.md#queryoutputtypedef) 
## ExpenseDetectionTypeDef

```python
# ExpenseDetectionTypeDef definition

class ExpenseDetectionTypeDef(TypedDict):
    Text: NotRequired[str],
    Geometry: NotRequired[GeometryTypeDef],  # (1)
    Confidence: NotRequired[float],
```

1. See [:material-code-braces: GeometryTypeDef](./type_defs.md#geometrytypedef) 
## LendingDetectionTypeDef

```python
# LendingDetectionTypeDef definition

class LendingDetectionTypeDef(TypedDict):
    Text: NotRequired[str],
    SelectionStatus: NotRequired[SelectionStatusType],  # (1)
    Geometry: NotRequired[GeometryTypeDef],  # (2)
    Confidence: NotRequired[float],
```

1. See [:material-code-brackets: SelectionStatusType](./literals.md#selectionstatustype) 
2. See [:material-code-braces: GeometryTypeDef](./type_defs.md#geometrytypedef) 
## SignatureDetectionTypeDef

```python
# SignatureDetectionTypeDef definition

class SignatureDetectionTypeDef(TypedDict):
    Confidence: NotRequired[float],
    Geometry: NotRequired[GeometryTypeDef],  # (1)
```

1. See [:material-code-braces: GeometryTypeDef](./type_defs.md#geometrytypedef) 
## QueriesConfigTypeDef

```python
# QueriesConfigTypeDef definition

class QueriesConfigTypeDef(TypedDict):
    Queries: Sequence[QueryUnionTypeDef],  # (1)
```

1. See [:material-code-braces: QueryTypeDef](./type_defs.md#querytypedef) [:material-code-braces: QueryOutputTypeDef](./type_defs.md#queryoutputtypedef) 
## GetLendingAnalysisSummaryResponseTypeDef

```python
# GetLendingAnalysisSummaryResponseTypeDef definition

class GetLendingAnalysisSummaryResponseTypeDef(TypedDict):
    DocumentMetadata: DocumentMetadataTypeDef,  # (1)
    JobStatus: JobStatusType,  # (2)
    Summary: LendingSummaryTypeDef,  # (3)
    Warnings: List[WarningTypeDef],  # (4)
    StatusMessage: str,
    AnalyzeLendingModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: LendingSummaryTypeDef](./type_defs.md#lendingsummarytypedef) 
4. See [:material-code-braces: WarningTypeDef](./type_defs.md#warningtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AnalyzeDocumentResponseTypeDef

```python
# AnalyzeDocumentResponseTypeDef definition

class AnalyzeDocumentResponseTypeDef(TypedDict):
    DocumentMetadata: DocumentMetadataTypeDef,  # (1)
    Blocks: List[BlockTypeDef],  # (2)
    HumanLoopActivationOutput: HumanLoopActivationOutputTypeDef,  # (3)
    AnalyzeDocumentModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
2. See [:material-code-braces: BlockTypeDef](./type_defs.md#blocktypedef) 
3. See [:material-code-braces: HumanLoopActivationOutputTypeDef](./type_defs.md#humanloopactivationoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectDocumentTextResponseTypeDef

```python
# DetectDocumentTextResponseTypeDef definition

class DetectDocumentTextResponseTypeDef(TypedDict):
    DocumentMetadata: DocumentMetadataTypeDef,  # (1)
    Blocks: List[BlockTypeDef],  # (2)
    DetectDocumentTextModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
2. See [:material-code-braces: BlockTypeDef](./type_defs.md#blocktypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDocumentAnalysisResponseTypeDef

```python
# GetDocumentAnalysisResponseTypeDef definition

class GetDocumentAnalysisResponseTypeDef(TypedDict):
    DocumentMetadata: DocumentMetadataTypeDef,  # (1)
    JobStatus: JobStatusType,  # (2)
    Blocks: List[BlockTypeDef],  # (3)
    Warnings: List[WarningTypeDef],  # (4)
    StatusMessage: str,
    AnalyzeDocumentModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: BlockTypeDef](./type_defs.md#blocktypedef) 
4. See [:material-code-braces: WarningTypeDef](./type_defs.md#warningtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDocumentTextDetectionResponseTypeDef

```python
# GetDocumentTextDetectionResponseTypeDef definition

class GetDocumentTextDetectionResponseTypeDef(TypedDict):
    DocumentMetadata: DocumentMetadataTypeDef,  # (1)
    JobStatus: JobStatusType,  # (2)
    Blocks: List[BlockTypeDef],  # (3)
    Warnings: List[WarningTypeDef],  # (4)
    StatusMessage: str,
    DetectDocumentTextModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: BlockTypeDef](./type_defs.md#blocktypedef) 
4. See [:material-code-braces: WarningTypeDef](./type_defs.md#warningtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IdentityDocumentTypeDef

```python
# IdentityDocumentTypeDef definition

class IdentityDocumentTypeDef(TypedDict):
    DocumentIndex: NotRequired[int],
    IdentityDocumentFields: NotRequired[List[IdentityDocumentFieldTypeDef]],  # (1)
    Blocks: NotRequired[List[BlockTypeDef]],  # (2)
```

1. See [:material-code-braces: IdentityDocumentFieldTypeDef](./type_defs.md#identitydocumentfieldtypedef) 
2. See [:material-code-braces: BlockTypeDef](./type_defs.md#blocktypedef) 
## ExpenseFieldTypeDef

```python
# ExpenseFieldTypeDef definition

class ExpenseFieldTypeDef(TypedDict):
    Type: NotRequired[ExpenseTypeTypeDef],  # (1)
    LabelDetection: NotRequired[ExpenseDetectionTypeDef],  # (2)
    ValueDetection: NotRequired[ExpenseDetectionTypeDef],  # (2)
    PageNumber: NotRequired[int],
    Currency: NotRequired[ExpenseCurrencyTypeDef],  # (4)
    GroupProperties: NotRequired[List[ExpenseGroupPropertyTypeDef]],  # (5)
```

1. See [:material-code-braces: ExpenseTypeTypeDef](./type_defs.md#expensetypetypedef) 
2. See [:material-code-braces: ExpenseDetectionTypeDef](./type_defs.md#expensedetectiontypedef) 
3. See [:material-code-braces: ExpenseDetectionTypeDef](./type_defs.md#expensedetectiontypedef) 
4. See [:material-code-braces: ExpenseCurrencyTypeDef](./type_defs.md#expensecurrencytypedef) 
5. See [:material-code-braces: ExpenseGroupPropertyTypeDef](./type_defs.md#expensegrouppropertytypedef) 
## LendingFieldTypeDef

```python
# LendingFieldTypeDef definition

class LendingFieldTypeDef(TypedDict):
    Type: NotRequired[str],
    KeyDetection: NotRequired[LendingDetectionTypeDef],  # (1)
    ValueDetections: NotRequired[List[LendingDetectionTypeDef]],  # (2)
```

1. See [:material-code-braces: LendingDetectionTypeDef](./type_defs.md#lendingdetectiontypedef) 
2. See [:material-code-braces: LendingDetectionTypeDef](./type_defs.md#lendingdetectiontypedef) 
## AnalyzeDocumentRequestRequestTypeDef

```python
# AnalyzeDocumentRequestRequestTypeDef definition

class AnalyzeDocumentRequestRequestTypeDef(TypedDict):
    Document: DocumentTypeDef,  # (1)
    FeatureTypes: Sequence[FeatureTypeType],  # (2)
    HumanLoopConfig: NotRequired[HumanLoopConfigTypeDef],  # (3)
    QueriesConfig: NotRequired[QueriesConfigTypeDef],  # (4)
    AdaptersConfig: NotRequired[AdaptersConfigTypeDef],  # (5)
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
3. See [:material-code-braces: HumanLoopConfigTypeDef](./type_defs.md#humanloopconfigtypedef) 
4. See [:material-code-braces: QueriesConfigTypeDef](./type_defs.md#queriesconfigtypedef) 
5. See [:material-code-braces: AdaptersConfigTypeDef](./type_defs.md#adaptersconfigtypedef) 
## StartDocumentAnalysisRequestRequestTypeDef

```python
# StartDocumentAnalysisRequestRequestTypeDef definition

class StartDocumentAnalysisRequestRequestTypeDef(TypedDict):
    DocumentLocation: DocumentLocationTypeDef,  # (1)
    FeatureTypes: Sequence[FeatureTypeType],  # (2)
    ClientRequestToken: NotRequired[str],
    JobTag: NotRequired[str],
    NotificationChannel: NotRequired[NotificationChannelTypeDef],  # (3)
    OutputConfig: NotRequired[OutputConfigTypeDef],  # (4)
    KMSKeyId: NotRequired[str],
    QueriesConfig: NotRequired[QueriesConfigTypeDef],  # (5)
    AdaptersConfig: NotRequired[AdaptersConfigTypeDef],  # (6)
```

1. See [:material-code-braces: DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef) 
2. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
3. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
4. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
5. See [:material-code-braces: QueriesConfigTypeDef](./type_defs.md#queriesconfigtypedef) 
6. See [:material-code-braces: AdaptersConfigTypeDef](./type_defs.md#adaptersconfigtypedef) 
## AnalyzeIDResponseTypeDef

```python
# AnalyzeIDResponseTypeDef definition

class AnalyzeIDResponseTypeDef(TypedDict):
    IdentityDocuments: List[IdentityDocumentTypeDef],  # (1)
    DocumentMetadata: DocumentMetadataTypeDef,  # (2)
    AnalyzeIDModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: IdentityDocumentTypeDef](./type_defs.md#identitydocumenttypedef) 
2. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LineItemFieldsTypeDef

```python
# LineItemFieldsTypeDef definition

class LineItemFieldsTypeDef(TypedDict):
    LineItemExpenseFields: NotRequired[List[ExpenseFieldTypeDef]],  # (1)
```

1. See [:material-code-braces: ExpenseFieldTypeDef](./type_defs.md#expensefieldtypedef) 
## LendingDocumentTypeDef

```python
# LendingDocumentTypeDef definition

class LendingDocumentTypeDef(TypedDict):
    LendingFields: NotRequired[List[LendingFieldTypeDef]],  # (1)
    SignatureDetections: NotRequired[List[SignatureDetectionTypeDef]],  # (2)
```

1. See [:material-code-braces: LendingFieldTypeDef](./type_defs.md#lendingfieldtypedef) 
2. See [:material-code-braces: SignatureDetectionTypeDef](./type_defs.md#signaturedetectiontypedef) 
## LineItemGroupTypeDef

```python
# LineItemGroupTypeDef definition

class LineItemGroupTypeDef(TypedDict):
    LineItemGroupIndex: NotRequired[int],
    LineItems: NotRequired[List[LineItemFieldsTypeDef]],  # (1)
```

1. See [:material-code-braces: LineItemFieldsTypeDef](./type_defs.md#lineitemfieldstypedef) 
## ExpenseDocumentTypeDef

```python
# ExpenseDocumentTypeDef definition

class ExpenseDocumentTypeDef(TypedDict):
    ExpenseIndex: NotRequired[int],
    SummaryFields: NotRequired[List[ExpenseFieldTypeDef]],  # (1)
    LineItemGroups: NotRequired[List[LineItemGroupTypeDef]],  # (2)
    Blocks: NotRequired[List[BlockTypeDef]],  # (3)
```

1. See [:material-code-braces: ExpenseFieldTypeDef](./type_defs.md#expensefieldtypedef) 
2. See [:material-code-braces: LineItemGroupTypeDef](./type_defs.md#lineitemgrouptypedef) 
3. See [:material-code-braces: BlockTypeDef](./type_defs.md#blocktypedef) 
## AnalyzeExpenseResponseTypeDef

```python
# AnalyzeExpenseResponseTypeDef definition

class AnalyzeExpenseResponseTypeDef(TypedDict):
    DocumentMetadata: DocumentMetadataTypeDef,  # (1)
    ExpenseDocuments: List[ExpenseDocumentTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
2. See [:material-code-braces: ExpenseDocumentTypeDef](./type_defs.md#expensedocumenttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExtractionTypeDef

```python
# ExtractionTypeDef definition

class ExtractionTypeDef(TypedDict):
    LendingDocument: NotRequired[LendingDocumentTypeDef],  # (1)
    ExpenseDocument: NotRequired[ExpenseDocumentTypeDef],  # (2)
    IdentityDocument: NotRequired[IdentityDocumentTypeDef],  # (3)
```

1. See [:material-code-braces: LendingDocumentTypeDef](./type_defs.md#lendingdocumenttypedef) 
2. See [:material-code-braces: ExpenseDocumentTypeDef](./type_defs.md#expensedocumenttypedef) 
3. See [:material-code-braces: IdentityDocumentTypeDef](./type_defs.md#identitydocumenttypedef) 
## GetExpenseAnalysisResponseTypeDef

```python
# GetExpenseAnalysisResponseTypeDef definition

class GetExpenseAnalysisResponseTypeDef(TypedDict):
    DocumentMetadata: DocumentMetadataTypeDef,  # (1)
    JobStatus: JobStatusType,  # (2)
    ExpenseDocuments: List[ExpenseDocumentTypeDef],  # (3)
    Warnings: List[WarningTypeDef],  # (4)
    StatusMessage: str,
    AnalyzeExpenseModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: ExpenseDocumentTypeDef](./type_defs.md#expensedocumenttypedef) 
4. See [:material-code-braces: WarningTypeDef](./type_defs.md#warningtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LendingResultTypeDef

```python
# LendingResultTypeDef definition

class LendingResultTypeDef(TypedDict):
    Page: NotRequired[int],
    PageClassification: NotRequired[PageClassificationTypeDef],  # (1)
    Extractions: NotRequired[List[ExtractionTypeDef]],  # (2)
```

1. See [:material-code-braces: PageClassificationTypeDef](./type_defs.md#pageclassificationtypedef) 
2. See [:material-code-braces: ExtractionTypeDef](./type_defs.md#extractiontypedef) 
## GetLendingAnalysisResponseTypeDef

```python
# GetLendingAnalysisResponseTypeDef definition

class GetLendingAnalysisResponseTypeDef(TypedDict):
    DocumentMetadata: DocumentMetadataTypeDef,  # (1)
    JobStatus: JobStatusType,  # (2)
    Results: List[LendingResultTypeDef],  # (3)
    Warnings: List[WarningTypeDef],  # (4)
    StatusMessage: str,
    AnalyzeLendingModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: LendingResultTypeDef](./type_defs.md#lendingresulttypedef) 
4. See [:material-code-braces: WarningTypeDef](./type_defs.md#warningtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
