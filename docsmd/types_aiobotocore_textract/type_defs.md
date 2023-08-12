# Type definitions

> [Index](../README.md) > [Textract](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Textract](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
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
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## NormalizedValueTypeDef

```python
# NormalizedValueTypeDef definition

class NormalizedValueTypeDef(TypedDict):
    Value: NotRequired[str],
    ValueType: NotRequired[ValueTypeType],  # (1)
```

1. See [:material-code-brackets: ValueTypeType](./literals.md#valuetypetype) 
## QueryTypeDef

```python
# QueryTypeDef definition

class QueryTypeDef(TypedDict):
    Text: str,
    Alias: NotRequired[str],
    Pages: NotRequired[Sequence[str]],
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

## S3ObjectTypeDef

```python
# S3ObjectTypeDef definition

class S3ObjectTypeDef(TypedDict):
    Bucket: NotRequired[str],
    Name: NotRequired[str],
    Version: NotRequired[str],
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
## NotificationChannelTypeDef

```python
# NotificationChannelTypeDef definition

class NotificationChannelTypeDef(TypedDict):
    SNSTopicArn: str,
    RoleArn: str,
```

## OutputConfigTypeDef

```python
# OutputConfigTypeDef definition

class OutputConfigTypeDef(TypedDict):
    S3Bucket: str,
    S3Prefix: NotRequired[str],
```

## PredictionTypeDef

```python
# PredictionTypeDef definition

class PredictionTypeDef(TypedDict):
    Value: NotRequired[str],
    Confidence: NotRequired[float],
```

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
## AnalyzeIDDetectionsTypeDef

```python
# AnalyzeIDDetectionsTypeDef definition

class AnalyzeIDDetectionsTypeDef(TypedDict):
    Text: str,
    NormalizedValue: NotRequired[NormalizedValueTypeDef],  # (1)
    Confidence: NotRequired[float],
```

1. See [:material-code-braces: NormalizedValueTypeDef](./type_defs.md#normalizedvaluetypedef) 
## QueriesConfigTypeDef

```python
# QueriesConfigTypeDef definition

class QueriesConfigTypeDef(TypedDict):
    Queries: Sequence[QueryTypeDef],  # (1)
```

1. See [:material-code-braces: QueryTypeDef](./type_defs.md#querytypedef) 
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
## DocumentLocationTypeDef

```python
# DocumentLocationTypeDef definition

class DocumentLocationTypeDef(TypedDict):
    S3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## DocumentTypeDef

```python
# DocumentTypeDef definition

class DocumentTypeDef(TypedDict):
    Bytes: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    S3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
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
## PageClassificationTypeDef

```python
# PageClassificationTypeDef definition

class PageClassificationTypeDef(TypedDict):
    PageType: List[PredictionTypeDef],  # (1)
    PageNumber: List[PredictionTypeDef],  # (1)
```

1. See [:material-code-braces: PredictionTypeDef](./type_defs.md#predictiontypedef) 
2. See [:material-code-braces: PredictionTypeDef](./type_defs.md#predictiontypedef) 
## IdentityDocumentFieldTypeDef

```python
# IdentityDocumentFieldTypeDef definition

class IdentityDocumentFieldTypeDef(TypedDict):
    Type: NotRequired[AnalyzeIDDetectionsTypeDef],  # (1)
    ValueDetection: NotRequired[AnalyzeIDDetectionsTypeDef],  # (1)
```

1. See [:material-code-braces: AnalyzeIDDetectionsTypeDef](./type_defs.md#analyzeiddetectionstypedef) 
2. See [:material-code-braces: AnalyzeIDDetectionsTypeDef](./type_defs.md#analyzeiddetectionstypedef) 
## LendingSummaryTypeDef

```python
# LendingSummaryTypeDef definition

class LendingSummaryTypeDef(TypedDict):
    DocumentGroups: NotRequired[List[DocumentGroupTypeDef]],  # (1)
    UndetectedDocumentTypes: NotRequired[List[str]],
```

1. See [:material-code-braces: DocumentGroupTypeDef](./type_defs.md#documentgrouptypedef) 
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
```

1. See [:material-code-braces: DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef) 
2. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
3. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
4. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
5. See [:material-code-braces: QueriesConfigTypeDef](./type_defs.md#queriesconfigtypedef) 
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
    Query: NotRequired[QueryTypeDef],  # (7)
```

1. See [:material-code-brackets: BlockTypeType](./literals.md#blocktypetype) 
2. See [:material-code-brackets: TextTypeType](./literals.md#texttypetype) 
3. See [:material-code-braces: GeometryTypeDef](./type_defs.md#geometrytypedef) 
4. See [:material-code-braces: RelationshipTypeDef](./type_defs.md#relationshiptypedef) 
5. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
6. See [:material-code-brackets: SelectionStatusType](./literals.md#selectionstatustype) 
7. See [:material-code-braces: QueryTypeDef](./type_defs.md#querytypedef) 
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
## AnalyzeDocumentRequestRequestTypeDef

```python
# AnalyzeDocumentRequestRequestTypeDef definition

class AnalyzeDocumentRequestRequestTypeDef(TypedDict):
    Document: DocumentTypeDef,  # (1)
    FeatureTypes: Sequence[FeatureTypeType],  # (2)
    HumanLoopConfig: NotRequired[HumanLoopConfigTypeDef],  # (3)
    QueriesConfig: NotRequired[QueriesConfigTypeDef],  # (4)
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
3. See [:material-code-braces: HumanLoopConfigTypeDef](./type_defs.md#humanloopconfigtypedef) 
4. See [:material-code-braces: QueriesConfigTypeDef](./type_defs.md#queriesconfigtypedef) 
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
    NextToken: str,
    Blocks: List[BlockTypeDef],  # (3)
    Warnings: List[WarningTypeDef],  # (4)
    StatusMessage: str,
    AnalyzeDocumentModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
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
    NextToken: str,
    Blocks: List[BlockTypeDef],  # (3)
    Warnings: List[WarningTypeDef],  # (4)
    StatusMessage: str,
    DetectDocumentTextModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
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
    NextToken: str,
    ExpenseDocuments: List[ExpenseDocumentTypeDef],  # (3)
    Warnings: List[WarningTypeDef],  # (4)
    StatusMessage: str,
    AnalyzeExpenseModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
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
    NextToken: str,
    Results: List[LendingResultTypeDef],  # (3)
    Warnings: List[WarningTypeDef],  # (4)
    StatusMessage: str,
    AnalyzeLendingModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: LendingResultTypeDef](./type_defs.md#lendingresulttypedef) 
4. See [:material-code-braces: WarningTypeDef](./type_defs.md#warningtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
