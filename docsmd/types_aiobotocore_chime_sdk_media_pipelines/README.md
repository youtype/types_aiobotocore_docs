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
- [KinesisVideoStreamPoolStatusType](./literals.md#kinesisvideostreampoolstatustype)
- [LayoutOptionType](./literals.md#layoutoptiontype)
- [LiveConnectorMuxTypeType](./literals.md#liveconnectormuxtypetype)
- [LiveConnectorSinkTypeType](./literals.md#liveconnectorsinktypetype)
- [LiveConnectorSourceTypeType](./literals.md#liveconnectorsourcetypetype)
- [MediaEncodingType](./literals.md#mediaencodingtype)
- [MediaInsightsPipelineConfigurationElementTypeType](./literals.md#mediainsightspipelineconfigurationelementtypetype)
- [MediaPipelineElementStatusType](./literals.md#mediapipelineelementstatustype)
- [MediaPipelineSinkTypeType](./literals.md#mediapipelinesinktypetype)
- [MediaPipelineSourceTypeType](./literals.md#mediapipelinesourcetypetype)
- [MediaPipelineStatusType](./literals.md#mediapipelinestatustype)
- [MediaPipelineStatusUpdateType](./literals.md#mediapipelinestatusupdatetype)
- [MediaPipelineTaskStatusType](./literals.md#mediapipelinetaskstatustype)
- [MediaStreamPipelineSinkTypeType](./literals.md#mediastreampipelinesinktypetype)
- [MediaStreamTypeType](./literals.md#mediastreamtypetype)
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
- [VoiceAnalyticsLanguageCodeType](./literals.md#voiceanalyticslanguagecodetype)
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
- [KinesisVideoStreamConfigurationTypeDef](./type_defs.md#kinesisvideostreamconfigurationtypedef)
- [MediaStreamSinkTypeDef](./type_defs.md#mediastreamsinktypedef)
- [MediaStreamSourceTypeDef](./type_defs.md#mediastreamsourcetypedef)
- [DeleteMediaCapturePipelineRequestRequestTypeDef](./type_defs.md#deletemediacapturepipelinerequestrequesttypedef)
- [DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef](./type_defs.md#deletemediainsightspipelineconfigurationrequestrequesttypedef)
- [DeleteMediaPipelineKinesisVideoStreamPoolRequestRequestTypeDef](./type_defs.md#deletemediapipelinekinesisvideostreampoolrequestrequesttypedef)
- [DeleteMediaPipelineRequestRequestTypeDef](./type_defs.md#deletemediapipelinerequestrequesttypedef)
- [TimestampRangeOutputTypeDef](./type_defs.md#timestamprangeoutputtypedef)
- [GetMediaCapturePipelineRequestRequestTypeDef](./type_defs.md#getmediacapturepipelinerequestrequesttypedef)
- [GetMediaInsightsPipelineConfigurationRequestRequestTypeDef](./type_defs.md#getmediainsightspipelineconfigurationrequestrequesttypedef)
- [GetMediaPipelineKinesisVideoStreamPoolRequestRequestTypeDef](./type_defs.md#getmediapipelinekinesisvideostreampoolrequestrequesttypedef)
- [GetMediaPipelineRequestRequestTypeDef](./type_defs.md#getmediapipelinerequestrequesttypedef)
- [GetSpeakerSearchTaskRequestRequestTypeDef](./type_defs.md#getspeakersearchtaskrequestrequesttypedef)
- [SpeakerSearchTaskTypeDef](./type_defs.md#speakersearchtasktypedef)
- [GetVoiceToneAnalysisTaskRequestRequestTypeDef](./type_defs.md#getvoicetoneanalysistaskrequestrequesttypedef)
- [VoiceToneAnalysisTaskTypeDef](./type_defs.md#voicetoneanalysistasktypedef)
- [HorizontalLayoutConfigurationTypeDef](./type_defs.md#horizontallayoutconfigurationtypedef)
- [PresenterOnlyConfigurationTypeDef](./type_defs.md#presenteronlyconfigurationtypedef)
- [VerticalLayoutConfigurationTypeDef](./type_defs.md#verticallayoutconfigurationtypedef)
- [VideoAttributeTypeDef](./type_defs.md#videoattributetypedef)
- [IssueDetectionConfigurationTypeDef](./type_defs.md#issuedetectionconfigurationtypedef)
- [KeywordMatchConfigurationOutputTypeDef](./type_defs.md#keywordmatchconfigurationoutputtypedef)
- [KeywordMatchConfigurationTypeDef](./type_defs.md#keywordmatchconfigurationtypedef)
- [KinesisDataStreamSinkConfigurationTypeDef](./type_defs.md#kinesisdatastreamsinkconfigurationtypedef)
- [KinesisVideoStreamConfigurationUpdateTypeDef](./type_defs.md#kinesisvideostreamconfigurationupdatetypedef)
- [KinesisVideoStreamPoolSummaryTypeDef](./type_defs.md#kinesisvideostreampoolsummarytypedef)
- [RecordingStreamConfigurationTypeDef](./type_defs.md#recordingstreamconfigurationtypedef)
- [KinesisVideoStreamSourceTaskConfigurationTypeDef](./type_defs.md#kinesisvideostreamsourcetaskconfigurationtypedef)
- [LambdaFunctionSinkConfigurationTypeDef](./type_defs.md#lambdafunctionsinkconfigurationtypedef)
- [ListMediaCapturePipelinesRequestRequestTypeDef](./type_defs.md#listmediacapturepipelinesrequestrequesttypedef)
- [MediaCapturePipelineSummaryTypeDef](./type_defs.md#mediacapturepipelinesummarytypedef)
- [ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef](./type_defs.md#listmediainsightspipelineconfigurationsrequestrequesttypedef)
- [MediaInsightsPipelineConfigurationSummaryTypeDef](./type_defs.md#mediainsightspipelineconfigurationsummarytypedef)
- [ListMediaPipelineKinesisVideoStreamPoolsRequestRequestTypeDef](./type_defs.md#listmediapipelinekinesisvideostreampoolsrequestrequesttypedef)
- [ListMediaPipelinesRequestRequestTypeDef](./type_defs.md#listmediapipelinesrequestrequesttypedef)
- [MediaPipelineSummaryTypeDef](./type_defs.md#mediapipelinesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [LiveConnectorRTMPConfigurationTypeDef](./type_defs.md#liveconnectorrtmpconfigurationtypedef)
- [S3RecordingSinkConfigurationTypeDef](./type_defs.md#s3recordingsinkconfigurationtypedef)
- [SnsTopicSinkConfigurationTypeDef](./type_defs.md#snstopicsinkconfigurationtypedef)
- [SqsQueueSinkConfigurationTypeDef](./type_defs.md#sqsqueuesinkconfigurationtypedef)
- [VoiceAnalyticsProcessorConfigurationTypeDef](./type_defs.md#voiceanalyticsprocessorconfigurationtypedef)
- [VoiceEnhancementSinkConfigurationTypeDef](./type_defs.md#voiceenhancementsinkconfigurationtypedef)
- [MediaInsightsPipelineElementStatusTypeDef](./type_defs.md#mediainsightspipelineelementstatustypedef)
- [SentimentConfigurationTypeDef](./type_defs.md#sentimentconfigurationtypedef)
- [SelectedVideoStreamsOutputTypeDef](./type_defs.md#selectedvideostreamsoutputtypedef)
- [SelectedVideoStreamsTypeDef](./type_defs.md#selectedvideostreamstypedef)
- [StopSpeakerSearchTaskRequestRequestTypeDef](./type_defs.md#stopspeakersearchtaskrequestrequesttypedef)
- [StopVoiceToneAnalysisTaskRequestRequestTypeDef](./type_defs.md#stopvoicetoneanalysistaskrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateMediaInsightsPipelineStatusRequestRequestTypeDef](./type_defs.md#updatemediainsightspipelinestatusrequestrequesttypedef)
- [AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef](./type_defs.md#amazontranscribecallanalyticsprocessorconfigurationoutputtypedef)
- [AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef](./type_defs.md#amazontranscribecallanalyticsprocessorconfigurationtypedef)
- [ArtifactsConcatenationConfigurationTypeDef](./type_defs.md#artifactsconcatenationconfigurationtypedef)
- [StreamChannelDefinitionOutputTypeDef](./type_defs.md#streamchanneldefinitionoutputtypedef)
- [StreamChannelDefinitionTypeDef](./type_defs.md#streamchanneldefinitiontypedef)
- [ConcatenationSinkTypeDef](./type_defs.md#concatenationsinktypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CreateMediaPipelineKinesisVideoStreamPoolRequestRequestTypeDef](./type_defs.md#createmediapipelinekinesisvideostreampoolrequestrequesttypedef)
- [KinesisVideoStreamPoolConfigurationTypeDef](./type_defs.md#kinesisvideostreampoolconfigurationtypedef)
- [CreateMediaStreamPipelineRequestRequestTypeDef](./type_defs.md#createmediastreampipelinerequestrequesttypedef)
- [MediaStreamPipelineTypeDef](./type_defs.md#mediastreampipelinetypedef)
- [FragmentSelectorOutputTypeDef](./type_defs.md#fragmentselectoroutputtypedef)
- [GetSpeakerSearchTaskResponseTypeDef](./type_defs.md#getspeakersearchtaskresponsetypedef)
- [StartSpeakerSearchTaskResponseTypeDef](./type_defs.md#startspeakersearchtaskresponsetypedef)
- [GetVoiceToneAnalysisTaskResponseTypeDef](./type_defs.md#getvoicetoneanalysistaskresponsetypedef)
- [StartVoiceToneAnalysisTaskResponseTypeDef](./type_defs.md#startvoicetoneanalysistaskresponsetypedef)
- [GridViewConfigurationTypeDef](./type_defs.md#gridviewconfigurationtypedef)
- [KeywordMatchConfigurationUnionTypeDef](./type_defs.md#keywordmatchconfigurationuniontypedef)
- [UpdateMediaPipelineKinesisVideoStreamPoolRequestRequestTypeDef](./type_defs.md#updatemediapipelinekinesisvideostreampoolrequestrequesttypedef)
- [ListMediaPipelineKinesisVideoStreamPoolsResponseTypeDef](./type_defs.md#listmediapipelinekinesisvideostreampoolsresponsetypedef)
- [StartSpeakerSearchTaskRequestRequestTypeDef](./type_defs.md#startspeakersearchtaskrequestrequesttypedef)
- [StartVoiceToneAnalysisTaskRequestRequestTypeDef](./type_defs.md#startvoicetoneanalysistaskrequestrequesttypedef)
- [ListMediaCapturePipelinesResponseTypeDef](./type_defs.md#listmediacapturepipelinesresponsetypedef)
- [ListMediaInsightsPipelineConfigurationsResponseTypeDef](./type_defs.md#listmediainsightspipelineconfigurationsresponsetypedef)
- [ListMediaPipelinesResponseTypeDef](./type_defs.md#listmediapipelinesresponsetypedef)
- [LiveConnectorSinkConfigurationTypeDef](./type_defs.md#liveconnectorsinkconfigurationtypedef)
- [RealTimeAlertRuleOutputTypeDef](./type_defs.md#realtimealertruleoutputtypedef)
- [SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef)
- [SelectedVideoStreamsUnionTypeDef](./type_defs.md#selectedvideostreamsuniontypedef)
- [TimestampRangeTypeDef](./type_defs.md#timestamprangetypedef)
- [MediaInsightsPipelineConfigurationElementOutputTypeDef](./type_defs.md#mediainsightspipelineconfigurationelementoutputtypedef)
- [AmazonTranscribeCallAnalyticsProcessorConfigurationUnionTypeDef](./type_defs.md#amazontranscribecallanalyticsprocessorconfigurationuniontypedef)
- [ChimeSdkMeetingConcatenationConfigurationTypeDef](./type_defs.md#chimesdkmeetingconcatenationconfigurationtypedef)
- [StreamConfigurationOutputTypeDef](./type_defs.md#streamconfigurationoutputtypedef)
- [StreamChannelDefinitionUnionTypeDef](./type_defs.md#streamchanneldefinitionuniontypedef)
- [CreateMediaPipelineKinesisVideoStreamPoolResponseTypeDef](./type_defs.md#createmediapipelinekinesisvideostreampoolresponsetypedef)
- [GetMediaPipelineKinesisVideoStreamPoolResponseTypeDef](./type_defs.md#getmediapipelinekinesisvideostreampoolresponsetypedef)
- [UpdateMediaPipelineKinesisVideoStreamPoolResponseTypeDef](./type_defs.md#updatemediapipelinekinesisvideostreampoolresponsetypedef)
- [CreateMediaStreamPipelineResponseTypeDef](./type_defs.md#createmediastreampipelineresponsetypedef)
- [KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef](./type_defs.md#kinesisvideostreamrecordingsourceruntimeconfigurationoutputtypedef)
- [CompositedVideoArtifactsConfigurationTypeDef](./type_defs.md#compositedvideoartifactsconfigurationtypedef)
- [RealTimeAlertRuleTypeDef](./type_defs.md#realtimealertruletypedef)
- [RealTimeAlertConfigurationOutputTypeDef](./type_defs.md#realtimealertconfigurationoutputtypedef)
- [SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef)
- [TimestampRangeUnionTypeDef](./type_defs.md#timestamprangeuniontypedef)
- [MediaInsightsPipelineConfigurationElementTypeDef](./type_defs.md#mediainsightspipelineconfigurationelementtypedef)
- [MediaCapturePipelineSourceConfigurationTypeDef](./type_defs.md#mediacapturepipelinesourceconfigurationtypedef)
- [KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef](./type_defs.md#kinesisvideostreamsourceruntimeconfigurationoutputtypedef)
- [StreamConfigurationTypeDef](./type_defs.md#streamconfigurationtypedef)
- [ArtifactsConfigurationTypeDef](./type_defs.md#artifactsconfigurationtypedef)
- [ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef](./type_defs.md#chimesdkmeetingliveconnectorconfigurationoutputtypedef)
- [RealTimeAlertRuleUnionTypeDef](./type_defs.md#realtimealertruleuniontypedef)
- [MediaInsightsPipelineConfigurationTypeDef](./type_defs.md#mediainsightspipelineconfigurationtypedef)
- [SourceConfigurationUnionTypeDef](./type_defs.md#sourceconfigurationuniontypedef)
- [FragmentSelectorTypeDef](./type_defs.md#fragmentselectortypedef)
- [MediaInsightsPipelineConfigurationElementUnionTypeDef](./type_defs.md#mediainsightspipelineconfigurationelementuniontypedef)
- [ConcatenationSourceTypeDef](./type_defs.md#concatenationsourcetypedef)
- [MediaInsightsPipelineTypeDef](./type_defs.md#mediainsightspipelinetypedef)
- [StreamConfigurationUnionTypeDef](./type_defs.md#streamconfigurationuniontypedef)
- [ChimeSdkMeetingConfigurationOutputTypeDef](./type_defs.md#chimesdkmeetingconfigurationoutputtypedef)
- [LiveConnectorSourceConfigurationOutputTypeDef](./type_defs.md#liveconnectorsourceconfigurationoutputtypedef)
- [RealTimeAlertConfigurationTypeDef](./type_defs.md#realtimealertconfigurationtypedef)
- [CreateMediaInsightsPipelineConfigurationResponseTypeDef](./type_defs.md#createmediainsightspipelineconfigurationresponsetypedef)
- [GetMediaInsightsPipelineConfigurationResponseTypeDef](./type_defs.md#getmediainsightspipelineconfigurationresponsetypedef)
- [UpdateMediaInsightsPipelineConfigurationResponseTypeDef](./type_defs.md#updatemediainsightspipelineconfigurationresponsetypedef)
- [ChimeSdkMeetingConfigurationTypeDef](./type_defs.md#chimesdkmeetingconfigurationtypedef)
- [ChimeSdkMeetingLiveConnectorConfigurationTypeDef](./type_defs.md#chimesdkmeetingliveconnectorconfigurationtypedef)
- [FragmentSelectorUnionTypeDef](./type_defs.md#fragmentselectoruniontypedef)
- [CreateMediaConcatenationPipelineRequestRequestTypeDef](./type_defs.md#createmediaconcatenationpipelinerequestrequesttypedef)
- [MediaConcatenationPipelineTypeDef](./type_defs.md#mediaconcatenationpipelinetypedef)
- [CreateMediaInsightsPipelineResponseTypeDef](./type_defs.md#createmediainsightspipelineresponsetypedef)
- [KinesisVideoStreamSourceRuntimeConfigurationTypeDef](./type_defs.md#kinesisvideostreamsourceruntimeconfigurationtypedef)
- [MediaCapturePipelineTypeDef](./type_defs.md#mediacapturepipelinetypedef)
- [MediaLiveConnectorPipelineTypeDef](./type_defs.md#medialiveconnectorpipelinetypedef)
- [CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef](./type_defs.md#createmediainsightspipelineconfigurationrequestrequesttypedef)
- [UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef](./type_defs.md#updatemediainsightspipelineconfigurationrequestrequesttypedef)
- [CreateMediaCapturePipelineRequestRequestTypeDef](./type_defs.md#createmediacapturepipelinerequestrequesttypedef)
- [ChimeSdkMeetingLiveConnectorConfigurationUnionTypeDef](./type_defs.md#chimesdkmeetingliveconnectorconfigurationuniontypedef)
- [KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef](./type_defs.md#kinesisvideostreamrecordingsourceruntimeconfigurationtypedef)
- [CreateMediaConcatenationPipelineResponseTypeDef](./type_defs.md#createmediaconcatenationpipelineresponsetypedef)
- [CreateMediaCapturePipelineResponseTypeDef](./type_defs.md#createmediacapturepipelineresponsetypedef)
- [GetMediaCapturePipelineResponseTypeDef](./type_defs.md#getmediacapturepipelineresponsetypedef)
- [CreateMediaLiveConnectorPipelineResponseTypeDef](./type_defs.md#createmedialiveconnectorpipelineresponsetypedef)
- [MediaPipelineTypeDef](./type_defs.md#mediapipelinetypedef)
- [LiveConnectorSourceConfigurationTypeDef](./type_defs.md#liveconnectorsourceconfigurationtypedef)
- [CreateMediaInsightsPipelineRequestRequestTypeDef](./type_defs.md#createmediainsightspipelinerequestrequesttypedef)
- [GetMediaPipelineResponseTypeDef](./type_defs.md#getmediapipelineresponsetypedef)
- [LiveConnectorSourceConfigurationUnionTypeDef](./type_defs.md#liveconnectorsourceconfigurationuniontypedef)
- [CreateMediaLiveConnectorPipelineRequestRequestTypeDef](./type_defs.md#createmedialiveconnectorpipelinerequestrequesttypedef)

