# ChimeSDKMediaPipelines module

> [Index](../README.md) > ChimeSDKMediaPipelines


!!! note ""

    Auto-generated documentation for [ChimeSDKMediaPipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
    type annotations stubs module [types-aiobotocore-chime-sdk-media-pipelines](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ChimeSDKMediaPipelines` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[chime-sdk-media-pipelines]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[chime-sdk-media-pipelines]'


# standalone installation
python -m pip install types-aiobotocore-chime-sdk-media-pipelines
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-chime-sdk-media-pipelines
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ChimeSDKMediaPipelinesClient

Type annotations and code completion for  `#!python session.create_client("chime-sdk-media-pipelines")` as [ChimeSDKMediaPipelinesClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client)

```python
# ChimeSDKMediaPipelinesClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_chime_sdk_media_pipelines.client import ChimeSDKMediaPipelinesClient


session = get_session()
async with session.create_client("chime-sdk-media-pipelines") as client:
    client: ChimeSDKMediaPipelinesClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActiveSpeakerPositionType usage example

from types_aiobotocore_chime_sdk_media_pipelines.literals import ActiveSpeakerPositionType

def get_value() -> ActiveSpeakerPositionType:
    return "BottomLeft"
```

- [ActiveSpeakerPositionType](./literals.md#activespeakerpositiontype)
- [ArtifactsConcatenationStateType](./literals.md#artifactsconcatenationstatetype)
- [ArtifactsStateType](./literals.md#artifactsstatetype)
- [AudioArtifactsConcatenationStateType](./literals.md#audioartifactsconcatenationstatetype)
- [AudioChannelsOptionType](./literals.md#audiochannelsoptiontype)
- [AudioMuxTypeType](./literals.md#audiomuxtypetype)
- [BorderColorType](./literals.md#bordercolortype)
- [CallAnalyticsLanguageCodeType](./literals.md#callanalyticslanguagecodetype)
- [CanvasOrientationType](./literals.md#canvasorientationtype)
- [ConcatenationSinkTypeType](./literals.md#concatenationsinktypetype)
- [ConcatenationSourceTypeType](./literals.md#concatenationsourcetypetype)
- [ContentMuxTypeType](./literals.md#contentmuxtypetype)
- [ContentRedactionOutputType](./literals.md#contentredactionoutputtype)
- [ContentShareLayoutOptionType](./literals.md#contentsharelayoutoptiontype)
- [ContentTypeType](./literals.md#contenttypetype)
- [FragmentSelectorTypeType](./literals.md#fragmentselectortypetype)
- [HighlightColorType](./literals.md#highlightcolortype)
- [HorizontalTilePositionType](./literals.md#horizontaltilepositiontype)
- [LayoutOptionType](./literals.md#layoutoptiontype)
- [LiveConnectorMuxTypeType](./literals.md#liveconnectormuxtypetype)
- [LiveConnectorSinkTypeType](./literals.md#liveconnectorsinktypetype)
- [LiveConnectorSourceTypeType](./literals.md#liveconnectorsourcetypetype)
- [MediaEncodingType](./literals.md#mediaencodingtype)
- [MediaInsightsPipelineConfigurationElementTypeType](./literals.md#mediainsightspipelineconfigurationelementtypetype)
- [MediaPipelineSinkTypeType](./literals.md#mediapipelinesinktypetype)
- [MediaPipelineSourceTypeType](./literals.md#mediapipelinesourcetypetype)
- [MediaPipelineStatusType](./literals.md#mediapipelinestatustype)
- [MediaPipelineStatusUpdateType](./literals.md#mediapipelinestatusupdatetype)
- [PartialResultsStabilityType](./literals.md#partialresultsstabilitytype)
- [ParticipantRoleType](./literals.md#participantroletype)
- [PresenterPositionType](./literals.md#presenterpositiontype)
- [RealTimeAlertRuleTypeType](./literals.md#realtimealertruletypetype)
- [RecordingFileFormatType](./literals.md#recordingfileformattype)
- [ResolutionOptionType](./literals.md#resolutionoptiontype)
- [SentimentTypeType](./literals.md#sentimenttypetype)
- [TileOrderType](./literals.md#tileordertype)
- [VerticalTilePositionType](./literals.md#verticaltilepositiontype)
- [VideoMuxTypeType](./literals.md#videomuxtypetype)
- [VocabularyFilterMethodType](./literals.md#vocabularyfiltermethodtype)
- [VoiceAnalyticsConfigurationStatusType](./literals.md#voiceanalyticsconfigurationstatustype)
- [ChimeSDKMediaPipelinesServiceName](./literals.md#chimesdkmediapipelinesservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActiveSpeakerOnlyConfigurationTypeDef](./type_defs.md#activespeakeronlyconfigurationtypedef)
- [PostCallAnalyticsSettingsTypeDef](./type_defs.md#postcallanalyticssettingstypedef)
- [AmazonTranscribeProcessorConfigurationTypeDef](./type_defs.md#amazontranscribeprocessorconfigurationtypedef)
- [AudioConcatenationConfigurationTypeDef](./type_defs.md#audioconcatenationconfigurationtypedef)
- [CompositedVideoConcatenationConfigurationTypeDef](./type_defs.md#compositedvideoconcatenationconfigurationtypedef)
- [ContentConcatenationConfigurationTypeDef](./type_defs.md#contentconcatenationconfigurationtypedef)
- [DataChannelConcatenationConfigurationTypeDef](./type_defs.md#datachannelconcatenationconfigurationtypedef)
- [MeetingEventsConcatenationConfigurationTypeDef](./type_defs.md#meetingeventsconcatenationconfigurationtypedef)
- [TranscriptionMessagesConcatenationConfigurationTypeDef](./type_defs.md#transcriptionmessagesconcatenationconfigurationtypedef)
- [VideoConcatenationConfigurationTypeDef](./type_defs.md#videoconcatenationconfigurationtypedef)
- [AudioArtifactsConfigurationTypeDef](./type_defs.md#audioartifactsconfigurationtypedef)
- [ContentArtifactsConfigurationTypeDef](./type_defs.md#contentartifactsconfigurationtypedef)
- [VideoArtifactsConfigurationTypeDef](./type_defs.md#videoartifactsconfigurationtypedef)
- [ChannelDefinitionTypeDef](./type_defs.md#channeldefinitiontypedef)
- [S3BucketSinkConfigurationTypeDef](./type_defs.md#s3bucketsinkconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [S3RecordingSinkRuntimeConfigurationTypeDef](./type_defs.md#s3recordingsinkruntimeconfigurationtypedef)
- [DeleteMediaCapturePipelineRequestRequestTypeDef](./type_defs.md#deletemediacapturepipelinerequestrequesttypedef)
- [DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef](./type_defs.md#deletemediainsightspipelineconfigurationrequestrequesttypedef)
- [DeleteMediaPipelineRequestRequestTypeDef](./type_defs.md#deletemediapipelinerequestrequesttypedef)
- [GetMediaCapturePipelineRequestRequestTypeDef](./type_defs.md#getmediacapturepipelinerequestrequesttypedef)
- [GetMediaInsightsPipelineConfigurationRequestRequestTypeDef](./type_defs.md#getmediainsightspipelineconfigurationrequestrequesttypedef)
- [GetMediaPipelineRequestRequestTypeDef](./type_defs.md#getmediapipelinerequestrequesttypedef)
- [HorizontalLayoutConfigurationTypeDef](./type_defs.md#horizontallayoutconfigurationtypedef)
- [PresenterOnlyConfigurationTypeDef](./type_defs.md#presenteronlyconfigurationtypedef)
- [VerticalLayoutConfigurationTypeDef](./type_defs.md#verticallayoutconfigurationtypedef)
- [VideoAttributeTypeDef](./type_defs.md#videoattributetypedef)
- [IssueDetectionConfigurationTypeDef](./type_defs.md#issuedetectionconfigurationtypedef)
- [KeywordMatchConfigurationTypeDef](./type_defs.md#keywordmatchconfigurationtypedef)
- [KinesisDataStreamSinkConfigurationTypeDef](./type_defs.md#kinesisdatastreamsinkconfigurationtypedef)
- [RecordingStreamConfigurationTypeDef](./type_defs.md#recordingstreamconfigurationtypedef)
- [LambdaFunctionSinkConfigurationTypeDef](./type_defs.md#lambdafunctionsinkconfigurationtypedef)
- [ListMediaCapturePipelinesRequestRequestTypeDef](./type_defs.md#listmediacapturepipelinesrequestrequesttypedef)
- [MediaCapturePipelineSummaryTypeDef](./type_defs.md#mediacapturepipelinesummarytypedef)
- [ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef](./type_defs.md#listmediainsightspipelineconfigurationsrequestrequesttypedef)
- [MediaInsightsPipelineConfigurationSummaryTypeDef](./type_defs.md#mediainsightspipelineconfigurationsummarytypedef)
- [ListMediaPipelinesRequestRequestTypeDef](./type_defs.md#listmediapipelinesrequestrequesttypedef)
- [MediaPipelineSummaryTypeDef](./type_defs.md#mediapipelinesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [LiveConnectorRTMPConfigurationTypeDef](./type_defs.md#liveconnectorrtmpconfigurationtypedef)
- [S3RecordingSinkConfigurationTypeDef](./type_defs.md#s3recordingsinkconfigurationtypedef)
- [SnsTopicSinkConfigurationTypeDef](./type_defs.md#snstopicsinkconfigurationtypedef)
- [SqsQueueSinkConfigurationTypeDef](./type_defs.md#sqsqueuesinkconfigurationtypedef)
- [VoiceAnalyticsProcessorConfigurationTypeDef](./type_defs.md#voiceanalyticsprocessorconfigurationtypedef)
- [SentimentConfigurationTypeDef](./type_defs.md#sentimentconfigurationtypedef)
- [SelectedVideoStreamsTypeDef](./type_defs.md#selectedvideostreamstypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateMediaInsightsPipelineStatusRequestRequestTypeDef](./type_defs.md#updatemediainsightspipelinestatusrequestrequesttypedef)
- [AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef](./type_defs.md#amazontranscribecallanalyticsprocessorconfigurationtypedef)
- [ArtifactsConcatenationConfigurationTypeDef](./type_defs.md#artifactsconcatenationconfigurationtypedef)
- [StreamChannelDefinitionTypeDef](./type_defs.md#streamchanneldefinitiontypedef)
- [ConcatenationSinkTypeDef](./type_defs.md#concatenationsinktypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [GridViewConfigurationTypeDef](./type_defs.md#gridviewconfigurationtypedef)
- [ListMediaCapturePipelinesResponseTypeDef](./type_defs.md#listmediacapturepipelinesresponsetypedef)
- [ListMediaInsightsPipelineConfigurationsResponseTypeDef](./type_defs.md#listmediainsightspipelineconfigurationsresponsetypedef)
- [ListMediaPipelinesResponseTypeDef](./type_defs.md#listmediapipelinesresponsetypedef)
- [LiveConnectorSinkConfigurationTypeDef](./type_defs.md#liveconnectorsinkconfigurationtypedef)
- [RealTimeAlertRuleTypeDef](./type_defs.md#realtimealertruletypedef)
- [SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef)
- [TimestampRangeTypeDef](./type_defs.md#timestamprangetypedef)
- [MediaInsightsPipelineConfigurationElementTypeDef](./type_defs.md#mediainsightspipelineconfigurationelementtypedef)
- [ChimeSdkMeetingConcatenationConfigurationTypeDef](./type_defs.md#chimesdkmeetingconcatenationconfigurationtypedef)
- [StreamConfigurationTypeDef](./type_defs.md#streamconfigurationtypedef)
- [CompositedVideoArtifactsConfigurationTypeDef](./type_defs.md#compositedvideoartifactsconfigurationtypedef)
- [RealTimeAlertConfigurationTypeDef](./type_defs.md#realtimealertconfigurationtypedef)
- [FragmentSelectorTypeDef](./type_defs.md#fragmentselectortypedef)
- [MediaCapturePipelineSourceConfigurationTypeDef](./type_defs.md#mediacapturepipelinesourceconfigurationtypedef)
- [KinesisVideoStreamSourceRuntimeConfigurationTypeDef](./type_defs.md#kinesisvideostreamsourceruntimeconfigurationtypedef)
- [ArtifactsConfigurationTypeDef](./type_defs.md#artifactsconfigurationtypedef)
- [ChimeSdkMeetingLiveConnectorConfigurationTypeDef](./type_defs.md#chimesdkmeetingliveconnectorconfigurationtypedef)
- [CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef](./type_defs.md#createmediainsightspipelineconfigurationrequestrequesttypedef)
- [MediaInsightsPipelineConfigurationTypeDef](./type_defs.md#mediainsightspipelineconfigurationtypedef)
- [UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef](./type_defs.md#updatemediainsightspipelineconfigurationrequestrequesttypedef)
- [KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef](./type_defs.md#kinesisvideostreamrecordingsourceruntimeconfigurationtypedef)
- [ConcatenationSourceTypeDef](./type_defs.md#concatenationsourcetypedef)
- [ChimeSdkMeetingConfigurationTypeDef](./type_defs.md#chimesdkmeetingconfigurationtypedef)
- [LiveConnectorSourceConfigurationTypeDef](./type_defs.md#liveconnectorsourceconfigurationtypedef)
- [CreateMediaInsightsPipelineConfigurationResponseTypeDef](./type_defs.md#createmediainsightspipelineconfigurationresponsetypedef)
- [GetMediaInsightsPipelineConfigurationResponseTypeDef](./type_defs.md#getmediainsightspipelineconfigurationresponsetypedef)
- [UpdateMediaInsightsPipelineConfigurationResponseTypeDef](./type_defs.md#updatemediainsightspipelineconfigurationresponsetypedef)
- [CreateMediaInsightsPipelineRequestRequestTypeDef](./type_defs.md#createmediainsightspipelinerequestrequesttypedef)
- [MediaInsightsPipelineTypeDef](./type_defs.md#mediainsightspipelinetypedef)
- [CreateMediaConcatenationPipelineRequestRequestTypeDef](./type_defs.md#createmediaconcatenationpipelinerequestrequesttypedef)
- [MediaConcatenationPipelineTypeDef](./type_defs.md#mediaconcatenationpipelinetypedef)
- [CreateMediaCapturePipelineRequestRequestTypeDef](./type_defs.md#createmediacapturepipelinerequestrequesttypedef)
- [MediaCapturePipelineTypeDef](./type_defs.md#mediacapturepipelinetypedef)
- [CreateMediaLiveConnectorPipelineRequestRequestTypeDef](./type_defs.md#createmedialiveconnectorpipelinerequestrequesttypedef)
- [MediaLiveConnectorPipelineTypeDef](./type_defs.md#medialiveconnectorpipelinetypedef)
- [CreateMediaInsightsPipelineResponseTypeDef](./type_defs.md#createmediainsightspipelineresponsetypedef)
- [CreateMediaConcatenationPipelineResponseTypeDef](./type_defs.md#createmediaconcatenationpipelineresponsetypedef)
- [CreateMediaCapturePipelineResponseTypeDef](./type_defs.md#createmediacapturepipelineresponsetypedef)
- [GetMediaCapturePipelineResponseTypeDef](./type_defs.md#getmediacapturepipelineresponsetypedef)
- [CreateMediaLiveConnectorPipelineResponseTypeDef](./type_defs.md#createmedialiveconnectorpipelineresponsetypedef)
- [MediaPipelineTypeDef](./type_defs.md#mediapipelinetypedef)
- [GetMediaPipelineResponseTypeDef](./type_defs.md#getmediapipelineresponsetypedef)

