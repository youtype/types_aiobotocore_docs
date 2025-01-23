# Type definitions

> [Index](../README.md) > [ConnectContactLens](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ConnectContactLens](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#connectcontactlens)
    type annotations stubs module [types-aiobotocore-connect-contact-lens](https://pypi.org/project/types-aiobotocore-connect-contact-lens/).



## PointOfInterestTypeDef

```python
# PointOfInterestTypeDef definition

class PointOfInterestTypeDef(TypedDict):
    BeginOffsetMillis: int,
    EndOffsetMillis: int,
```

## CharacterOffsetsTypeDef

```python
# CharacterOffsetsTypeDef definition

class CharacterOffsetsTypeDef(TypedDict):
    BeginOffsetChar: int,
    EndOffsetChar: int,
```

## ListRealtimeContactAnalysisSegmentsRequestRequestTypeDef

```python
# ListRealtimeContactAnalysisSegmentsRequestRequestTypeDef definition

class ListRealtimeContactAnalysisSegmentsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
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

## PostContactSummaryTypeDef

```python
# PostContactSummaryTypeDef definition

class PostContactSummaryTypeDef(TypedDict):
    Status: PostContactSummaryStatusType,  # (1)
    Content: NotRequired[str],
    FailureCode: NotRequired[PostContactSummaryFailureCodeType],  # (2)
```

1. See [:material-code-brackets: PostContactSummaryStatusType](./literals.md#postcontactsummarystatustype) 
2. See [:material-code-brackets: PostContactSummaryFailureCodeType](./literals.md#postcontactsummaryfailurecodetype) 
## CategoryDetailsTypeDef

```python
# CategoryDetailsTypeDef definition

class CategoryDetailsTypeDef(TypedDict):
    PointsOfInterest: List[PointOfInterestTypeDef],  # (1)
```

1. See [:material-code-braces: PointOfInterestTypeDef](./type_defs.md#pointofinteresttypedef) 
## IssueDetectedTypeDef

```python
# IssueDetectedTypeDef definition

class IssueDetectedTypeDef(TypedDict):
    CharacterOffsets: CharacterOffsetsTypeDef,  # (1)
```

1. See [:material-code-braces: CharacterOffsetsTypeDef](./type_defs.md#characteroffsetstypedef) 
## CategoriesTypeDef

```python
# CategoriesTypeDef definition

class CategoriesTypeDef(TypedDict):
    MatchedCategories: List[str],
    MatchedDetails: Dict[str, CategoryDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: CategoryDetailsTypeDef](./type_defs.md#categorydetailstypedef) 
## TranscriptTypeDef

```python
# TranscriptTypeDef definition

class TranscriptTypeDef(TypedDict):
    Id: str,
    ParticipantId: str,
    ParticipantRole: str,
    Content: str,
    BeginOffsetMillis: int,
    EndOffsetMillis: int,
    Sentiment: SentimentValueType,  # (1)
    IssuesDetected: NotRequired[List[IssueDetectedTypeDef]],  # (2)
```

1. See [:material-code-brackets: SentimentValueType](./literals.md#sentimentvaluetype) 
2. See [:material-code-braces: IssueDetectedTypeDef](./type_defs.md#issuedetectedtypedef) 
## RealtimeContactAnalysisSegmentTypeDef

```python
# RealtimeContactAnalysisSegmentTypeDef definition

class RealtimeContactAnalysisSegmentTypeDef(TypedDict):
    Transcript: NotRequired[TranscriptTypeDef],  # (1)
    Categories: NotRequired[CategoriesTypeDef],  # (2)
    PostContactSummary: NotRequired[PostContactSummaryTypeDef],  # (3)
```

1. See [:material-code-braces: TranscriptTypeDef](./type_defs.md#transcripttypedef) 
2. See [:material-code-braces: CategoriesTypeDef](./type_defs.md#categoriestypedef) 
3. See [:material-code-braces: PostContactSummaryTypeDef](./type_defs.md#postcontactsummarytypedef) 
## ListRealtimeContactAnalysisSegmentsResponseTypeDef

```python
# ListRealtimeContactAnalysisSegmentsResponseTypeDef definition

class ListRealtimeContactAnalysisSegmentsResponseTypeDef(TypedDict):
    Segments: List[RealtimeContactAnalysisSegmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RealtimeContactAnalysisSegmentTypeDef](./type_defs.md#realtimecontactanalysissegmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
