# Type definitions

> [Index](../README.md) > [Rekognition](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Rekognition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#rekognition)
    type annotations stubs module [types-aiobotocore-rekognition](https://pypi.org/project/types-aiobotocore-rekognition/).

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


## ConnectedHomeSettingsUnionTypeDef

```python
# ConnectedHomeSettingsUnionTypeDef definition

ConnectedHomeSettingsUnionTypeDef = Union[
    ConnectedHomeSettingsTypeDef,  # (1)
    ConnectedHomeSettingsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConnectedHomeSettingsTypeDef](./type_defs.md#connectedhomesettingstypedef) 
2. See [:material-code-braces: ConnectedHomeSettingsOutputTypeDef](./type_defs.md#connectedhomesettingsoutputtypedef) 

## RegionOfInterestUnionTypeDef

```python
# RegionOfInterestUnionTypeDef definition

RegionOfInterestUnionTypeDef = Union[
    RegionOfInterestTypeDef,  # (1)
    RegionOfInterestOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RegionOfInterestTypeDef](./type_defs.md#regionofinteresttypedef) 
2. See [:material-code-braces: RegionOfInterestOutputTypeDef](./type_defs.md#regionofinterestoutputtypedef) 



## AgeRangeTypeDef

```python
# AgeRangeTypeDef definition

class AgeRangeTypeDef(TypedDict):
    Low: NotRequired[int],
    High: NotRequired[int],
```

## AssociateFacesRequestRequestTypeDef

```python
# AssociateFacesRequestRequestTypeDef definition

class AssociateFacesRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    UserId: str,
    FaceIds: Sequence[str],
    UserMatchThreshold: NotRequired[float],
    ClientRequestToken: NotRequired[str],
```

## AssociatedFaceTypeDef

```python
# AssociatedFaceTypeDef definition

class AssociatedFaceTypeDef(TypedDict):
    FaceId: NotRequired[str],
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

## UnsuccessfulFaceAssociationTypeDef

```python
# UnsuccessfulFaceAssociationTypeDef definition

class UnsuccessfulFaceAssociationTypeDef(TypedDict):
    FaceId: NotRequired[str],
    UserId: NotRequired[str],
    Confidence: NotRequired[float],
    Reasons: NotRequired[List[UnsuccessfulFaceAssociationReasonType]],  # (1)
```

1. See [:material-code-brackets: UnsuccessfulFaceAssociationReasonType](./literals.md#unsuccessfulfaceassociationreasontype) 
## AudioMetadataTypeDef

```python
# AudioMetadataTypeDef definition

class AudioMetadataTypeDef(TypedDict):
    Codec: NotRequired[str],
    DurationMillis: NotRequired[int],
    SampleRate: NotRequired[int],
    NumberOfChannels: NotRequired[int],
```

## BoundingBoxTypeDef

```python
# BoundingBoxTypeDef definition

class BoundingBoxTypeDef(TypedDict):
    Width: NotRequired[float],
    Height: NotRequired[float],
    Left: NotRequired[float],
    Top: NotRequired[float],
```

## S3ObjectTypeDef

```python
# S3ObjectTypeDef definition

class S3ObjectTypeDef(TypedDict):
    Bucket: NotRequired[str],
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## BeardTypeDef

```python
# BeardTypeDef definition

class BeardTypeDef(TypedDict):
    Value: NotRequired[bool],
    Confidence: NotRequired[float],
```

## BlackFrameTypeDef

```python
# BlackFrameTypeDef definition

class BlackFrameTypeDef(TypedDict):
    MaxPixelThreshold: NotRequired[float],
    MinCoveragePercentage: NotRequired[float],
```

## KnownGenderTypeDef

```python
# KnownGenderTypeDef definition

class KnownGenderTypeDef(TypedDict):
    Type: NotRequired[KnownGenderTypeType],  # (1)
```

1. See [:material-code-brackets: KnownGenderTypeType](./literals.md#knowngendertypetype) 
## EmotionTypeDef

```python
# EmotionTypeDef definition

class EmotionTypeDef(TypedDict):
    Type: NotRequired[EmotionNameType],  # (1)
    Confidence: NotRequired[float],
```

1. See [:material-code-brackets: EmotionNameType](./literals.md#emotionnametype) 
## ImageQualityTypeDef

```python
# ImageQualityTypeDef definition

class ImageQualityTypeDef(TypedDict):
    Brightness: NotRequired[float],
    Sharpness: NotRequired[float],
```

## LandmarkTypeDef

```python
# LandmarkTypeDef definition

class LandmarkTypeDef(TypedDict):
    Type: NotRequired[LandmarkTypeType],  # (1)
    X: NotRequired[float],
    Y: NotRequired[float],
```

1. See [:material-code-brackets: LandmarkTypeType](./literals.md#landmarktypetype) 
## PoseTypeDef

```python
# PoseTypeDef definition

class PoseTypeDef(TypedDict):
    Roll: NotRequired[float],
    Yaw: NotRequired[float],
    Pitch: NotRequired[float],
```

## SmileTypeDef

```python
# SmileTypeDef definition

class SmileTypeDef(TypedDict):
    Value: NotRequired[bool],
    Confidence: NotRequired[float],
```

## ConnectedHomeSettingsForUpdateTypeDef

```python
# ConnectedHomeSettingsForUpdateTypeDef definition

class ConnectedHomeSettingsForUpdateTypeDef(TypedDict):
    Labels: NotRequired[Sequence[str]],
    MinConfidence: NotRequired[float],
```

## ConnectedHomeSettingsOutputTypeDef

```python
# ConnectedHomeSettingsOutputTypeDef definition

class ConnectedHomeSettingsOutputTypeDef(TypedDict):
    Labels: List[str],
    MinConfidence: NotRequired[float],
```

## ConnectedHomeSettingsTypeDef

```python
# ConnectedHomeSettingsTypeDef definition

class ConnectedHomeSettingsTypeDef(TypedDict):
    Labels: Sequence[str],
    MinConfidence: NotRequired[float],
```

## ContentTypeTypeDef

```python
# ContentTypeTypeDef definition

class ContentTypeTypeDef(TypedDict):
    Confidence: NotRequired[float],
    Name: NotRequired[str],
```

## ModerationLabelTypeDef

```python
# ModerationLabelTypeDef definition

class ModerationLabelTypeDef(TypedDict):
    Confidence: NotRequired[float],
    Name: NotRequired[str],
    ParentName: NotRequired[str],
    TaxonomyLevel: NotRequired[int],
```

## OutputConfigTypeDef

```python
# OutputConfigTypeDef definition

class OutputConfigTypeDef(TypedDict):
    S3Bucket: NotRequired[str],
    S3KeyPrefix: NotRequired[str],
```

## CoversBodyPartTypeDef

```python
# CoversBodyPartTypeDef definition

class CoversBodyPartTypeDef(TypedDict):
    Confidence: NotRequired[float],
    Value: NotRequired[bool],
```

## CreateCollectionRequestRequestTypeDef

```python
# CreateCollectionRequestRequestTypeDef definition

class CreateCollectionRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    Tags: NotRequired[Mapping[str, str]],
```

## LivenessOutputConfigTypeDef

```python
# LivenessOutputConfigTypeDef definition

class LivenessOutputConfigTypeDef(TypedDict):
    S3Bucket: str,
    S3KeyPrefix: NotRequired[str],
```

## CreateProjectRequestRequestTypeDef

```python
# CreateProjectRequestRequestTypeDef definition

class CreateProjectRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    Feature: NotRequired[CustomizationFeatureType],  # (1)
    AutoUpdate: NotRequired[ProjectAutoUpdateType],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: CustomizationFeatureType](./literals.md#customizationfeaturetype) 
2. See [:material-code-brackets: ProjectAutoUpdateType](./literals.md#projectautoupdatetype) 
## StreamProcessorDataSharingPreferenceTypeDef

```python
# StreamProcessorDataSharingPreferenceTypeDef definition

class StreamProcessorDataSharingPreferenceTypeDef(TypedDict):
    OptIn: bool,
```

## StreamProcessorNotificationChannelTypeDef

```python
# StreamProcessorNotificationChannelTypeDef definition

class StreamProcessorNotificationChannelTypeDef(TypedDict):
    SNSTopicArn: str,
```

## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    UserId: str,
    ClientRequestToken: NotRequired[str],
```

## CustomizationFeatureContentModerationConfigTypeDef

```python
# CustomizationFeatureContentModerationConfigTypeDef definition

class CustomizationFeatureContentModerationConfigTypeDef(TypedDict):
    ConfidenceThreshold: NotRequired[float],
```

## DatasetStatsTypeDef

```python
# DatasetStatsTypeDef definition

class DatasetStatsTypeDef(TypedDict):
    LabeledEntries: NotRequired[int],
    TotalEntries: NotRequired[int],
    TotalLabels: NotRequired[int],
    ErrorEntries: NotRequired[int],
```

## DatasetLabelStatsTypeDef

```python
# DatasetLabelStatsTypeDef definition

class DatasetLabelStatsTypeDef(TypedDict):
    EntryCount: NotRequired[int],
    BoundingBoxCount: NotRequired[int],
```

## DatasetMetadataTypeDef

```python
# DatasetMetadataTypeDef definition

class DatasetMetadataTypeDef(TypedDict):
    CreationTimestamp: NotRequired[datetime],
    DatasetType: NotRequired[DatasetTypeType],  # (1)
    DatasetArn: NotRequired[str],
    Status: NotRequired[DatasetStatusType],  # (2)
    StatusMessage: NotRequired[str],
    StatusMessageCode: NotRequired[DatasetStatusMessageCodeType],  # (3)
```

1. See [:material-code-brackets: DatasetTypeType](./literals.md#datasettypetype) 
2. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
3. See [:material-code-brackets: DatasetStatusMessageCodeType](./literals.md#datasetstatusmessagecodetype) 
## DeleteCollectionRequestRequestTypeDef

```python
# DeleteCollectionRequestRequestTypeDef definition

class DeleteCollectionRequestRequestTypeDef(TypedDict):
    CollectionId: str,
```

## DeleteDatasetRequestRequestTypeDef

```python
# DeleteDatasetRequestRequestTypeDef definition

class DeleteDatasetRequestRequestTypeDef(TypedDict):
    DatasetArn: str,
```

## DeleteFacesRequestRequestTypeDef

```python
# DeleteFacesRequestRequestTypeDef definition

class DeleteFacesRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    FaceIds: Sequence[str],
```

## UnsuccessfulFaceDeletionTypeDef

```python
# UnsuccessfulFaceDeletionTypeDef definition

class UnsuccessfulFaceDeletionTypeDef(TypedDict):
    FaceId: NotRequired[str],
    UserId: NotRequired[str],
    Reasons: NotRequired[List[UnsuccessfulFaceDeletionReasonType]],  # (1)
```

1. See [:material-code-brackets: UnsuccessfulFaceDeletionReasonType](./literals.md#unsuccessfulfacedeletionreasontype) 
## DeleteProjectPolicyRequestRequestTypeDef

```python
# DeleteProjectPolicyRequestRequestTypeDef definition

class DeleteProjectPolicyRequestRequestTypeDef(TypedDict):
    ProjectArn: str,
    PolicyName: str,
    PolicyRevisionId: NotRequired[str],
```

## DeleteProjectRequestRequestTypeDef

```python
# DeleteProjectRequestRequestTypeDef definition

class DeleteProjectRequestRequestTypeDef(TypedDict):
    ProjectArn: str,
```

## DeleteProjectVersionRequestRequestTypeDef

```python
# DeleteProjectVersionRequestRequestTypeDef definition

class DeleteProjectVersionRequestRequestTypeDef(TypedDict):
    ProjectVersionArn: str,
```

## DeleteStreamProcessorRequestRequestTypeDef

```python
# DeleteStreamProcessorRequestRequestTypeDef definition

class DeleteStreamProcessorRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    UserId: str,
    ClientRequestToken: NotRequired[str],
```

## DescribeCollectionRequestRequestTypeDef

```python
# DescribeCollectionRequestRequestTypeDef definition

class DescribeCollectionRequestRequestTypeDef(TypedDict):
    CollectionId: str,
```

## DescribeDatasetRequestRequestTypeDef

```python
# DescribeDatasetRequestRequestTypeDef definition

class DescribeDatasetRequestRequestTypeDef(TypedDict):
    DatasetArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeProjectVersionsRequestRequestTypeDef

```python
# DescribeProjectVersionsRequestRequestTypeDef definition

class DescribeProjectVersionsRequestRequestTypeDef(TypedDict):
    ProjectArn: str,
    VersionNames: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeProjectsRequestRequestTypeDef

```python
# DescribeProjectsRequestRequestTypeDef definition

class DescribeProjectsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ProjectNames: NotRequired[Sequence[str]],
    Features: NotRequired[Sequence[CustomizationFeatureType]],  # (1)
```

1. See [:material-code-brackets: CustomizationFeatureType](./literals.md#customizationfeaturetype) 
## DescribeStreamProcessorRequestRequestTypeDef

```python
# DescribeStreamProcessorRequestRequestTypeDef definition

class DescribeStreamProcessorRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DetectLabelsImageQualityTypeDef

```python
# DetectLabelsImageQualityTypeDef definition

class DetectLabelsImageQualityTypeDef(TypedDict):
    Brightness: NotRequired[float],
    Sharpness: NotRequired[float],
    Contrast: NotRequired[float],
```

## DominantColorTypeDef

```python
# DominantColorTypeDef definition

class DominantColorTypeDef(TypedDict):
    Red: NotRequired[int],
    Blue: NotRequired[int],
    Green: NotRequired[int],
    HexCode: NotRequired[str],
    CSSColor: NotRequired[str],
    SimplifiedColor: NotRequired[str],
    PixelPercent: NotRequired[float],
```

## DetectLabelsImagePropertiesSettingsTypeDef

```python
# DetectLabelsImagePropertiesSettingsTypeDef definition

class DetectLabelsImagePropertiesSettingsTypeDef(TypedDict):
    MaxDominantColors: NotRequired[int],
```

## GeneralLabelsSettingsTypeDef

```python
# GeneralLabelsSettingsTypeDef definition

class GeneralLabelsSettingsTypeDef(TypedDict):
    LabelInclusionFilters: NotRequired[Sequence[str]],
    LabelExclusionFilters: NotRequired[Sequence[str]],
    LabelCategoryInclusionFilters: NotRequired[Sequence[str]],
    LabelCategoryExclusionFilters: NotRequired[Sequence[str]],
```

## HumanLoopActivationOutputTypeDef

```python
# HumanLoopActivationOutputTypeDef definition

class HumanLoopActivationOutputTypeDef(TypedDict):
    HumanLoopArn: NotRequired[str],
    HumanLoopActivationReasons: NotRequired[List[str]],
    HumanLoopActivationConditionsEvaluationResults: NotRequired[str],
```

## ProtectiveEquipmentSummarizationAttributesTypeDef

```python
# ProtectiveEquipmentSummarizationAttributesTypeDef definition

class ProtectiveEquipmentSummarizationAttributesTypeDef(TypedDict):
    MinConfidence: float,
    RequiredEquipmentTypes: Sequence[ProtectiveEquipmentTypeType],  # (1)
```

1. See [:material-code-brackets: ProtectiveEquipmentTypeType](./literals.md#protectiveequipmenttypetype) 
## ProtectiveEquipmentSummaryTypeDef

```python
# ProtectiveEquipmentSummaryTypeDef definition

class ProtectiveEquipmentSummaryTypeDef(TypedDict):
    PersonsWithRequiredEquipment: NotRequired[List[int]],
    PersonsWithoutRequiredEquipment: NotRequired[List[int]],
    PersonsIndeterminate: NotRequired[List[int]],
```

## DetectionFilterTypeDef

```python
# DetectionFilterTypeDef definition

class DetectionFilterTypeDef(TypedDict):
    MinConfidence: NotRequired[float],
    MinBoundingBoxHeight: NotRequired[float],
    MinBoundingBoxWidth: NotRequired[float],
```

## DisassociateFacesRequestRequestTypeDef

```python
# DisassociateFacesRequestRequestTypeDef definition

class DisassociateFacesRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    UserId: str,
    FaceIds: Sequence[str],
    ClientRequestToken: NotRequired[str],
```

## DisassociatedFaceTypeDef

```python
# DisassociatedFaceTypeDef definition

class DisassociatedFaceTypeDef(TypedDict):
    FaceId: NotRequired[str],
```

## UnsuccessfulFaceDisassociationTypeDef

```python
# UnsuccessfulFaceDisassociationTypeDef definition

class UnsuccessfulFaceDisassociationTypeDef(TypedDict):
    FaceId: NotRequired[str],
    UserId: NotRequired[str],
    Reasons: NotRequired[List[UnsuccessfulFaceDisassociationReasonType]],  # (1)
```

1. See [:material-code-brackets: UnsuccessfulFaceDisassociationReasonType](./literals.md#unsuccessfulfacedisassociationreasontype) 
## DistributeDatasetTypeDef

```python
# DistributeDatasetTypeDef definition

class DistributeDatasetTypeDef(TypedDict):
    Arn: str,
```

## EyeDirectionTypeDef

```python
# EyeDirectionTypeDef definition

class EyeDirectionTypeDef(TypedDict):
    Yaw: NotRequired[float],
    Pitch: NotRequired[float],
    Confidence: NotRequired[float],
```

## EyeOpenTypeDef

```python
# EyeOpenTypeDef definition

class EyeOpenTypeDef(TypedDict):
    Value: NotRequired[bool],
    Confidence: NotRequired[float],
```

## EyeglassesTypeDef

```python
# EyeglassesTypeDef definition

class EyeglassesTypeDef(TypedDict):
    Value: NotRequired[bool],
    Confidence: NotRequired[float],
```

## FaceOccludedTypeDef

```python
# FaceOccludedTypeDef definition

class FaceOccludedTypeDef(TypedDict):
    Value: NotRequired[bool],
    Confidence: NotRequired[float],
```

## GenderTypeDef

```python
# GenderTypeDef definition

class GenderTypeDef(TypedDict):
    Value: NotRequired[GenderTypeType],  # (1)
    Confidence: NotRequired[float],
```

1. See [:material-code-brackets: GenderTypeType](./literals.md#gendertypetype) 
## MouthOpenTypeDef

```python
# MouthOpenTypeDef definition

class MouthOpenTypeDef(TypedDict):
    Value: NotRequired[bool],
    Confidence: NotRequired[float],
```

## MustacheTypeDef

```python
# MustacheTypeDef definition

class MustacheTypeDef(TypedDict):
    Value: NotRequired[bool],
    Confidence: NotRequired[float],
```

## SunglassesTypeDef

```python
# SunglassesTypeDef definition

class SunglassesTypeDef(TypedDict):
    Value: NotRequired[bool],
    Confidence: NotRequired[float],
```

## FaceSearchSettingsTypeDef

```python
# FaceSearchSettingsTypeDef definition

class FaceSearchSettingsTypeDef(TypedDict):
    CollectionId: NotRequired[str],
    FaceMatchThreshold: NotRequired[float],
```

## PointTypeDef

```python
# PointTypeDef definition

class PointTypeDef(TypedDict):
    X: NotRequired[float],
    Y: NotRequired[float],
```

## GetCelebrityInfoRequestRequestTypeDef

```python
# GetCelebrityInfoRequestRequestTypeDef definition

class GetCelebrityInfoRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetCelebrityRecognitionRequestRequestTypeDef

```python
# GetCelebrityRecognitionRequestRequestTypeDef definition

class GetCelebrityRecognitionRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SortBy: NotRequired[CelebrityRecognitionSortByType],  # (1)
```

1. See [:material-code-brackets: CelebrityRecognitionSortByType](./literals.md#celebrityrecognitionsortbytype) 
## VideoMetadataTypeDef

```python
# VideoMetadataTypeDef definition

class VideoMetadataTypeDef(TypedDict):
    Codec: NotRequired[str],
    DurationMillis: NotRequired[int],
    Format: NotRequired[str],
    FrameRate: NotRequired[float],
    FrameHeight: NotRequired[int],
    FrameWidth: NotRequired[int],
    ColorRange: NotRequired[VideoColorRangeType],  # (1)
```

1. See [:material-code-brackets: VideoColorRangeType](./literals.md#videocolorrangetype) 
## GetContentModerationRequestMetadataTypeDef

```python
# GetContentModerationRequestMetadataTypeDef definition

class GetContentModerationRequestMetadataTypeDef(TypedDict):
    SortBy: NotRequired[ContentModerationSortByType],  # (1)
    AggregateBy: NotRequired[ContentModerationAggregateByType],  # (2)
```

1. See [:material-code-brackets: ContentModerationSortByType](./literals.md#contentmoderationsortbytype) 
2. See [:material-code-brackets: ContentModerationAggregateByType](./literals.md#contentmoderationaggregatebytype) 
## GetContentModerationRequestRequestTypeDef

```python
# GetContentModerationRequestRequestTypeDef definition

class GetContentModerationRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SortBy: NotRequired[ContentModerationSortByType],  # (1)
    AggregateBy: NotRequired[ContentModerationAggregateByType],  # (2)
```

1. See [:material-code-brackets: ContentModerationSortByType](./literals.md#contentmoderationsortbytype) 
2. See [:material-code-brackets: ContentModerationAggregateByType](./literals.md#contentmoderationaggregatebytype) 
## GetFaceDetectionRequestRequestTypeDef

```python
# GetFaceDetectionRequestRequestTypeDef definition

class GetFaceDetectionRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetFaceLivenessSessionResultsRequestRequestTypeDef

```python
# GetFaceLivenessSessionResultsRequestRequestTypeDef definition

class GetFaceLivenessSessionResultsRequestRequestTypeDef(TypedDict):
    SessionId: str,
```

## GetFaceSearchRequestRequestTypeDef

```python
# GetFaceSearchRequestRequestTypeDef definition

class GetFaceSearchRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SortBy: NotRequired[FaceSearchSortByType],  # (1)
```

1. See [:material-code-brackets: FaceSearchSortByType](./literals.md#facesearchsortbytype) 
## GetLabelDetectionRequestMetadataTypeDef

```python
# GetLabelDetectionRequestMetadataTypeDef definition

class GetLabelDetectionRequestMetadataTypeDef(TypedDict):
    SortBy: NotRequired[LabelDetectionSortByType],  # (1)
    AggregateBy: NotRequired[LabelDetectionAggregateByType],  # (2)
```

1. See [:material-code-brackets: LabelDetectionSortByType](./literals.md#labeldetectionsortbytype) 
2. See [:material-code-brackets: LabelDetectionAggregateByType](./literals.md#labeldetectionaggregatebytype) 
## GetLabelDetectionRequestRequestTypeDef

```python
# GetLabelDetectionRequestRequestTypeDef definition

class GetLabelDetectionRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SortBy: NotRequired[LabelDetectionSortByType],  # (1)
    AggregateBy: NotRequired[LabelDetectionAggregateByType],  # (2)
```

1. See [:material-code-brackets: LabelDetectionSortByType](./literals.md#labeldetectionsortbytype) 
2. See [:material-code-brackets: LabelDetectionAggregateByType](./literals.md#labeldetectionaggregatebytype) 
## GetMediaAnalysisJobRequestRequestTypeDef

```python
# GetMediaAnalysisJobRequestRequestTypeDef definition

class GetMediaAnalysisJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## MediaAnalysisJobFailureDetailsTypeDef

```python
# MediaAnalysisJobFailureDetailsTypeDef definition

class MediaAnalysisJobFailureDetailsTypeDef(TypedDict):
    Code: NotRequired[MediaAnalysisJobFailureCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: MediaAnalysisJobFailureCodeType](./literals.md#mediaanalysisjobfailurecodetype) 
## MediaAnalysisOutputConfigTypeDef

```python
# MediaAnalysisOutputConfigTypeDef definition

class MediaAnalysisOutputConfigTypeDef(TypedDict):
    S3Bucket: str,
    S3KeyPrefix: NotRequired[str],
```

## GetPersonTrackingRequestRequestTypeDef

```python
# GetPersonTrackingRequestRequestTypeDef definition

class GetPersonTrackingRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SortBy: NotRequired[PersonTrackingSortByType],  # (1)
```

1. See [:material-code-brackets: PersonTrackingSortByType](./literals.md#persontrackingsortbytype) 
## GetSegmentDetectionRequestRequestTypeDef

```python
# GetSegmentDetectionRequestRequestTypeDef definition

class GetSegmentDetectionRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## SegmentTypeInfoTypeDef

```python
# SegmentTypeInfoTypeDef definition

class SegmentTypeInfoTypeDef(TypedDict):
    Type: NotRequired[SegmentTypeType],  # (1)
    ModelVersion: NotRequired[str],
```

1. See [:material-code-brackets: SegmentTypeType](./literals.md#segmenttypetype) 
## GetTextDetectionRequestRequestTypeDef

```python
# GetTextDetectionRequestRequestTypeDef definition

class GetTextDetectionRequestRequestTypeDef(TypedDict):
    JobId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## HumanLoopDataAttributesTypeDef

```python
# HumanLoopDataAttributesTypeDef definition

class HumanLoopDataAttributesTypeDef(TypedDict):
    ContentClassifiers: NotRequired[Sequence[ContentClassifierType]],  # (1)
```

1. See [:material-code-brackets: ContentClassifierType](./literals.md#contentclassifiertype) 
## KinesisDataStreamTypeDef

```python
# KinesisDataStreamTypeDef definition

class KinesisDataStreamTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## KinesisVideoStreamStartSelectorTypeDef

```python
# KinesisVideoStreamStartSelectorTypeDef definition

class KinesisVideoStreamStartSelectorTypeDef(TypedDict):
    ProducerTimestamp: NotRequired[int],
    FragmentNumber: NotRequired[str],
```

## KinesisVideoStreamTypeDef

```python
# KinesisVideoStreamTypeDef definition

class KinesisVideoStreamTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## LabelAliasTypeDef

```python
# LabelAliasTypeDef definition

class LabelAliasTypeDef(TypedDict):
    Name: NotRequired[str],
```

## LabelCategoryTypeDef

```python
# LabelCategoryTypeDef definition

class LabelCategoryTypeDef(TypedDict):
    Name: NotRequired[str],
```

## ParentTypeDef

```python
# ParentTypeDef definition

class ParentTypeDef(TypedDict):
    Name: NotRequired[str],
```

## ListCollectionsRequestRequestTypeDef

```python
# ListCollectionsRequestRequestTypeDef definition

class ListCollectionsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDatasetEntriesRequestRequestTypeDef

```python
# ListDatasetEntriesRequestRequestTypeDef definition

class ListDatasetEntriesRequestRequestTypeDef(TypedDict):
    DatasetArn: str,
    ContainsLabels: NotRequired[Sequence[str]],
    Labeled: NotRequired[bool],
    SourceRefContains: NotRequired[str],
    HasErrors: NotRequired[bool],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDatasetLabelsRequestRequestTypeDef

```python
# ListDatasetLabelsRequestRequestTypeDef definition

class ListDatasetLabelsRequestRequestTypeDef(TypedDict):
    DatasetArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListFacesRequestRequestTypeDef

```python
# ListFacesRequestRequestTypeDef definition

class ListFacesRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    UserId: NotRequired[str],
    FaceIds: NotRequired[Sequence[str]],
```

## ListMediaAnalysisJobsRequestRequestTypeDef

```python
# ListMediaAnalysisJobsRequestRequestTypeDef definition

class ListMediaAnalysisJobsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListProjectPoliciesRequestRequestTypeDef

```python
# ListProjectPoliciesRequestRequestTypeDef definition

class ListProjectPoliciesRequestRequestTypeDef(TypedDict):
    ProjectArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ProjectPolicyTypeDef

```python
# ProjectPolicyTypeDef definition

class ProjectPolicyTypeDef(TypedDict):
    ProjectArn: NotRequired[str],
    PolicyName: NotRequired[str],
    PolicyRevisionId: NotRequired[str],
    PolicyDocument: NotRequired[str],
    CreationTimestamp: NotRequired[datetime],
    LastUpdatedTimestamp: NotRequired[datetime],
```

## ListStreamProcessorsRequestRequestTypeDef

```python
# ListStreamProcessorsRequestRequestTypeDef definition

class ListStreamProcessorsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## StreamProcessorTypeDef

```python
# StreamProcessorTypeDef definition

class StreamProcessorTypeDef(TypedDict):
    Name: NotRequired[str],
    Status: NotRequired[StreamProcessorStatusType],  # (1)
```

1. See [:material-code-brackets: StreamProcessorStatusType](./literals.md#streamprocessorstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListUsersRequestRequestTypeDef

```python
# ListUsersRequestRequestTypeDef definition

class ListUsersRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    UserId: NotRequired[str],
    UserStatus: NotRequired[UserStatusType],  # (1)
```

1. See [:material-code-brackets: UserStatusType](./literals.md#userstatustype) 
## MatchedUserTypeDef

```python
# MatchedUserTypeDef definition

class MatchedUserTypeDef(TypedDict):
    UserId: NotRequired[str],
    UserStatus: NotRequired[UserStatusType],  # (1)
```

1. See [:material-code-brackets: UserStatusType](./literals.md#userstatustype) 
## MediaAnalysisDetectModerationLabelsConfigTypeDef

```python
# MediaAnalysisDetectModerationLabelsConfigTypeDef definition

class MediaAnalysisDetectModerationLabelsConfigTypeDef(TypedDict):
    MinConfidence: NotRequired[float],
    ProjectVersion: NotRequired[str],
```

## MediaAnalysisModelVersionsTypeDef

```python
# MediaAnalysisModelVersionsTypeDef definition

class MediaAnalysisModelVersionsTypeDef(TypedDict):
    Moderation: NotRequired[str],
```

## NotificationChannelTypeDef

```python
# NotificationChannelTypeDef definition

class NotificationChannelTypeDef(TypedDict):
    SNSTopicArn: str,
    RoleArn: str,
```

## PutProjectPolicyRequestRequestTypeDef

```python
# PutProjectPolicyRequestRequestTypeDef definition

class PutProjectPolicyRequestRequestTypeDef(TypedDict):
    ProjectArn: str,
    PolicyName: str,
    PolicyDocument: str,
    PolicyRevisionId: NotRequired[str],
```

## S3DestinationTypeDef

```python
# S3DestinationTypeDef definition

class S3DestinationTypeDef(TypedDict):
    Bucket: NotRequired[str],
    KeyPrefix: NotRequired[str],
```

## SearchFacesRequestRequestTypeDef

```python
# SearchFacesRequestRequestTypeDef definition

class SearchFacesRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    FaceId: str,
    MaxFaces: NotRequired[int],
    FaceMatchThreshold: NotRequired[float],
```

## SearchUsersRequestRequestTypeDef

```python
# SearchUsersRequestRequestTypeDef definition

class SearchUsersRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    UserId: NotRequired[str],
    FaceId: NotRequired[str],
    UserMatchThreshold: NotRequired[float],
    MaxUsers: NotRequired[int],
```

## SearchedFaceTypeDef

```python
# SearchedFaceTypeDef definition

class SearchedFaceTypeDef(TypedDict):
    FaceId: NotRequired[str],
```

## SearchedUserTypeDef

```python
# SearchedUserTypeDef definition

class SearchedUserTypeDef(TypedDict):
    UserId: NotRequired[str],
```

## ShotSegmentTypeDef

```python
# ShotSegmentTypeDef definition

class ShotSegmentTypeDef(TypedDict):
    Index: NotRequired[int],
    Confidence: NotRequired[float],
```

## TechnicalCueSegmentTypeDef

```python
# TechnicalCueSegmentTypeDef definition

class TechnicalCueSegmentTypeDef(TypedDict):
    Type: NotRequired[TechnicalCueTypeType],  # (1)
    Confidence: NotRequired[float],
```

1. See [:material-code-brackets: TechnicalCueTypeType](./literals.md#technicalcuetypetype) 
## StartProjectVersionRequestRequestTypeDef

```python
# StartProjectVersionRequestRequestTypeDef definition

class StartProjectVersionRequestRequestTypeDef(TypedDict):
    ProjectVersionArn: str,
    MinInferenceUnits: int,
    MaxInferenceUnits: NotRequired[int],
```

## StartShotDetectionFilterTypeDef

```python
# StartShotDetectionFilterTypeDef definition

class StartShotDetectionFilterTypeDef(TypedDict):
    MinSegmentConfidence: NotRequired[float],
```

## StreamProcessingStopSelectorTypeDef

```python
# StreamProcessingStopSelectorTypeDef definition

class StreamProcessingStopSelectorTypeDef(TypedDict):
    MaxDurationInSeconds: NotRequired[int],
```

## StopProjectVersionRequestRequestTypeDef

```python
# StopProjectVersionRequestRequestTypeDef definition

class StopProjectVersionRequestRequestTypeDef(TypedDict):
    ProjectVersionArn: str,
```

## StopStreamProcessorRequestRequestTypeDef

```python
# StopStreamProcessorRequestRequestTypeDef definition

class StopStreamProcessorRequestRequestTypeDef(TypedDict):
    Name: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## CopyProjectVersionResponseTypeDef

```python
# CopyProjectVersionResponseTypeDef definition

class CopyProjectVersionResponseTypeDef(TypedDict):
    ProjectVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCollectionResponseTypeDef

```python
# CreateCollectionResponseTypeDef definition

class CreateCollectionResponseTypeDef(TypedDict):
    StatusCode: int,
    CollectionArn: str,
    FaceModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatasetResponseTypeDef

```python
# CreateDatasetResponseTypeDef definition

class CreateDatasetResponseTypeDef(TypedDict):
    DatasetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFaceLivenessSessionResponseTypeDef

```python
# CreateFaceLivenessSessionResponseTypeDef definition

class CreateFaceLivenessSessionResponseTypeDef(TypedDict):
    SessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectResponseTypeDef

```python
# CreateProjectResponseTypeDef definition

class CreateProjectResponseTypeDef(TypedDict):
    ProjectArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectVersionResponseTypeDef

```python
# CreateProjectVersionResponseTypeDef definition

class CreateProjectVersionResponseTypeDef(TypedDict):
    ProjectVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStreamProcessorResponseTypeDef

```python
# CreateStreamProcessorResponseTypeDef definition

class CreateStreamProcessorResponseTypeDef(TypedDict):
    StreamProcessorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCollectionResponseTypeDef

```python
# DeleteCollectionResponseTypeDef definition

class DeleteCollectionResponseTypeDef(TypedDict):
    StatusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProjectResponseTypeDef

```python
# DeleteProjectResponseTypeDef definition

class DeleteProjectResponseTypeDef(TypedDict):
    Status: ProjectStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProjectVersionResponseTypeDef

```python
# DeleteProjectVersionResponseTypeDef definition

class DeleteProjectVersionResponseTypeDef(TypedDict):
    Status: ProjectVersionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ProjectVersionStatusType](./literals.md#projectversionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCollectionResponseTypeDef

```python
# DescribeCollectionResponseTypeDef definition

class DescribeCollectionResponseTypeDef(TypedDict):
    FaceCount: int,
    FaceModelVersion: str,
    CollectionARN: str,
    CreationTimestamp: datetime,
    UserCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollectionsResponseTypeDef

```python
# ListCollectionsResponseTypeDef definition

class ListCollectionsResponseTypeDef(TypedDict):
    CollectionIds: List[str],
    FaceModelVersions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatasetEntriesResponseTypeDef

```python
# ListDatasetEntriesResponseTypeDef definition

class ListDatasetEntriesResponseTypeDef(TypedDict):
    DatasetEntries: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutProjectPolicyResponseTypeDef

```python
# PutProjectPolicyResponseTypeDef definition

class PutProjectPolicyResponseTypeDef(TypedDict):
    PolicyRevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCelebrityRecognitionResponseTypeDef

```python
# StartCelebrityRecognitionResponseTypeDef definition

class StartCelebrityRecognitionResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartContentModerationResponseTypeDef

```python
# StartContentModerationResponseTypeDef definition

class StartContentModerationResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartFaceDetectionResponseTypeDef

```python
# StartFaceDetectionResponseTypeDef definition

class StartFaceDetectionResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartFaceSearchResponseTypeDef

```python
# StartFaceSearchResponseTypeDef definition

class StartFaceSearchResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartLabelDetectionResponseTypeDef

```python
# StartLabelDetectionResponseTypeDef definition

class StartLabelDetectionResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMediaAnalysisJobResponseTypeDef

```python
# StartMediaAnalysisJobResponseTypeDef definition

class StartMediaAnalysisJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartPersonTrackingResponseTypeDef

```python
# StartPersonTrackingResponseTypeDef definition

class StartPersonTrackingResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartProjectVersionResponseTypeDef

```python
# StartProjectVersionResponseTypeDef definition

class StartProjectVersionResponseTypeDef(TypedDict):
    Status: ProjectVersionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ProjectVersionStatusType](./literals.md#projectversionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSegmentDetectionResponseTypeDef

```python
# StartSegmentDetectionResponseTypeDef definition

class StartSegmentDetectionResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartStreamProcessorResponseTypeDef

```python
# StartStreamProcessorResponseTypeDef definition

class StartStreamProcessorResponseTypeDef(TypedDict):
    SessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTextDetectionResponseTypeDef

```python
# StartTextDetectionResponseTypeDef definition

class StartTextDetectionResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopProjectVersionResponseTypeDef

```python
# StopProjectVersionResponseTypeDef definition

class StopProjectVersionResponseTypeDef(TypedDict):
    Status: ProjectVersionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ProjectVersionStatusType](./literals.md#projectversionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateFacesResponseTypeDef

```python
# AssociateFacesResponseTypeDef definition

class AssociateFacesResponseTypeDef(TypedDict):
    AssociatedFaces: List[AssociatedFaceTypeDef],  # (1)
    UnsuccessfulFaceAssociations: List[UnsuccessfulFaceAssociationTypeDef],  # (2)
    UserStatus: UserStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AssociatedFaceTypeDef](./type_defs.md#associatedfacetypedef) 
2. See [:material-code-braces: UnsuccessfulFaceAssociationTypeDef](./type_defs.md#unsuccessfulfaceassociationtypedef) 
3. See [:material-code-brackets: UserStatusType](./literals.md#userstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ComparedSourceImageFaceTypeDef

```python
# ComparedSourceImageFaceTypeDef definition

class ComparedSourceImageFaceTypeDef(TypedDict):
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (1)
    Confidence: NotRequired[float],
```

1. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
## FaceTypeDef

```python
# FaceTypeDef definition

class FaceTypeDef(TypedDict):
    FaceId: NotRequired[str],
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (1)
    ImageId: NotRequired[str],
    ExternalImageId: NotRequired[str],
    Confidence: NotRequired[float],
    IndexFacesModelVersion: NotRequired[str],
    UserId: NotRequired[str],
```

1. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
## AuditImageTypeDef

```python
# AuditImageTypeDef definition

class AuditImageTypeDef(TypedDict):
    Bytes: NotRequired[bytes],
    S3Object: NotRequired[S3ObjectTypeDef],  # (1)
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (2)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
2. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
## GroundTruthManifestTypeDef

```python
# GroundTruthManifestTypeDef definition

class GroundTruthManifestTypeDef(TypedDict):
    S3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## MediaAnalysisInputTypeDef

```python
# MediaAnalysisInputTypeDef definition

class MediaAnalysisInputTypeDef(TypedDict):
    S3Object: S3ObjectTypeDef,  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## MediaAnalysisManifestSummaryTypeDef

```python
# MediaAnalysisManifestSummaryTypeDef definition

class MediaAnalysisManifestSummaryTypeDef(TypedDict):
    S3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## SummaryTypeDef

```python
# SummaryTypeDef definition

class SummaryTypeDef(TypedDict):
    S3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## VideoTypeDef

```python
# VideoTypeDef definition

class VideoTypeDef(TypedDict):
    S3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## StartTechnicalCueDetectionFilterTypeDef

```python
# StartTechnicalCueDetectionFilterTypeDef definition

class StartTechnicalCueDetectionFilterTypeDef(TypedDict):
    MinSegmentConfidence: NotRequired[float],
    BlackFrame: NotRequired[BlackFrameTypeDef],  # (1)
```

1. See [:material-code-braces: BlackFrameTypeDef](./type_defs.md#blackframetypedef) 
## DatasetChangesTypeDef

```python
# DatasetChangesTypeDef definition

class DatasetChangesTypeDef(TypedDict):
    GroundTruth: BlobTypeDef,
```

## ImageTypeDef

```python
# ImageTypeDef definition

class ImageTypeDef(TypedDict):
    Bytes: NotRequired[BlobTypeDef],
    S3Object: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## GetCelebrityInfoResponseTypeDef

```python
# GetCelebrityInfoResponseTypeDef definition

class GetCelebrityInfoResponseTypeDef(TypedDict):
    Urls: List[str],
    Name: str,
    KnownGender: KnownGenderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnownGenderTypeDef](./type_defs.md#knowngendertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ComparedFaceTypeDef

```python
# ComparedFaceTypeDef definition

class ComparedFaceTypeDef(TypedDict):
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (1)
    Confidence: NotRequired[float],
    Landmarks: NotRequired[List[LandmarkTypeDef]],  # (2)
    Pose: NotRequired[PoseTypeDef],  # (3)
    Quality: NotRequired[ImageQualityTypeDef],  # (4)
    Emotions: NotRequired[List[EmotionTypeDef]],  # (5)
    Smile: NotRequired[SmileTypeDef],  # (6)
```

1. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
2. See [:material-code-braces: LandmarkTypeDef](./type_defs.md#landmarktypedef) 
3. See [:material-code-braces: PoseTypeDef](./type_defs.md#posetypedef) 
4. See [:material-code-braces: ImageQualityTypeDef](./type_defs.md#imagequalitytypedef) 
5. See [:material-code-braces: EmotionTypeDef](./type_defs.md#emotiontypedef) 
6. See [:material-code-braces: SmileTypeDef](./type_defs.md#smiletypedef) 
## StreamProcessorSettingsForUpdateTypeDef

```python
# StreamProcessorSettingsForUpdateTypeDef definition

class StreamProcessorSettingsForUpdateTypeDef(TypedDict):
    ConnectedHomeForUpdate: NotRequired[ConnectedHomeSettingsForUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: ConnectedHomeSettingsForUpdateTypeDef](./type_defs.md#connectedhomesettingsforupdatetypedef) 
## ContentModerationDetectionTypeDef

```python
# ContentModerationDetectionTypeDef definition

class ContentModerationDetectionTypeDef(TypedDict):
    Timestamp: NotRequired[int],
    ModerationLabel: NotRequired[ModerationLabelTypeDef],  # (1)
    StartTimestampMillis: NotRequired[int],
    EndTimestampMillis: NotRequired[int],
    DurationMillis: NotRequired[int],
    ContentTypes: NotRequired[List[ContentTypeTypeDef]],  # (2)
```

1. See [:material-code-braces: ModerationLabelTypeDef](./type_defs.md#moderationlabeltypedef) 
2. See [:material-code-braces: ContentTypeTypeDef](./type_defs.md#contenttypetypedef) 
## CopyProjectVersionRequestRequestTypeDef

```python
# CopyProjectVersionRequestRequestTypeDef definition

class CopyProjectVersionRequestRequestTypeDef(TypedDict):
    SourceProjectArn: str,
    SourceProjectVersionArn: str,
    DestinationProjectArn: str,
    VersionName: str,
    OutputConfig: OutputConfigTypeDef,  # (1)
    Tags: NotRequired[Mapping[str, str]],
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
## EquipmentDetectionTypeDef

```python
# EquipmentDetectionTypeDef definition

class EquipmentDetectionTypeDef(TypedDict):
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (1)
    Confidence: NotRequired[float],
    Type: NotRequired[ProtectiveEquipmentTypeType],  # (2)
    CoversBodyPart: NotRequired[CoversBodyPartTypeDef],  # (3)
```

1. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
2. See [:material-code-brackets: ProtectiveEquipmentTypeType](./literals.md#protectiveequipmenttypetype) 
3. See [:material-code-braces: CoversBodyPartTypeDef](./type_defs.md#coversbodyparttypedef) 
## CreateFaceLivenessSessionRequestSettingsTypeDef

```python
# CreateFaceLivenessSessionRequestSettingsTypeDef definition

class CreateFaceLivenessSessionRequestSettingsTypeDef(TypedDict):
    OutputConfig: NotRequired[LivenessOutputConfigTypeDef],  # (1)
    AuditImagesLimit: NotRequired[int],
```

1. See [:material-code-braces: LivenessOutputConfigTypeDef](./type_defs.md#livenessoutputconfigtypedef) 
## CustomizationFeatureConfigTypeDef

```python
# CustomizationFeatureConfigTypeDef definition

class CustomizationFeatureConfigTypeDef(TypedDict):
    ContentModeration: NotRequired[CustomizationFeatureContentModerationConfigTypeDef],  # (1)
```

1. See [:material-code-braces: CustomizationFeatureContentModerationConfigTypeDef](./type_defs.md#customizationfeaturecontentmoderationconfigtypedef) 
## DatasetDescriptionTypeDef

```python
# DatasetDescriptionTypeDef definition

class DatasetDescriptionTypeDef(TypedDict):
    CreationTimestamp: NotRequired[datetime],
    LastUpdatedTimestamp: NotRequired[datetime],
    Status: NotRequired[DatasetStatusType],  # (1)
    StatusMessage: NotRequired[str],
    StatusMessageCode: NotRequired[DatasetStatusMessageCodeType],  # (2)
    DatasetStats: NotRequired[DatasetStatsTypeDef],  # (3)
```

1. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
2. See [:material-code-brackets: DatasetStatusMessageCodeType](./literals.md#datasetstatusmessagecodetype) 
3. See [:material-code-braces: DatasetStatsTypeDef](./type_defs.md#datasetstatstypedef) 
## DatasetLabelDescriptionTypeDef

```python
# DatasetLabelDescriptionTypeDef definition

class DatasetLabelDescriptionTypeDef(TypedDict):
    LabelName: NotRequired[str],
    LabelStats: NotRequired[DatasetLabelStatsTypeDef],  # (1)
```

1. See [:material-code-braces: DatasetLabelStatsTypeDef](./type_defs.md#datasetlabelstatstypedef) 
## ProjectDescriptionTypeDef

```python
# ProjectDescriptionTypeDef definition

class ProjectDescriptionTypeDef(TypedDict):
    ProjectArn: NotRequired[str],
    CreationTimestamp: NotRequired[datetime],
    Status: NotRequired[ProjectStatusType],  # (1)
    Datasets: NotRequired[List[DatasetMetadataTypeDef]],  # (2)
    Feature: NotRequired[CustomizationFeatureType],  # (3)
    AutoUpdate: NotRequired[ProjectAutoUpdateType],  # (4)
```

1. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
2. See [:material-code-braces: DatasetMetadataTypeDef](./type_defs.md#datasetmetadatatypedef) 
3. See [:material-code-brackets: CustomizationFeatureType](./literals.md#customizationfeaturetype) 
4. See [:material-code-brackets: ProjectAutoUpdateType](./literals.md#projectautoupdatetype) 
## DeleteFacesResponseTypeDef

```python
# DeleteFacesResponseTypeDef definition

class DeleteFacesResponseTypeDef(TypedDict):
    DeletedFaces: List[str],
    UnsuccessfulFaceDeletions: List[UnsuccessfulFaceDeletionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnsuccessfulFaceDeletionTypeDef](./type_defs.md#unsuccessfulfacedeletiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProjectVersionsRequestPaginateTypeDef

```python
# DescribeProjectVersionsRequestPaginateTypeDef definition

class DescribeProjectVersionsRequestPaginateTypeDef(TypedDict):
    ProjectArn: str,
    VersionNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeProjectsRequestPaginateTypeDef

```python
# DescribeProjectsRequestPaginateTypeDef definition

class DescribeProjectsRequestPaginateTypeDef(TypedDict):
    ProjectNames: NotRequired[Sequence[str]],
    Features: NotRequired[Sequence[CustomizationFeatureType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: CustomizationFeatureType](./literals.md#customizationfeaturetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollectionsRequestPaginateTypeDef

```python
# ListCollectionsRequestPaginateTypeDef definition

class ListCollectionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatasetEntriesRequestPaginateTypeDef

```python
# ListDatasetEntriesRequestPaginateTypeDef definition

class ListDatasetEntriesRequestPaginateTypeDef(TypedDict):
    DatasetArn: str,
    ContainsLabels: NotRequired[Sequence[str]],
    Labeled: NotRequired[bool],
    SourceRefContains: NotRequired[str],
    HasErrors: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatasetLabelsRequestPaginateTypeDef

```python
# ListDatasetLabelsRequestPaginateTypeDef definition

class ListDatasetLabelsRequestPaginateTypeDef(TypedDict):
    DatasetArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFacesRequestPaginateTypeDef

```python
# ListFacesRequestPaginateTypeDef definition

class ListFacesRequestPaginateTypeDef(TypedDict):
    CollectionId: str,
    UserId: NotRequired[str],
    FaceIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectPoliciesRequestPaginateTypeDef

```python
# ListProjectPoliciesRequestPaginateTypeDef definition

class ListProjectPoliciesRequestPaginateTypeDef(TypedDict):
    ProjectArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStreamProcessorsRequestPaginateTypeDef

```python
# ListStreamProcessorsRequestPaginateTypeDef definition

class ListStreamProcessorsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsersRequestPaginateTypeDef

```python
# ListUsersRequestPaginateTypeDef definition

class ListUsersRequestPaginateTypeDef(TypedDict):
    CollectionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeProjectVersionsRequestWaitTypeDef

```python
# DescribeProjectVersionsRequestWaitTypeDef definition

class DescribeProjectVersionsRequestWaitTypeDef(TypedDict):
    ProjectArn: str,
    VersionNames: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DetectLabelsImageBackgroundTypeDef

```python
# DetectLabelsImageBackgroundTypeDef definition

class DetectLabelsImageBackgroundTypeDef(TypedDict):
    Quality: NotRequired[DetectLabelsImageQualityTypeDef],  # (1)
    DominantColors: NotRequired[List[DominantColorTypeDef]],  # (2)
```

1. See [:material-code-braces: DetectLabelsImageQualityTypeDef](./type_defs.md#detectlabelsimagequalitytypedef) 
2. See [:material-code-braces: DominantColorTypeDef](./type_defs.md#dominantcolortypedef) 
## DetectLabelsImageForegroundTypeDef

```python
# DetectLabelsImageForegroundTypeDef definition

class DetectLabelsImageForegroundTypeDef(TypedDict):
    Quality: NotRequired[DetectLabelsImageQualityTypeDef],  # (1)
    DominantColors: NotRequired[List[DominantColorTypeDef]],  # (2)
```

1. See [:material-code-braces: DetectLabelsImageQualityTypeDef](./type_defs.md#detectlabelsimagequalitytypedef) 
2. See [:material-code-braces: DominantColorTypeDef](./type_defs.md#dominantcolortypedef) 
## InstanceTypeDef

```python
# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (1)
    Confidence: NotRequired[float],
    DominantColors: NotRequired[List[DominantColorTypeDef]],  # (2)
```

1. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
2. See [:material-code-braces: DominantColorTypeDef](./type_defs.md#dominantcolortypedef) 
## DetectLabelsSettingsTypeDef

```python
# DetectLabelsSettingsTypeDef definition

class DetectLabelsSettingsTypeDef(TypedDict):
    GeneralLabels: NotRequired[GeneralLabelsSettingsTypeDef],  # (1)
    ImageProperties: NotRequired[DetectLabelsImagePropertiesSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: GeneralLabelsSettingsTypeDef](./type_defs.md#generallabelssettingstypedef) 
2. See [:material-code-braces: DetectLabelsImagePropertiesSettingsTypeDef](./type_defs.md#detectlabelsimagepropertiessettingstypedef) 
## LabelDetectionSettingsTypeDef

```python
# LabelDetectionSettingsTypeDef definition

class LabelDetectionSettingsTypeDef(TypedDict):
    GeneralLabels: NotRequired[GeneralLabelsSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: GeneralLabelsSettingsTypeDef](./type_defs.md#generallabelssettingstypedef) 
## DetectModerationLabelsResponseTypeDef

```python
# DetectModerationLabelsResponseTypeDef definition

class DetectModerationLabelsResponseTypeDef(TypedDict):
    ModerationLabels: List[ModerationLabelTypeDef],  # (1)
    ModerationModelVersion: str,
    HumanLoopActivationOutput: HumanLoopActivationOutputTypeDef,  # (2)
    ProjectVersion: str,
    ContentTypes: List[ContentTypeTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ModerationLabelTypeDef](./type_defs.md#moderationlabeltypedef) 
2. See [:material-code-braces: HumanLoopActivationOutputTypeDef](./type_defs.md#humanloopactivationoutputtypedef) 
3. See [:material-code-braces: ContentTypeTypeDef](./type_defs.md#contenttypetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateFacesResponseTypeDef

```python
# DisassociateFacesResponseTypeDef definition

class DisassociateFacesResponseTypeDef(TypedDict):
    DisassociatedFaces: List[DisassociatedFaceTypeDef],  # (1)
    UnsuccessfulFaceDisassociations: List[UnsuccessfulFaceDisassociationTypeDef],  # (2)
    UserStatus: UserStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DisassociatedFaceTypeDef](./type_defs.md#disassociatedfacetypedef) 
2. See [:material-code-braces: UnsuccessfulFaceDisassociationTypeDef](./type_defs.md#unsuccessfulfacedisassociationtypedef) 
3. See [:material-code-brackets: UserStatusType](./literals.md#userstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DistributeDatasetEntriesRequestRequestTypeDef

```python
# DistributeDatasetEntriesRequestRequestTypeDef definition

class DistributeDatasetEntriesRequestRequestTypeDef(TypedDict):
    Datasets: Sequence[DistributeDatasetTypeDef],  # (1)
```

1. See [:material-code-braces: DistributeDatasetTypeDef](./type_defs.md#distributedatasettypedef) 
## FaceDetailTypeDef

```python
# FaceDetailTypeDef definition

class FaceDetailTypeDef(TypedDict):
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (1)
    AgeRange: NotRequired[AgeRangeTypeDef],  # (2)
    Smile: NotRequired[SmileTypeDef],  # (3)
    Eyeglasses: NotRequired[EyeglassesTypeDef],  # (4)
    Sunglasses: NotRequired[SunglassesTypeDef],  # (5)
    Gender: NotRequired[GenderTypeDef],  # (6)
    Beard: NotRequired[BeardTypeDef],  # (7)
    Mustache: NotRequired[MustacheTypeDef],  # (8)
    EyesOpen: NotRequired[EyeOpenTypeDef],  # (9)
    MouthOpen: NotRequired[MouthOpenTypeDef],  # (10)
    Emotions: NotRequired[List[EmotionTypeDef]],  # (11)
    Landmarks: NotRequired[List[LandmarkTypeDef]],  # (12)
    Pose: NotRequired[PoseTypeDef],  # (13)
    Quality: NotRequired[ImageQualityTypeDef],  # (14)
    Confidence: NotRequired[float],
    FaceOccluded: NotRequired[FaceOccludedTypeDef],  # (15)
    EyeDirection: NotRequired[EyeDirectionTypeDef],  # (16)
```

1. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
2. See [:material-code-braces: AgeRangeTypeDef](./type_defs.md#agerangetypedef) 
3. See [:material-code-braces: SmileTypeDef](./type_defs.md#smiletypedef) 
4. See [:material-code-braces: EyeglassesTypeDef](./type_defs.md#eyeglassestypedef) 
5. See [:material-code-braces: SunglassesTypeDef](./type_defs.md#sunglassestypedef) 
6. See [:material-code-braces: GenderTypeDef](./type_defs.md#gendertypedef) 
7. See [:material-code-braces: BeardTypeDef](./type_defs.md#beardtypedef) 
8. See [:material-code-braces: MustacheTypeDef](./type_defs.md#mustachetypedef) 
9. See [:material-code-braces: EyeOpenTypeDef](./type_defs.md#eyeopentypedef) 
10. See [:material-code-braces: MouthOpenTypeDef](./type_defs.md#mouthopentypedef) 
11. See [:material-code-braces: EmotionTypeDef](./type_defs.md#emotiontypedef) 
12. See [:material-code-braces: LandmarkTypeDef](./type_defs.md#landmarktypedef) 
13. See [:material-code-braces: PoseTypeDef](./type_defs.md#posetypedef) 
14. See [:material-code-braces: ImageQualityTypeDef](./type_defs.md#imagequalitytypedef) 
15. See [:material-code-braces: FaceOccludedTypeDef](./type_defs.md#faceoccludedtypedef) 
16. See [:material-code-braces: EyeDirectionTypeDef](./type_defs.md#eyedirectiontypedef) 
## StreamProcessorSettingsOutputTypeDef

```python
# StreamProcessorSettingsOutputTypeDef definition

class StreamProcessorSettingsOutputTypeDef(TypedDict):
    FaceSearch: NotRequired[FaceSearchSettingsTypeDef],  # (1)
    ConnectedHome: NotRequired[ConnectedHomeSettingsOutputTypeDef],  # (2)
```

1. See [:material-code-braces: FaceSearchSettingsTypeDef](./type_defs.md#facesearchsettingstypedef) 
2. See [:material-code-braces: ConnectedHomeSettingsOutputTypeDef](./type_defs.md#connectedhomesettingsoutputtypedef) 
## GeometryTypeDef

```python
# GeometryTypeDef definition

class GeometryTypeDef(TypedDict):
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (1)
    Polygon: NotRequired[List[PointTypeDef]],  # (2)
```

1. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
2. See [:material-code-braces: PointTypeDef](./type_defs.md#pointtypedef) 
## RegionOfInterestOutputTypeDef

```python
# RegionOfInterestOutputTypeDef definition

class RegionOfInterestOutputTypeDef(TypedDict):
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (1)
    Polygon: NotRequired[List[PointTypeDef]],  # (2)
```

1. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
2. See [:material-code-braces: PointTypeDef](./type_defs.md#pointtypedef) 
## RegionOfInterestTypeDef

```python
# RegionOfInterestTypeDef definition

class RegionOfInterestTypeDef(TypedDict):
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (1)
    Polygon: NotRequired[Sequence[PointTypeDef]],  # (2)
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
## StreamProcessingStartSelectorTypeDef

```python
# StreamProcessingStartSelectorTypeDef definition

class StreamProcessingStartSelectorTypeDef(TypedDict):
    KVSStreamStartSelector: NotRequired[KinesisVideoStreamStartSelectorTypeDef],  # (1)
```

1. See [:material-code-braces: KinesisVideoStreamStartSelectorTypeDef](./type_defs.md#kinesisvideostreamstartselectortypedef) 
## StreamProcessorInputTypeDef

```python
# StreamProcessorInputTypeDef definition

class StreamProcessorInputTypeDef(TypedDict):
    KinesisVideoStream: NotRequired[KinesisVideoStreamTypeDef],  # (1)
```

1. See [:material-code-braces: KinesisVideoStreamTypeDef](./type_defs.md#kinesisvideostreamtypedef) 
## ListProjectPoliciesResponseTypeDef

```python
# ListProjectPoliciesResponseTypeDef definition

class ListProjectPoliciesResponseTypeDef(TypedDict):
    ProjectPolicies: List[ProjectPolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectPolicyTypeDef](./type_defs.md#projectpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStreamProcessorsResponseTypeDef

```python
# ListStreamProcessorsResponseTypeDef definition

class ListStreamProcessorsResponseTypeDef(TypedDict):
    StreamProcessors: List[StreamProcessorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StreamProcessorTypeDef](./type_defs.md#streamprocessortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersResponseTypeDef

```python
# ListUsersResponseTypeDef definition

class ListUsersResponseTypeDef(TypedDict):
    Users: List[UserTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UserMatchTypeDef

```python
# UserMatchTypeDef definition

class UserMatchTypeDef(TypedDict):
    Similarity: NotRequired[float],
    User: NotRequired[MatchedUserTypeDef],  # (1)
```

1. See [:material-code-braces: MatchedUserTypeDef](./type_defs.md#matchedusertypedef) 
## MediaAnalysisOperationsConfigTypeDef

```python
# MediaAnalysisOperationsConfigTypeDef definition

class MediaAnalysisOperationsConfigTypeDef(TypedDict):
    DetectModerationLabels: NotRequired[MediaAnalysisDetectModerationLabelsConfigTypeDef],  # (1)
```

1. See [:material-code-braces: MediaAnalysisDetectModerationLabelsConfigTypeDef](./type_defs.md#mediaanalysisdetectmoderationlabelsconfigtypedef) 
## MediaAnalysisResultsTypeDef

```python
# MediaAnalysisResultsTypeDef definition

class MediaAnalysisResultsTypeDef(TypedDict):
    S3Object: NotRequired[S3ObjectTypeDef],  # (1)
    ModelVersions: NotRequired[MediaAnalysisModelVersionsTypeDef],  # (2)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
2. See [:material-code-braces: MediaAnalysisModelVersionsTypeDef](./type_defs.md#mediaanalysismodelversionstypedef) 
## StreamProcessorOutputTypeDef

```python
# StreamProcessorOutputTypeDef definition

class StreamProcessorOutputTypeDef(TypedDict):
    KinesisDataStream: NotRequired[KinesisDataStreamTypeDef],  # (1)
    S3Destination: NotRequired[S3DestinationTypeDef],  # (2)
```

1. See [:material-code-braces: KinesisDataStreamTypeDef](./type_defs.md#kinesisdatastreamtypedef) 
2. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
## SegmentDetectionTypeDef

```python
# SegmentDetectionTypeDef definition

class SegmentDetectionTypeDef(TypedDict):
    Type: NotRequired[SegmentTypeType],  # (1)
    StartTimestampMillis: NotRequired[int],
    EndTimestampMillis: NotRequired[int],
    DurationMillis: NotRequired[int],
    StartTimecodeSMPTE: NotRequired[str],
    EndTimecodeSMPTE: NotRequired[str],
    DurationSMPTE: NotRequired[str],
    TechnicalCueSegment: NotRequired[TechnicalCueSegmentTypeDef],  # (2)
    ShotSegment: NotRequired[ShotSegmentTypeDef],  # (3)
    StartFrameNumber: NotRequired[int],
    EndFrameNumber: NotRequired[int],
    DurationFrames: NotRequired[int],
```

1. See [:material-code-brackets: SegmentTypeType](./literals.md#segmenttypetype) 
2. See [:material-code-braces: TechnicalCueSegmentTypeDef](./type_defs.md#technicalcuesegmenttypedef) 
3. See [:material-code-braces: ShotSegmentTypeDef](./type_defs.md#shotsegmenttypedef) 
## FaceMatchTypeDef

```python
# FaceMatchTypeDef definition

class FaceMatchTypeDef(TypedDict):
    Similarity: NotRequired[float],
    Face: NotRequired[FaceTypeDef],  # (1)
```

1. See [:material-code-braces: FaceTypeDef](./type_defs.md#facetypedef) 
## ListFacesResponseTypeDef

```python
# ListFacesResponseTypeDef definition

class ListFacesResponseTypeDef(TypedDict):
    Faces: List[FaceTypeDef],  # (1)
    FaceModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FaceTypeDef](./type_defs.md#facetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFaceLivenessSessionResultsResponseTypeDef

```python
# GetFaceLivenessSessionResultsResponseTypeDef definition

class GetFaceLivenessSessionResultsResponseTypeDef(TypedDict):
    SessionId: str,
    Status: LivenessSessionStatusType,  # (1)
    Confidence: float,
    ReferenceImage: AuditImageTypeDef,  # (2)
    AuditImages: List[AuditImageTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: LivenessSessionStatusType](./literals.md#livenesssessionstatustype) 
2. See [:material-code-braces: AuditImageTypeDef](./type_defs.md#auditimagetypedef) 
3. See [:material-code-braces: AuditImageTypeDef](./type_defs.md#auditimagetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetTypeDef

```python
# AssetTypeDef definition

class AssetTypeDef(TypedDict):
    GroundTruthManifest: NotRequired[GroundTruthManifestTypeDef],  # (1)
```

1. See [:material-code-braces: GroundTruthManifestTypeDef](./type_defs.md#groundtruthmanifesttypedef) 
## DatasetSourceTypeDef

```python
# DatasetSourceTypeDef definition

class DatasetSourceTypeDef(TypedDict):
    GroundTruthManifest: NotRequired[GroundTruthManifestTypeDef],  # (1)
    DatasetArn: NotRequired[str],
```

1. See [:material-code-braces: GroundTruthManifestTypeDef](./type_defs.md#groundtruthmanifesttypedef) 
## EvaluationResultTypeDef

```python
# EvaluationResultTypeDef definition

class EvaluationResultTypeDef(TypedDict):
    F1Score: NotRequired[float],
    Summary: NotRequired[SummaryTypeDef],  # (1)
```

1. See [:material-code-braces: SummaryTypeDef](./type_defs.md#summarytypedef) 
## StartCelebrityRecognitionRequestRequestTypeDef

```python
# StartCelebrityRecognitionRequestRequestTypeDef definition

class StartCelebrityRecognitionRequestRequestTypeDef(TypedDict):
    Video: VideoTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
    NotificationChannel: NotRequired[NotificationChannelTypeDef],  # (2)
    JobTag: NotRequired[str],
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
## StartContentModerationRequestRequestTypeDef

```python
# StartContentModerationRequestRequestTypeDef definition

class StartContentModerationRequestRequestTypeDef(TypedDict):
    Video: VideoTypeDef,  # (1)
    MinConfidence: NotRequired[float],
    ClientRequestToken: NotRequired[str],
    NotificationChannel: NotRequired[NotificationChannelTypeDef],  # (2)
    JobTag: NotRequired[str],
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
## StartFaceDetectionRequestRequestTypeDef

```python
# StartFaceDetectionRequestRequestTypeDef definition

class StartFaceDetectionRequestRequestTypeDef(TypedDict):
    Video: VideoTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
    NotificationChannel: NotRequired[NotificationChannelTypeDef],  # (2)
    FaceAttributes: NotRequired[FaceAttributesType],  # (3)
    JobTag: NotRequired[str],
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
3. See [:material-code-brackets: FaceAttributesType](./literals.md#faceattributestype) 
## StartFaceSearchRequestRequestTypeDef

```python
# StartFaceSearchRequestRequestTypeDef definition

class StartFaceSearchRequestRequestTypeDef(TypedDict):
    Video: VideoTypeDef,  # (1)
    CollectionId: str,
    ClientRequestToken: NotRequired[str],
    FaceMatchThreshold: NotRequired[float],
    NotificationChannel: NotRequired[NotificationChannelTypeDef],  # (2)
    JobTag: NotRequired[str],
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
## StartPersonTrackingRequestRequestTypeDef

```python
# StartPersonTrackingRequestRequestTypeDef definition

class StartPersonTrackingRequestRequestTypeDef(TypedDict):
    Video: VideoTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
    NotificationChannel: NotRequired[NotificationChannelTypeDef],  # (2)
    JobTag: NotRequired[str],
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
## StartSegmentDetectionFiltersTypeDef

```python
# StartSegmentDetectionFiltersTypeDef definition

class StartSegmentDetectionFiltersTypeDef(TypedDict):
    TechnicalCueFilter: NotRequired[StartTechnicalCueDetectionFilterTypeDef],  # (1)
    ShotFilter: NotRequired[StartShotDetectionFilterTypeDef],  # (2)
```

1. See [:material-code-braces: StartTechnicalCueDetectionFilterTypeDef](./type_defs.md#starttechnicalcuedetectionfiltertypedef) 
2. See [:material-code-braces: StartShotDetectionFilterTypeDef](./type_defs.md#startshotdetectionfiltertypedef) 
## UpdateDatasetEntriesRequestRequestTypeDef

```python
# UpdateDatasetEntriesRequestRequestTypeDef definition

class UpdateDatasetEntriesRequestRequestTypeDef(TypedDict):
    DatasetArn: str,
    Changes: DatasetChangesTypeDef,  # (1)
```

1. See [:material-code-braces: DatasetChangesTypeDef](./type_defs.md#datasetchangestypedef) 
## CompareFacesRequestRequestTypeDef

```python
# CompareFacesRequestRequestTypeDef definition

class CompareFacesRequestRequestTypeDef(TypedDict):
    SourceImage: ImageTypeDef,  # (1)
    TargetImage: ImageTypeDef,  # (1)
    SimilarityThreshold: NotRequired[float],
    QualityFilter: NotRequired[QualityFilterType],  # (3)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
3. See [:material-code-brackets: QualityFilterType](./literals.md#qualityfiltertype) 
## DetectCustomLabelsRequestRequestTypeDef

```python
# DetectCustomLabelsRequestRequestTypeDef definition

class DetectCustomLabelsRequestRequestTypeDef(TypedDict):
    ProjectVersionArn: str,
    Image: ImageTypeDef,  # (1)
    MaxResults: NotRequired[int],
    MinConfidence: NotRequired[float],
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
## DetectFacesRequestRequestTypeDef

```python
# DetectFacesRequestRequestTypeDef definition

class DetectFacesRequestRequestTypeDef(TypedDict):
    Image: ImageTypeDef,  # (1)
    Attributes: NotRequired[Sequence[AttributeType]],  # (2)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-brackets: AttributeType](./literals.md#attributetype) 
## DetectProtectiveEquipmentRequestRequestTypeDef

```python
# DetectProtectiveEquipmentRequestRequestTypeDef definition

class DetectProtectiveEquipmentRequestRequestTypeDef(TypedDict):
    Image: ImageTypeDef,  # (1)
    SummarizationAttributes: NotRequired[ProtectiveEquipmentSummarizationAttributesTypeDef],  # (2)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: ProtectiveEquipmentSummarizationAttributesTypeDef](./type_defs.md#protectiveequipmentsummarizationattributestypedef) 
## IndexFacesRequestRequestTypeDef

```python
# IndexFacesRequestRequestTypeDef definition

class IndexFacesRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    Image: ImageTypeDef,  # (1)
    ExternalImageId: NotRequired[str],
    DetectionAttributes: NotRequired[Sequence[AttributeType]],  # (2)
    MaxFaces: NotRequired[int],
    QualityFilter: NotRequired[QualityFilterType],  # (3)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-brackets: AttributeType](./literals.md#attributetype) 
3. See [:material-code-brackets: QualityFilterType](./literals.md#qualityfiltertype) 
## RecognizeCelebritiesRequestRequestTypeDef

```python
# RecognizeCelebritiesRequestRequestTypeDef definition

class RecognizeCelebritiesRequestRequestTypeDef(TypedDict):
    Image: ImageTypeDef,  # (1)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
## SearchFacesByImageRequestRequestTypeDef

```python
# SearchFacesByImageRequestRequestTypeDef definition

class SearchFacesByImageRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    Image: ImageTypeDef,  # (1)
    MaxFaces: NotRequired[int],
    FaceMatchThreshold: NotRequired[float],
    QualityFilter: NotRequired[QualityFilterType],  # (2)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-brackets: QualityFilterType](./literals.md#qualityfiltertype) 
## SearchUsersByImageRequestRequestTypeDef

```python
# SearchUsersByImageRequestRequestTypeDef definition

class SearchUsersByImageRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    Image: ImageTypeDef,  # (1)
    UserMatchThreshold: NotRequired[float],
    MaxUsers: NotRequired[int],
    QualityFilter: NotRequired[QualityFilterType],  # (2)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-brackets: QualityFilterType](./literals.md#qualityfiltertype) 
## CelebrityTypeDef

```python
# CelebrityTypeDef definition

class CelebrityTypeDef(TypedDict):
    Urls: NotRequired[List[str]],
    Name: NotRequired[str],
    Id: NotRequired[str],
    Face: NotRequired[ComparedFaceTypeDef],  # (1)
    MatchConfidence: NotRequired[float],
    KnownGender: NotRequired[KnownGenderTypeDef],  # (2)
```

1. See [:material-code-braces: ComparedFaceTypeDef](./type_defs.md#comparedfacetypedef) 
2. See [:material-code-braces: KnownGenderTypeDef](./type_defs.md#knowngendertypedef) 
## CompareFacesMatchTypeDef

```python
# CompareFacesMatchTypeDef definition

class CompareFacesMatchTypeDef(TypedDict):
    Similarity: NotRequired[float],
    Face: NotRequired[ComparedFaceTypeDef],  # (1)
```

1. See [:material-code-braces: ComparedFaceTypeDef](./type_defs.md#comparedfacetypedef) 
## StreamProcessorSettingsTypeDef

```python
# StreamProcessorSettingsTypeDef definition

class StreamProcessorSettingsTypeDef(TypedDict):
    FaceSearch: NotRequired[FaceSearchSettingsTypeDef],  # (1)
    ConnectedHome: NotRequired[ConnectedHomeSettingsUnionTypeDef],  # (2)
```

1. See [:material-code-braces: FaceSearchSettingsTypeDef](./type_defs.md#facesearchsettingstypedef) 
2. See [:material-code-braces: ConnectedHomeSettingsTypeDef](./type_defs.md#connectedhomesettingstypedef) [:material-code-braces: ConnectedHomeSettingsOutputTypeDef](./type_defs.md#connectedhomesettingsoutputtypedef) 
## GetContentModerationResponseTypeDef

```python
# GetContentModerationResponseTypeDef definition

class GetContentModerationResponseTypeDef(TypedDict):
    JobStatus: VideoJobStatusType,  # (1)
    StatusMessage: str,
    VideoMetadata: VideoMetadataTypeDef,  # (2)
    ModerationLabels: List[ContentModerationDetectionTypeDef],  # (3)
    ModerationModelVersion: str,
    JobId: str,
    Video: VideoTypeDef,  # (4)
    JobTag: str,
    GetRequestMetadata: GetContentModerationRequestMetadataTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: VideoJobStatusType](./literals.md#videojobstatustype) 
2. See [:material-code-braces: VideoMetadataTypeDef](./type_defs.md#videometadatatypedef) 
3. See [:material-code-braces: ContentModerationDetectionTypeDef](./type_defs.md#contentmoderationdetectiontypedef) 
4. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
5. See [:material-code-braces: GetContentModerationRequestMetadataTypeDef](./type_defs.md#getcontentmoderationrequestmetadatatypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProtectiveEquipmentBodyPartTypeDef

```python
# ProtectiveEquipmentBodyPartTypeDef definition

class ProtectiveEquipmentBodyPartTypeDef(TypedDict):
    Name: NotRequired[BodyPartType],  # (1)
    Confidence: NotRequired[float],
    EquipmentDetections: NotRequired[List[EquipmentDetectionTypeDef]],  # (2)
```

1. See [:material-code-brackets: BodyPartType](./literals.md#bodyparttype) 
2. See [:material-code-braces: EquipmentDetectionTypeDef](./type_defs.md#equipmentdetectiontypedef) 
## CreateFaceLivenessSessionRequestRequestTypeDef

```python
# CreateFaceLivenessSessionRequestRequestTypeDef definition

class CreateFaceLivenessSessionRequestRequestTypeDef(TypedDict):
    KmsKeyId: NotRequired[str],
    Settings: NotRequired[CreateFaceLivenessSessionRequestSettingsTypeDef],  # (1)
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: CreateFaceLivenessSessionRequestSettingsTypeDef](./type_defs.md#createfacelivenesssessionrequestsettingstypedef) 
## DescribeDatasetResponseTypeDef

```python
# DescribeDatasetResponseTypeDef definition

class DescribeDatasetResponseTypeDef(TypedDict):
    DatasetDescription: DatasetDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetDescriptionTypeDef](./type_defs.md#datasetdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatasetLabelsResponseTypeDef

```python
# ListDatasetLabelsResponseTypeDef definition

class ListDatasetLabelsResponseTypeDef(TypedDict):
    DatasetLabelDescriptions: List[DatasetLabelDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DatasetLabelDescriptionTypeDef](./type_defs.md#datasetlabeldescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProjectsResponseTypeDef

```python
# DescribeProjectsResponseTypeDef definition

class DescribeProjectsResponseTypeDef(TypedDict):
    ProjectDescriptions: List[ProjectDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectDescriptionTypeDef](./type_defs.md#projectdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectLabelsImagePropertiesTypeDef

```python
# DetectLabelsImagePropertiesTypeDef definition

class DetectLabelsImagePropertiesTypeDef(TypedDict):
    Quality: NotRequired[DetectLabelsImageQualityTypeDef],  # (1)
    DominantColors: NotRequired[List[DominantColorTypeDef]],  # (2)
    Foreground: NotRequired[DetectLabelsImageForegroundTypeDef],  # (3)
    Background: NotRequired[DetectLabelsImageBackgroundTypeDef],  # (4)
```

1. See [:material-code-braces: DetectLabelsImageQualityTypeDef](./type_defs.md#detectlabelsimagequalitytypedef) 
2. See [:material-code-braces: DominantColorTypeDef](./type_defs.md#dominantcolortypedef) 
3. See [:material-code-braces: DetectLabelsImageForegroundTypeDef](./type_defs.md#detectlabelsimageforegroundtypedef) 
4. See [:material-code-braces: DetectLabelsImageBackgroundTypeDef](./type_defs.md#detectlabelsimagebackgroundtypedef) 
## LabelTypeDef

```python
# LabelTypeDef definition

class LabelTypeDef(TypedDict):
    Name: NotRequired[str],
    Confidence: NotRequired[float],
    Instances: NotRequired[List[InstanceTypeDef]],  # (1)
    Parents: NotRequired[List[ParentTypeDef]],  # (2)
    Aliases: NotRequired[List[LabelAliasTypeDef]],  # (3)
    Categories: NotRequired[List[LabelCategoryTypeDef]],  # (4)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ParentTypeDef](./type_defs.md#parenttypedef) 
3. See [:material-code-braces: LabelAliasTypeDef](./type_defs.md#labelaliastypedef) 
4. See [:material-code-braces: LabelCategoryTypeDef](./type_defs.md#labelcategorytypedef) 
## DetectLabelsRequestRequestTypeDef

```python
# DetectLabelsRequestRequestTypeDef definition

class DetectLabelsRequestRequestTypeDef(TypedDict):
    Image: ImageTypeDef,  # (1)
    MaxLabels: NotRequired[int],
    MinConfidence: NotRequired[float],
    Features: NotRequired[Sequence[DetectLabelsFeatureNameType]],  # (2)
    Settings: NotRequired[DetectLabelsSettingsTypeDef],  # (3)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-brackets: DetectLabelsFeatureNameType](./literals.md#detectlabelsfeaturenametype) 
3. See [:material-code-braces: DetectLabelsSettingsTypeDef](./type_defs.md#detectlabelssettingstypedef) 
## StartLabelDetectionRequestRequestTypeDef

```python
# StartLabelDetectionRequestRequestTypeDef definition

class StartLabelDetectionRequestRequestTypeDef(TypedDict):
    Video: VideoTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
    MinConfidence: NotRequired[float],
    NotificationChannel: NotRequired[NotificationChannelTypeDef],  # (2)
    JobTag: NotRequired[str],
    Features: NotRequired[Sequence[LabelDetectionFeatureNameType]],  # (3)
    Settings: NotRequired[LabelDetectionSettingsTypeDef],  # (4)
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
3. See [:material-code-brackets: LabelDetectionFeatureNameType](./literals.md#labeldetectionfeaturenametype) 
4. See [:material-code-braces: LabelDetectionSettingsTypeDef](./type_defs.md#labeldetectionsettingstypedef) 
## CelebrityDetailTypeDef

```python
# CelebrityDetailTypeDef definition

class CelebrityDetailTypeDef(TypedDict):
    Urls: NotRequired[List[str]],
    Name: NotRequired[str],
    Id: NotRequired[str],
    Confidence: NotRequired[float],
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (1)
    Face: NotRequired[FaceDetailTypeDef],  # (2)
    KnownGender: NotRequired[KnownGenderTypeDef],  # (3)
```

1. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
2. See [:material-code-braces: FaceDetailTypeDef](./type_defs.md#facedetailtypedef) 
3. See [:material-code-braces: KnownGenderTypeDef](./type_defs.md#knowngendertypedef) 
## DetectFacesResponseTypeDef

```python
# DetectFacesResponseTypeDef definition

class DetectFacesResponseTypeDef(TypedDict):
    FaceDetails: List[FaceDetailTypeDef],  # (1)
    OrientationCorrection: OrientationCorrectionType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FaceDetailTypeDef](./type_defs.md#facedetailtypedef) 
2. See [:material-code-brackets: OrientationCorrectionType](./literals.md#orientationcorrectiontype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FaceDetectionTypeDef

```python
# FaceDetectionTypeDef definition

class FaceDetectionTypeDef(TypedDict):
    Timestamp: NotRequired[int],
    Face: NotRequired[FaceDetailTypeDef],  # (1)
```

1. See [:material-code-braces: FaceDetailTypeDef](./type_defs.md#facedetailtypedef) 
## FaceRecordTypeDef

```python
# FaceRecordTypeDef definition

class FaceRecordTypeDef(TypedDict):
    Face: NotRequired[FaceTypeDef],  # (1)
    FaceDetail: NotRequired[FaceDetailTypeDef],  # (2)
```

1. See [:material-code-braces: FaceTypeDef](./type_defs.md#facetypedef) 
2. See [:material-code-braces: FaceDetailTypeDef](./type_defs.md#facedetailtypedef) 
## PersonDetailTypeDef

```python
# PersonDetailTypeDef definition

class PersonDetailTypeDef(TypedDict):
    Index: NotRequired[int],
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (1)
    Face: NotRequired[FaceDetailTypeDef],  # (2)
```

1. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
2. See [:material-code-braces: FaceDetailTypeDef](./type_defs.md#facedetailtypedef) 
## SearchedFaceDetailsTypeDef

```python
# SearchedFaceDetailsTypeDef definition

class SearchedFaceDetailsTypeDef(TypedDict):
    FaceDetail: NotRequired[FaceDetailTypeDef],  # (1)
```

1. See [:material-code-braces: FaceDetailTypeDef](./type_defs.md#facedetailtypedef) 
## UnindexedFaceTypeDef

```python
# UnindexedFaceTypeDef definition

class UnindexedFaceTypeDef(TypedDict):
    Reasons: NotRequired[List[ReasonType]],  # (1)
    FaceDetail: NotRequired[FaceDetailTypeDef],  # (2)
```

1. See [:material-code-brackets: ReasonType](./literals.md#reasontype) 
2. See [:material-code-braces: FaceDetailTypeDef](./type_defs.md#facedetailtypedef) 
## UnsearchedFaceTypeDef

```python
# UnsearchedFaceTypeDef definition

class UnsearchedFaceTypeDef(TypedDict):
    FaceDetails: NotRequired[FaceDetailTypeDef],  # (1)
    Reasons: NotRequired[List[UnsearchedFaceReasonType]],  # (2)
```

1. See [:material-code-braces: FaceDetailTypeDef](./type_defs.md#facedetailtypedef) 
2. See [:material-code-brackets: UnsearchedFaceReasonType](./literals.md#unsearchedfacereasontype) 
## CustomLabelTypeDef

```python
# CustomLabelTypeDef definition

class CustomLabelTypeDef(TypedDict):
    Name: NotRequired[str],
    Confidence: NotRequired[float],
    Geometry: NotRequired[GeometryTypeDef],  # (1)
```

1. See [:material-code-braces: GeometryTypeDef](./type_defs.md#geometrytypedef) 
## TextDetectionTypeDef

```python
# TextDetectionTypeDef definition

class TextDetectionTypeDef(TypedDict):
    DetectedText: NotRequired[str],
    Type: NotRequired[TextTypesType],  # (1)
    Id: NotRequired[int],
    ParentId: NotRequired[int],
    Confidence: NotRequired[float],
    Geometry: NotRequired[GeometryTypeDef],  # (2)
```

1. See [:material-code-brackets: TextTypesType](./literals.md#texttypestype) 
2. See [:material-code-braces: GeometryTypeDef](./type_defs.md#geometrytypedef) 
## UpdateStreamProcessorRequestRequestTypeDef

```python
# UpdateStreamProcessorRequestRequestTypeDef definition

class UpdateStreamProcessorRequestRequestTypeDef(TypedDict):
    Name: str,
    SettingsForUpdate: NotRequired[StreamProcessorSettingsForUpdateTypeDef],  # (1)
    RegionsOfInterestForUpdate: NotRequired[Sequence[RegionOfInterestTypeDef]],  # (2)
    DataSharingPreferenceForUpdate: NotRequired[StreamProcessorDataSharingPreferenceTypeDef],  # (3)
    ParametersToDelete: NotRequired[Sequence[StreamProcessorParameterToDeleteType]],  # (4)
```

1. See [:material-code-braces: StreamProcessorSettingsForUpdateTypeDef](./type_defs.md#streamprocessorsettingsforupdatetypedef) 
2. See [:material-code-braces: RegionOfInterestTypeDef](./type_defs.md#regionofinteresttypedef) 
3. See [:material-code-braces: StreamProcessorDataSharingPreferenceTypeDef](./type_defs.md#streamprocessordatasharingpreferencetypedef) 
4. See [:material-code-brackets: StreamProcessorParameterToDeleteType](./literals.md#streamprocessorparametertodeletetype) 
## DetectModerationLabelsRequestRequestTypeDef

```python
# DetectModerationLabelsRequestRequestTypeDef definition

class DetectModerationLabelsRequestRequestTypeDef(TypedDict):
    Image: ImageTypeDef,  # (1)
    MinConfidence: NotRequired[float],
    HumanLoopConfig: NotRequired[HumanLoopConfigTypeDef],  # (2)
    ProjectVersion: NotRequired[str],
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: HumanLoopConfigTypeDef](./type_defs.md#humanloopconfigtypedef) 
## StartStreamProcessorRequestRequestTypeDef

```python
# StartStreamProcessorRequestRequestTypeDef definition

class StartStreamProcessorRequestRequestTypeDef(TypedDict):
    Name: str,
    StartSelector: NotRequired[StreamProcessingStartSelectorTypeDef],  # (1)
    StopSelector: NotRequired[StreamProcessingStopSelectorTypeDef],  # (2)
```

1. See [:material-code-braces: StreamProcessingStartSelectorTypeDef](./type_defs.md#streamprocessingstartselectortypedef) 
2. See [:material-code-braces: StreamProcessingStopSelectorTypeDef](./type_defs.md#streamprocessingstopselectortypedef) 
## SearchUsersResponseTypeDef

```python
# SearchUsersResponseTypeDef definition

class SearchUsersResponseTypeDef(TypedDict):
    UserMatches: List[UserMatchTypeDef],  # (1)
    FaceModelVersion: str,
    SearchedFace: SearchedFaceTypeDef,  # (2)
    SearchedUser: SearchedUserTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: UserMatchTypeDef](./type_defs.md#usermatchtypedef) 
2. See [:material-code-braces: SearchedFaceTypeDef](./type_defs.md#searchedfacetypedef) 
3. See [:material-code-braces: SearchedUserTypeDef](./type_defs.md#searchedusertypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMediaAnalysisJobRequestRequestTypeDef

```python
# StartMediaAnalysisJobRequestRequestTypeDef definition

class StartMediaAnalysisJobRequestRequestTypeDef(TypedDict):
    OperationsConfig: MediaAnalysisOperationsConfigTypeDef,  # (1)
    Input: MediaAnalysisInputTypeDef,  # (2)
    OutputConfig: MediaAnalysisOutputConfigTypeDef,  # (3)
    ClientRequestToken: NotRequired[str],
    JobName: NotRequired[str],
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-braces: MediaAnalysisOperationsConfigTypeDef](./type_defs.md#mediaanalysisoperationsconfigtypedef) 
2. See [:material-code-braces: MediaAnalysisInputTypeDef](./type_defs.md#mediaanalysisinputtypedef) 
3. See [:material-code-braces: MediaAnalysisOutputConfigTypeDef](./type_defs.md#mediaanalysisoutputconfigtypedef) 
## GetMediaAnalysisJobResponseTypeDef

```python
# GetMediaAnalysisJobResponseTypeDef definition

class GetMediaAnalysisJobResponseTypeDef(TypedDict):
    JobId: str,
    JobName: str,
    OperationsConfig: MediaAnalysisOperationsConfigTypeDef,  # (1)
    Status: MediaAnalysisJobStatusType,  # (2)
    FailureDetails: MediaAnalysisJobFailureDetailsTypeDef,  # (3)
    CreationTimestamp: datetime,
    CompletionTimestamp: datetime,
    Input: MediaAnalysisInputTypeDef,  # (4)
    OutputConfig: MediaAnalysisOutputConfigTypeDef,  # (5)
    KmsKeyId: str,
    Results: MediaAnalysisResultsTypeDef,  # (6)
    ManifestSummary: MediaAnalysisManifestSummaryTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: MediaAnalysisOperationsConfigTypeDef](./type_defs.md#mediaanalysisoperationsconfigtypedef) 
2. See [:material-code-brackets: MediaAnalysisJobStatusType](./literals.md#mediaanalysisjobstatustype) 
3. See [:material-code-braces: MediaAnalysisJobFailureDetailsTypeDef](./type_defs.md#mediaanalysisjobfailuredetailstypedef) 
4. See [:material-code-braces: MediaAnalysisInputTypeDef](./type_defs.md#mediaanalysisinputtypedef) 
5. See [:material-code-braces: MediaAnalysisOutputConfigTypeDef](./type_defs.md#mediaanalysisoutputconfigtypedef) 
6. See [:material-code-braces: MediaAnalysisResultsTypeDef](./type_defs.md#mediaanalysisresultstypedef) 
7. See [:material-code-braces: MediaAnalysisManifestSummaryTypeDef](./type_defs.md#mediaanalysismanifestsummarytypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MediaAnalysisJobDescriptionTypeDef

```python
# MediaAnalysisJobDescriptionTypeDef definition

class MediaAnalysisJobDescriptionTypeDef(TypedDict):
    JobId: str,
    OperationsConfig: MediaAnalysisOperationsConfigTypeDef,  # (1)
    Status: MediaAnalysisJobStatusType,  # (2)
    CreationTimestamp: datetime,
    Input: MediaAnalysisInputTypeDef,  # (4)
    OutputConfig: MediaAnalysisOutputConfigTypeDef,  # (5)
    JobName: NotRequired[str],
    FailureDetails: NotRequired[MediaAnalysisJobFailureDetailsTypeDef],  # (3)
    CompletionTimestamp: NotRequired[datetime],
    KmsKeyId: NotRequired[str],
    Results: NotRequired[MediaAnalysisResultsTypeDef],  # (6)
    ManifestSummary: NotRequired[MediaAnalysisManifestSummaryTypeDef],  # (7)
```

1. See [:material-code-braces: MediaAnalysisOperationsConfigTypeDef](./type_defs.md#mediaanalysisoperationsconfigtypedef) 
2. See [:material-code-brackets: MediaAnalysisJobStatusType](./literals.md#mediaanalysisjobstatustype) 
3. See [:material-code-braces: MediaAnalysisJobFailureDetailsTypeDef](./type_defs.md#mediaanalysisjobfailuredetailstypedef) 
4. See [:material-code-braces: MediaAnalysisInputTypeDef](./type_defs.md#mediaanalysisinputtypedef) 
5. See [:material-code-braces: MediaAnalysisOutputConfigTypeDef](./type_defs.md#mediaanalysisoutputconfigtypedef) 
6. See [:material-code-braces: MediaAnalysisResultsTypeDef](./type_defs.md#mediaanalysisresultstypedef) 
7. See [:material-code-braces: MediaAnalysisManifestSummaryTypeDef](./type_defs.md#mediaanalysismanifestsummarytypedef) 
## DescribeStreamProcessorResponseTypeDef

```python
# DescribeStreamProcessorResponseTypeDef definition

class DescribeStreamProcessorResponseTypeDef(TypedDict):
    Name: str,
    StreamProcessorArn: str,
    Status: StreamProcessorStatusType,  # (1)
    StatusMessage: str,
    CreationTimestamp: datetime,
    LastUpdateTimestamp: datetime,
    Input: StreamProcessorInputTypeDef,  # (2)
    Output: StreamProcessorOutputTypeDef,  # (3)
    RoleArn: str,
    Settings: StreamProcessorSettingsOutputTypeDef,  # (4)
    NotificationChannel: StreamProcessorNotificationChannelTypeDef,  # (5)
    KmsKeyId: str,
    RegionsOfInterest: List[RegionOfInterestOutputTypeDef],  # (6)
    DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: StreamProcessorStatusType](./literals.md#streamprocessorstatustype) 
2. See [:material-code-braces: StreamProcessorInputTypeDef](./type_defs.md#streamprocessorinputtypedef) 
3. See [:material-code-braces: StreamProcessorOutputTypeDef](./type_defs.md#streamprocessoroutputtypedef) 
4. See [:material-code-braces: StreamProcessorSettingsOutputTypeDef](./type_defs.md#streamprocessorsettingsoutputtypedef) 
5. See [:material-code-braces: StreamProcessorNotificationChannelTypeDef](./type_defs.md#streamprocessornotificationchanneltypedef) 
6. See [:material-code-braces: RegionOfInterestOutputTypeDef](./type_defs.md#regionofinterestoutputtypedef) 
7. See [:material-code-braces: StreamProcessorDataSharingPreferenceTypeDef](./type_defs.md#streamprocessordatasharingpreferencetypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSegmentDetectionResponseTypeDef

```python
# GetSegmentDetectionResponseTypeDef definition

class GetSegmentDetectionResponseTypeDef(TypedDict):
    JobStatus: VideoJobStatusType,  # (1)
    StatusMessage: str,
    VideoMetadata: List[VideoMetadataTypeDef],  # (2)
    AudioMetadata: List[AudioMetadataTypeDef],  # (3)
    Segments: List[SegmentDetectionTypeDef],  # (4)
    SelectedSegmentTypes: List[SegmentTypeInfoTypeDef],  # (5)
    JobId: str,
    Video: VideoTypeDef,  # (6)
    JobTag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: VideoJobStatusType](./literals.md#videojobstatustype) 
2. See [:material-code-braces: VideoMetadataTypeDef](./type_defs.md#videometadatatypedef) 
3. See [:material-code-braces: AudioMetadataTypeDef](./type_defs.md#audiometadatatypedef) 
4. See [:material-code-braces: SegmentDetectionTypeDef](./type_defs.md#segmentdetectiontypedef) 
5. See [:material-code-braces: SegmentTypeInfoTypeDef](./type_defs.md#segmenttypeinfotypedef) 
6. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchFacesByImageResponseTypeDef

```python
# SearchFacesByImageResponseTypeDef definition

class SearchFacesByImageResponseTypeDef(TypedDict):
    SearchedFaceBoundingBox: BoundingBoxTypeDef,  # (1)
    SearchedFaceConfidence: float,
    FaceMatches: List[FaceMatchTypeDef],  # (2)
    FaceModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
2. See [:material-code-braces: FaceMatchTypeDef](./type_defs.md#facematchtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchFacesResponseTypeDef

```python
# SearchFacesResponseTypeDef definition

class SearchFacesResponseTypeDef(TypedDict):
    SearchedFaceId: str,
    FaceMatches: List[FaceMatchTypeDef],  # (1)
    FaceModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FaceMatchTypeDef](./type_defs.md#facematchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestingDataOutputTypeDef

```python
# TestingDataOutputTypeDef definition

class TestingDataOutputTypeDef(TypedDict):
    Assets: NotRequired[List[AssetTypeDef]],  # (1)
    AutoCreate: NotRequired[bool],
```

1. See [:material-code-braces: AssetTypeDef](./type_defs.md#assettypedef) 
## TestingDataTypeDef

```python
# TestingDataTypeDef definition

class TestingDataTypeDef(TypedDict):
    Assets: NotRequired[Sequence[AssetTypeDef]],  # (1)
    AutoCreate: NotRequired[bool],
```

1. See [:material-code-braces: AssetTypeDef](./type_defs.md#assettypedef) 
## TrainingDataOutputTypeDef

```python
# TrainingDataOutputTypeDef definition

class TrainingDataOutputTypeDef(TypedDict):
    Assets: NotRequired[List[AssetTypeDef]],  # (1)
```

1. See [:material-code-braces: AssetTypeDef](./type_defs.md#assettypedef) 
## TrainingDataTypeDef

```python
# TrainingDataTypeDef definition

class TrainingDataTypeDef(TypedDict):
    Assets: NotRequired[Sequence[AssetTypeDef]],  # (1)
```

1. See [:material-code-braces: AssetTypeDef](./type_defs.md#assettypedef) 
## ValidationDataTypeDef

```python
# ValidationDataTypeDef definition

class ValidationDataTypeDef(TypedDict):
    Assets: NotRequired[List[AssetTypeDef]],  # (1)
```

1. See [:material-code-braces: AssetTypeDef](./type_defs.md#assettypedef) 
## CreateDatasetRequestRequestTypeDef

```python
# CreateDatasetRequestRequestTypeDef definition

class CreateDatasetRequestRequestTypeDef(TypedDict):
    DatasetType: DatasetTypeType,  # (1)
    ProjectArn: str,
    DatasetSource: NotRequired[DatasetSourceTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DatasetTypeType](./literals.md#datasettypetype) 
2. See [:material-code-braces: DatasetSourceTypeDef](./type_defs.md#datasetsourcetypedef) 
## StartSegmentDetectionRequestRequestTypeDef

```python
# StartSegmentDetectionRequestRequestTypeDef definition

class StartSegmentDetectionRequestRequestTypeDef(TypedDict):
    Video: VideoTypeDef,  # (1)
    SegmentTypes: Sequence[SegmentTypeType],  # (2)
    ClientRequestToken: NotRequired[str],
    NotificationChannel: NotRequired[NotificationChannelTypeDef],  # (3)
    JobTag: NotRequired[str],
    Filters: NotRequired[StartSegmentDetectionFiltersTypeDef],  # (4)
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
2. See [:material-code-brackets: SegmentTypeType](./literals.md#segmenttypetype) 
3. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
4. See [:material-code-braces: StartSegmentDetectionFiltersTypeDef](./type_defs.md#startsegmentdetectionfilterstypedef) 
## RecognizeCelebritiesResponseTypeDef

```python
# RecognizeCelebritiesResponseTypeDef definition

class RecognizeCelebritiesResponseTypeDef(TypedDict):
    CelebrityFaces: List[CelebrityTypeDef],  # (1)
    UnrecognizedFaces: List[ComparedFaceTypeDef],  # (2)
    OrientationCorrection: OrientationCorrectionType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: CelebrityTypeDef](./type_defs.md#celebritytypedef) 
2. See [:material-code-braces: ComparedFaceTypeDef](./type_defs.md#comparedfacetypedef) 
3. See [:material-code-brackets: OrientationCorrectionType](./literals.md#orientationcorrectiontype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CompareFacesResponseTypeDef

```python
# CompareFacesResponseTypeDef definition

class CompareFacesResponseTypeDef(TypedDict):
    SourceImageFace: ComparedSourceImageFaceTypeDef,  # (1)
    FaceMatches: List[CompareFacesMatchTypeDef],  # (2)
    UnmatchedFaces: List[ComparedFaceTypeDef],  # (3)
    SourceImageOrientationCorrection: OrientationCorrectionType,  # (4)
    TargetImageOrientationCorrection: OrientationCorrectionType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ComparedSourceImageFaceTypeDef](./type_defs.md#comparedsourceimagefacetypedef) 
2. See [:material-code-braces: CompareFacesMatchTypeDef](./type_defs.md#comparefacesmatchtypedef) 
3. See [:material-code-braces: ComparedFaceTypeDef](./type_defs.md#comparedfacetypedef) 
4. See [:material-code-brackets: OrientationCorrectionType](./literals.md#orientationcorrectiontype) 
5. See [:material-code-brackets: OrientationCorrectionType](./literals.md#orientationcorrectiontype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProtectiveEquipmentPersonTypeDef

```python
# ProtectiveEquipmentPersonTypeDef definition

class ProtectiveEquipmentPersonTypeDef(TypedDict):
    BodyParts: NotRequired[List[ProtectiveEquipmentBodyPartTypeDef]],  # (1)
    BoundingBox: NotRequired[BoundingBoxTypeDef],  # (2)
    Confidence: NotRequired[float],
    Id: NotRequired[int],
```

1. See [:material-code-braces: ProtectiveEquipmentBodyPartTypeDef](./type_defs.md#protectiveequipmentbodyparttypedef) 
2. See [:material-code-braces: BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef) 
## DetectLabelsResponseTypeDef

```python
# DetectLabelsResponseTypeDef definition

class DetectLabelsResponseTypeDef(TypedDict):
    Labels: List[LabelTypeDef],  # (1)
    OrientationCorrection: OrientationCorrectionType,  # (2)
    LabelModelVersion: str,
    ImageProperties: DetectLabelsImagePropertiesTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: LabelTypeDef](./type_defs.md#labeltypedef) 
2. See [:material-code-brackets: OrientationCorrectionType](./literals.md#orientationcorrectiontype) 
3. See [:material-code-braces: DetectLabelsImagePropertiesTypeDef](./type_defs.md#detectlabelsimagepropertiestypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LabelDetectionTypeDef

```python
# LabelDetectionTypeDef definition

class LabelDetectionTypeDef(TypedDict):
    Timestamp: NotRequired[int],
    Label: NotRequired[LabelTypeDef],  # (1)
    StartTimestampMillis: NotRequired[int],
    EndTimestampMillis: NotRequired[int],
    DurationMillis: NotRequired[int],
```

1. See [:material-code-braces: LabelTypeDef](./type_defs.md#labeltypedef) 
## CelebrityRecognitionTypeDef

```python
# CelebrityRecognitionTypeDef definition

class CelebrityRecognitionTypeDef(TypedDict):
    Timestamp: NotRequired[int],
    Celebrity: NotRequired[CelebrityDetailTypeDef],  # (1)
```

1. See [:material-code-braces: CelebrityDetailTypeDef](./type_defs.md#celebritydetailtypedef) 
## GetFaceDetectionResponseTypeDef

```python
# GetFaceDetectionResponseTypeDef definition

class GetFaceDetectionResponseTypeDef(TypedDict):
    JobStatus: VideoJobStatusType,  # (1)
    StatusMessage: str,
    VideoMetadata: VideoMetadataTypeDef,  # (2)
    Faces: List[FaceDetectionTypeDef],  # (3)
    JobId: str,
    Video: VideoTypeDef,  # (4)
    JobTag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: VideoJobStatusType](./literals.md#videojobstatustype) 
2. See [:material-code-braces: VideoMetadataTypeDef](./type_defs.md#videometadatatypedef) 
3. See [:material-code-braces: FaceDetectionTypeDef](./type_defs.md#facedetectiontypedef) 
4. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PersonDetectionTypeDef

```python
# PersonDetectionTypeDef definition

class PersonDetectionTypeDef(TypedDict):
    Timestamp: NotRequired[int],
    Person: NotRequired[PersonDetailTypeDef],  # (1)
```

1. See [:material-code-braces: PersonDetailTypeDef](./type_defs.md#persondetailtypedef) 
## PersonMatchTypeDef

```python
# PersonMatchTypeDef definition

class PersonMatchTypeDef(TypedDict):
    Timestamp: NotRequired[int],
    Person: NotRequired[PersonDetailTypeDef],  # (1)
    FaceMatches: NotRequired[List[FaceMatchTypeDef]],  # (2)
```

1. See [:material-code-braces: PersonDetailTypeDef](./type_defs.md#persondetailtypedef) 
2. See [:material-code-braces: FaceMatchTypeDef](./type_defs.md#facematchtypedef) 
## IndexFacesResponseTypeDef

```python
# IndexFacesResponseTypeDef definition

class IndexFacesResponseTypeDef(TypedDict):
    FaceRecords: List[FaceRecordTypeDef],  # (1)
    OrientationCorrection: OrientationCorrectionType,  # (2)
    FaceModelVersion: str,
    UnindexedFaces: List[UnindexedFaceTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: FaceRecordTypeDef](./type_defs.md#facerecordtypedef) 
2. See [:material-code-brackets: OrientationCorrectionType](./literals.md#orientationcorrectiontype) 
3. See [:material-code-braces: UnindexedFaceTypeDef](./type_defs.md#unindexedfacetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchUsersByImageResponseTypeDef

```python
# SearchUsersByImageResponseTypeDef definition

class SearchUsersByImageResponseTypeDef(TypedDict):
    UserMatches: List[UserMatchTypeDef],  # (1)
    FaceModelVersion: str,
    SearchedFace: SearchedFaceDetailsTypeDef,  # (2)
    UnsearchedFaces: List[UnsearchedFaceTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: UserMatchTypeDef](./type_defs.md#usermatchtypedef) 
2. See [:material-code-braces: SearchedFaceDetailsTypeDef](./type_defs.md#searchedfacedetailstypedef) 
3. See [:material-code-braces: UnsearchedFaceTypeDef](./type_defs.md#unsearchedfacetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectCustomLabelsResponseTypeDef

```python
# DetectCustomLabelsResponseTypeDef definition

class DetectCustomLabelsResponseTypeDef(TypedDict):
    CustomLabels: List[CustomLabelTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomLabelTypeDef](./type_defs.md#customlabeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectTextResponseTypeDef

```python
# DetectTextResponseTypeDef definition

class DetectTextResponseTypeDef(TypedDict):
    TextDetections: List[TextDetectionTypeDef],  # (1)
    TextModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TextDetectionTypeDef](./type_defs.md#textdetectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TextDetectionResultTypeDef

```python
# TextDetectionResultTypeDef definition

class TextDetectionResultTypeDef(TypedDict):
    Timestamp: NotRequired[int],
    TextDetection: NotRequired[TextDetectionTypeDef],  # (1)
```

1. See [:material-code-braces: TextDetectionTypeDef](./type_defs.md#textdetectiontypedef) 
## CreateStreamProcessorRequestRequestTypeDef

```python
# CreateStreamProcessorRequestRequestTypeDef definition

class CreateStreamProcessorRequestRequestTypeDef(TypedDict):
    Input: StreamProcessorInputTypeDef,  # (1)
    Output: StreamProcessorOutputTypeDef,  # (2)
    Name: str,
    Settings: StreamProcessorSettingsTypeDef,  # (3)
    RoleArn: str,
    Tags: NotRequired[Mapping[str, str]],
    NotificationChannel: NotRequired[StreamProcessorNotificationChannelTypeDef],  # (4)
    KmsKeyId: NotRequired[str],
    RegionsOfInterest: NotRequired[Sequence[RegionOfInterestUnionTypeDef]],  # (5)
    DataSharingPreference: NotRequired[StreamProcessorDataSharingPreferenceTypeDef],  # (6)
```

1. See [:material-code-braces: StreamProcessorInputTypeDef](./type_defs.md#streamprocessorinputtypedef) 
2. See [:material-code-braces: StreamProcessorOutputTypeDef](./type_defs.md#streamprocessoroutputtypedef) 
3. See [:material-code-braces: StreamProcessorSettingsTypeDef](./type_defs.md#streamprocessorsettingstypedef) 
4. See [:material-code-braces: StreamProcessorNotificationChannelTypeDef](./type_defs.md#streamprocessornotificationchanneltypedef) 
5. See [:material-code-braces: RegionOfInterestTypeDef](./type_defs.md#regionofinteresttypedef) [:material-code-braces: RegionOfInterestOutputTypeDef](./type_defs.md#regionofinterestoutputtypedef) 
6. See [:material-code-braces: StreamProcessorDataSharingPreferenceTypeDef](./type_defs.md#streamprocessordatasharingpreferencetypedef) 
## DetectTextFiltersTypeDef

```python
# DetectTextFiltersTypeDef definition

class DetectTextFiltersTypeDef(TypedDict):
    WordFilter: NotRequired[DetectionFilterTypeDef],  # (1)
    RegionsOfInterest: NotRequired[Sequence[RegionOfInterestUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: DetectionFilterTypeDef](./type_defs.md#detectionfiltertypedef) 
2. See [:material-code-braces: RegionOfInterestTypeDef](./type_defs.md#regionofinteresttypedef) [:material-code-braces: RegionOfInterestOutputTypeDef](./type_defs.md#regionofinterestoutputtypedef) 
## StartTextDetectionFiltersTypeDef

```python
# StartTextDetectionFiltersTypeDef definition

class StartTextDetectionFiltersTypeDef(TypedDict):
    WordFilter: NotRequired[DetectionFilterTypeDef],  # (1)
    RegionsOfInterest: NotRequired[Sequence[RegionOfInterestUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: DetectionFilterTypeDef](./type_defs.md#detectionfiltertypedef) 
2. See [:material-code-braces: RegionOfInterestTypeDef](./type_defs.md#regionofinteresttypedef) [:material-code-braces: RegionOfInterestOutputTypeDef](./type_defs.md#regionofinterestoutputtypedef) 
## ListMediaAnalysisJobsResponseTypeDef

```python
# ListMediaAnalysisJobsResponseTypeDef definition

class ListMediaAnalysisJobsResponseTypeDef(TypedDict):
    MediaAnalysisJobs: List[MediaAnalysisJobDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MediaAnalysisJobDescriptionTypeDef](./type_defs.md#mediaanalysisjobdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectVersionRequestRequestTypeDef

```python
# CreateProjectVersionRequestRequestTypeDef definition

class CreateProjectVersionRequestRequestTypeDef(TypedDict):
    ProjectArn: str,
    VersionName: str,
    OutputConfig: OutputConfigTypeDef,  # (1)
    TrainingData: NotRequired[TrainingDataTypeDef],  # (2)
    TestingData: NotRequired[TestingDataTypeDef],  # (3)
    Tags: NotRequired[Mapping[str, str]],
    KmsKeyId: NotRequired[str],
    VersionDescription: NotRequired[str],
    FeatureConfig: NotRequired[CustomizationFeatureConfigTypeDef],  # (4)
```

1. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
2. See [:material-code-braces: TrainingDataTypeDef](./type_defs.md#trainingdatatypedef) 
3. See [:material-code-braces: TestingDataTypeDef](./type_defs.md#testingdatatypedef) 
4. See [:material-code-braces: CustomizationFeatureConfigTypeDef](./type_defs.md#customizationfeatureconfigtypedef) 
## TestingDataResultTypeDef

```python
# TestingDataResultTypeDef definition

class TestingDataResultTypeDef(TypedDict):
    Input: NotRequired[TestingDataOutputTypeDef],  # (1)
    Output: NotRequired[TestingDataOutputTypeDef],  # (1)
    Validation: NotRequired[ValidationDataTypeDef],  # (3)
```

1. See [:material-code-braces: TestingDataOutputTypeDef](./type_defs.md#testingdataoutputtypedef) 
2. See [:material-code-braces: TestingDataOutputTypeDef](./type_defs.md#testingdataoutputtypedef) 
3. See [:material-code-braces: ValidationDataTypeDef](./type_defs.md#validationdatatypedef) 
## TrainingDataResultTypeDef

```python
# TrainingDataResultTypeDef definition

class TrainingDataResultTypeDef(TypedDict):
    Input: NotRequired[TrainingDataOutputTypeDef],  # (1)
    Output: NotRequired[TrainingDataOutputTypeDef],  # (1)
    Validation: NotRequired[ValidationDataTypeDef],  # (3)
```

1. See [:material-code-braces: TrainingDataOutputTypeDef](./type_defs.md#trainingdataoutputtypedef) 
2. See [:material-code-braces: TrainingDataOutputTypeDef](./type_defs.md#trainingdataoutputtypedef) 
3. See [:material-code-braces: ValidationDataTypeDef](./type_defs.md#validationdatatypedef) 
## DetectProtectiveEquipmentResponseTypeDef

```python
# DetectProtectiveEquipmentResponseTypeDef definition

class DetectProtectiveEquipmentResponseTypeDef(TypedDict):
    ProtectiveEquipmentModelVersion: str,
    Persons: List[ProtectiveEquipmentPersonTypeDef],  # (1)
    Summary: ProtectiveEquipmentSummaryTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProtectiveEquipmentPersonTypeDef](./type_defs.md#protectiveequipmentpersontypedef) 
2. See [:material-code-braces: ProtectiveEquipmentSummaryTypeDef](./type_defs.md#protectiveequipmentsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLabelDetectionResponseTypeDef

```python
# GetLabelDetectionResponseTypeDef definition

class GetLabelDetectionResponseTypeDef(TypedDict):
    JobStatus: VideoJobStatusType,  # (1)
    StatusMessage: str,
    VideoMetadata: VideoMetadataTypeDef,  # (2)
    Labels: List[LabelDetectionTypeDef],  # (3)
    LabelModelVersion: str,
    JobId: str,
    Video: VideoTypeDef,  # (4)
    JobTag: str,
    GetRequestMetadata: GetLabelDetectionRequestMetadataTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: VideoJobStatusType](./literals.md#videojobstatustype) 
2. See [:material-code-braces: VideoMetadataTypeDef](./type_defs.md#videometadatatypedef) 
3. See [:material-code-braces: LabelDetectionTypeDef](./type_defs.md#labeldetectiontypedef) 
4. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
5. See [:material-code-braces: GetLabelDetectionRequestMetadataTypeDef](./type_defs.md#getlabeldetectionrequestmetadatatypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCelebrityRecognitionResponseTypeDef

```python
# GetCelebrityRecognitionResponseTypeDef definition

class GetCelebrityRecognitionResponseTypeDef(TypedDict):
    JobStatus: VideoJobStatusType,  # (1)
    StatusMessage: str,
    VideoMetadata: VideoMetadataTypeDef,  # (2)
    Celebrities: List[CelebrityRecognitionTypeDef],  # (3)
    JobId: str,
    Video: VideoTypeDef,  # (4)
    JobTag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: VideoJobStatusType](./literals.md#videojobstatustype) 
2. See [:material-code-braces: VideoMetadataTypeDef](./type_defs.md#videometadatatypedef) 
3. See [:material-code-braces: CelebrityRecognitionTypeDef](./type_defs.md#celebrityrecognitiontypedef) 
4. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPersonTrackingResponseTypeDef

```python
# GetPersonTrackingResponseTypeDef definition

class GetPersonTrackingResponseTypeDef(TypedDict):
    JobStatus: VideoJobStatusType,  # (1)
    StatusMessage: str,
    VideoMetadata: VideoMetadataTypeDef,  # (2)
    Persons: List[PersonDetectionTypeDef],  # (3)
    JobId: str,
    Video: VideoTypeDef,  # (4)
    JobTag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: VideoJobStatusType](./literals.md#videojobstatustype) 
2. See [:material-code-braces: VideoMetadataTypeDef](./type_defs.md#videometadatatypedef) 
3. See [:material-code-braces: PersonDetectionTypeDef](./type_defs.md#persondetectiontypedef) 
4. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFaceSearchResponseTypeDef

```python
# GetFaceSearchResponseTypeDef definition

class GetFaceSearchResponseTypeDef(TypedDict):
    JobStatus: VideoJobStatusType,  # (1)
    StatusMessage: str,
    VideoMetadata: VideoMetadataTypeDef,  # (2)
    Persons: List[PersonMatchTypeDef],  # (3)
    JobId: str,
    Video: VideoTypeDef,  # (4)
    JobTag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: VideoJobStatusType](./literals.md#videojobstatustype) 
2. See [:material-code-braces: VideoMetadataTypeDef](./type_defs.md#videometadatatypedef) 
3. See [:material-code-braces: PersonMatchTypeDef](./type_defs.md#personmatchtypedef) 
4. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTextDetectionResponseTypeDef

```python
# GetTextDetectionResponseTypeDef definition

class GetTextDetectionResponseTypeDef(TypedDict):
    JobStatus: VideoJobStatusType,  # (1)
    StatusMessage: str,
    VideoMetadata: VideoMetadataTypeDef,  # (2)
    TextDetections: List[TextDetectionResultTypeDef],  # (3)
    TextModelVersion: str,
    JobId: str,
    Video: VideoTypeDef,  # (4)
    JobTag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: VideoJobStatusType](./literals.md#videojobstatustype) 
2. See [:material-code-braces: VideoMetadataTypeDef](./type_defs.md#videometadatatypedef) 
3. See [:material-code-braces: TextDetectionResultTypeDef](./type_defs.md#textdetectionresulttypedef) 
4. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectTextRequestRequestTypeDef

```python
# DetectTextRequestRequestTypeDef definition

class DetectTextRequestRequestTypeDef(TypedDict):
    Image: ImageTypeDef,  # (1)
    Filters: NotRequired[DetectTextFiltersTypeDef],  # (2)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: DetectTextFiltersTypeDef](./type_defs.md#detecttextfilterstypedef) 
## StartTextDetectionRequestRequestTypeDef

```python
# StartTextDetectionRequestRequestTypeDef definition

class StartTextDetectionRequestRequestTypeDef(TypedDict):
    Video: VideoTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
    NotificationChannel: NotRequired[NotificationChannelTypeDef],  # (2)
    JobTag: NotRequired[str],
    Filters: NotRequired[StartTextDetectionFiltersTypeDef],  # (3)
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
3. See [:material-code-braces: StartTextDetectionFiltersTypeDef](./type_defs.md#starttextdetectionfilterstypedef) 
## ProjectVersionDescriptionTypeDef

```python
# ProjectVersionDescriptionTypeDef definition

class ProjectVersionDescriptionTypeDef(TypedDict):
    ProjectVersionArn: NotRequired[str],
    CreationTimestamp: NotRequired[datetime],
    MinInferenceUnits: NotRequired[int],
    Status: NotRequired[ProjectVersionStatusType],  # (1)
    StatusMessage: NotRequired[str],
    BillableTrainingTimeInSeconds: NotRequired[int],
    TrainingEndTimestamp: NotRequired[datetime],
    OutputConfig: NotRequired[OutputConfigTypeDef],  # (2)
    TrainingDataResult: NotRequired[TrainingDataResultTypeDef],  # (3)
    TestingDataResult: NotRequired[TestingDataResultTypeDef],  # (4)
    EvaluationResult: NotRequired[EvaluationResultTypeDef],  # (5)
    ManifestSummary: NotRequired[GroundTruthManifestTypeDef],  # (6)
    KmsKeyId: NotRequired[str],
    MaxInferenceUnits: NotRequired[int],
    SourceProjectVersionArn: NotRequired[str],
    VersionDescription: NotRequired[str],
    Feature: NotRequired[CustomizationFeatureType],  # (7)
    BaseModelVersion: NotRequired[str],
    FeatureConfig: NotRequired[CustomizationFeatureConfigTypeDef],  # (8)
```

1. See [:material-code-brackets: ProjectVersionStatusType](./literals.md#projectversionstatustype) 
2. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
3. See [:material-code-braces: TrainingDataResultTypeDef](./type_defs.md#trainingdataresulttypedef) 
4. See [:material-code-braces: TestingDataResultTypeDef](./type_defs.md#testingdataresulttypedef) 
5. See [:material-code-braces: EvaluationResultTypeDef](./type_defs.md#evaluationresulttypedef) 
6. See [:material-code-braces: GroundTruthManifestTypeDef](./type_defs.md#groundtruthmanifesttypedef) 
7. See [:material-code-brackets: CustomizationFeatureType](./literals.md#customizationfeaturetype) 
8. See [:material-code-braces: CustomizationFeatureConfigTypeDef](./type_defs.md#customizationfeatureconfigtypedef) 
## DescribeProjectVersionsResponseTypeDef

```python
# DescribeProjectVersionsResponseTypeDef definition

class DescribeProjectVersionsResponseTypeDef(TypedDict):
    ProjectVersionDescriptions: List[ProjectVersionDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectVersionDescriptionTypeDef](./type_defs.md#projectversiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
