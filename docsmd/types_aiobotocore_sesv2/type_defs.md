# Type definitions

> [Index](../README.md) > [SESV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SESV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#sesv2)
    type annotations stubs module [types-aiobotocore-sesv2](https://pypi.org/project/types-aiobotocore-sesv2/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


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


## InboxPlacementTrackingOptionUnionTypeDef

```python
# InboxPlacementTrackingOptionUnionTypeDef definition

InboxPlacementTrackingOptionUnionTypeDef = Union[
    InboxPlacementTrackingOptionTypeDef,  # (1)
    InboxPlacementTrackingOptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InboxPlacementTrackingOptionTypeDef](./type_defs.md#inboxplacementtrackingoptiontypedef) 
2. See [:material-code-braces: InboxPlacementTrackingOptionOutputTypeDef](./type_defs.md#inboxplacementtrackingoptionoutputtypedef) 

## MessageInsightsFiltersUnionTypeDef

```python
# MessageInsightsFiltersUnionTypeDef definition

MessageInsightsFiltersUnionTypeDef = Union[
    MessageInsightsFiltersTypeDef,  # (1)
    MessageInsightsFiltersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MessageInsightsFiltersTypeDef](./type_defs.md#messageinsightsfilterstypedef) 
2. See [:material-code-braces: MessageInsightsFiltersOutputTypeDef](./type_defs.md#messageinsightsfiltersoutputtypedef) 

## CloudWatchDestinationUnionTypeDef

```python
# CloudWatchDestinationUnionTypeDef definition

CloudWatchDestinationUnionTypeDef = Union[
    CloudWatchDestinationTypeDef,  # (1)
    CloudWatchDestinationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CloudWatchDestinationTypeDef](./type_defs.md#cloudwatchdestinationtypedef) 
2. See [:material-code-braces: CloudWatchDestinationOutputTypeDef](./type_defs.md#cloudwatchdestinationoutputtypedef) 

## MetricsDataSourceUnionTypeDef

```python
# MetricsDataSourceUnionTypeDef definition

MetricsDataSourceUnionTypeDef = Union[
    MetricsDataSourceTypeDef,  # (1)
    MetricsDataSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MetricsDataSourceTypeDef](./type_defs.md#metricsdatasourcetypedef) 
2. See [:material-code-braces: MetricsDataSourceOutputTypeDef](./type_defs.md#metricsdatasourceoutputtypedef) 

## DomainDeliverabilityTrackingOptionUnionTypeDef

```python
# DomainDeliverabilityTrackingOptionUnionTypeDef definition

DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
    DomainDeliverabilityTrackingOptionTypeDef,  # (1)
    DomainDeliverabilityTrackingOptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DomainDeliverabilityTrackingOptionTypeDef](./type_defs.md#domaindeliverabilitytrackingoptiontypedef) 
2. See [:material-code-braces: DomainDeliverabilityTrackingOptionOutputTypeDef](./type_defs.md#domaindeliverabilitytrackingoptionoutputtypedef) 

## MessageInsightsDataSourceUnionTypeDef

```python
# MessageInsightsDataSourceUnionTypeDef definition

MessageInsightsDataSourceUnionTypeDef = Union[
    MessageInsightsDataSourceTypeDef,  # (1)
    MessageInsightsDataSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MessageInsightsDataSourceTypeDef](./type_defs.md#messageinsightsdatasourcetypedef) 
2. See [:material-code-braces: MessageInsightsDataSourceOutputTypeDef](./type_defs.md#messageinsightsdatasourceoutputtypedef) 



## ReviewDetailsTypeDef

```python
# ReviewDetailsTypeDef definition

class ReviewDetailsTypeDef(TypedDict):
    Status: NotRequired[ReviewStatusType],  # (1)
    CaseId: NotRequired[str],
```

1. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
## MetricDataErrorTypeDef

```python
# MetricDataErrorTypeDef definition

class MetricDataErrorTypeDef(TypedDict):
    Id: NotRequired[str],
    Code: NotRequired[QueryErrorCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: QueryErrorCodeType](./literals.md#queryerrorcodetype) 
## MetricDataResultTypeDef

```python
# MetricDataResultTypeDef definition

class MetricDataResultTypeDef(TypedDict):
    Id: NotRequired[str],
    Timestamps: NotRequired[List[datetime]],
    Values: NotRequired[List[int]],
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

## BlacklistEntryTypeDef

```python
# BlacklistEntryTypeDef definition

class BlacklistEntryTypeDef(TypedDict):
    RblName: NotRequired[str],
    ListingTime: NotRequired[datetime],
    Description: NotRequired[str],
```

## ContentTypeDef

```python
# ContentTypeDef definition

class ContentTypeDef(TypedDict):
    Data: str,
    Charset: NotRequired[str],
```

## BounceTypeDef

```python
# BounceTypeDef definition

class BounceTypeDef(TypedDict):
    BounceType: NotRequired[BounceTypeType],  # (1)
    BounceSubType: NotRequired[str],
    DiagnosticCode: NotRequired[str],
```

1. See [:material-code-brackets: BounceTypeType](./literals.md#bouncetypetype) 
## BulkEmailEntryResultTypeDef

```python
# BulkEmailEntryResultTypeDef definition

class BulkEmailEntryResultTypeDef(TypedDict):
    Status: NotRequired[BulkEmailStatusType],  # (1)
    Error: NotRequired[str],
    MessageId: NotRequired[str],
```

1. See [:material-code-brackets: BulkEmailStatusType](./literals.md#bulkemailstatustype) 
## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    ToAddresses: NotRequired[Sequence[str]],
    CcAddresses: NotRequired[Sequence[str]],
    BccAddresses: NotRequired[Sequence[str]],
```

## MessageHeaderTypeDef

```python
# MessageHeaderTypeDef definition

class MessageHeaderTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## MessageTagTypeDef

```python
# MessageTagTypeDef definition

class MessageTagTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## CancelExportJobRequestRequestTypeDef

```python
# CancelExportJobRequestRequestTypeDef definition

class CancelExportJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## CloudWatchDimensionConfigurationTypeDef

```python
# CloudWatchDimensionConfigurationTypeDef definition

class CloudWatchDimensionConfigurationTypeDef(TypedDict):
    DimensionName: str,
    DimensionValueSource: DimensionValueSourceType,  # (1)
    DefaultDimensionValue: str,
```

1. See [:material-code-brackets: DimensionValueSourceType](./literals.md#dimensionvaluesourcetype) 
## ComplaintTypeDef

```python
# ComplaintTypeDef definition

class ComplaintTypeDef(TypedDict):
    ComplaintSubType: NotRequired[str],
    ComplaintFeedbackType: NotRequired[str],
```

## ContactListDestinationTypeDef

```python
# ContactListDestinationTypeDef definition

class ContactListDestinationTypeDef(TypedDict):
    ContactListName: str,
    ContactListImportAction: ContactListImportActionType,  # (1)
```

1. See [:material-code-brackets: ContactListImportActionType](./literals.md#contactlistimportactiontype) 
## ContactListTypeDef

```python
# ContactListTypeDef definition

class ContactListTypeDef(TypedDict):
    ContactListName: NotRequired[str],
    LastUpdatedTimestamp: NotRequired[datetime],
```

## TopicPreferenceTypeDef

```python
# TopicPreferenceTypeDef definition

class TopicPreferenceTypeDef(TypedDict):
    TopicName: str,
    SubscriptionStatus: SubscriptionStatusType,  # (1)
```

1. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
## DeliveryOptionsTypeDef

```python
# DeliveryOptionsTypeDef definition

class DeliveryOptionsTypeDef(TypedDict):
    TlsPolicy: NotRequired[TlsPolicyType],  # (1)
    SendingPoolName: NotRequired[str],
    MaxDeliverySeconds: NotRequired[int],
```

1. See [:material-code-brackets: TlsPolicyType](./literals.md#tlspolicytype) 
## SendingOptionsTypeDef

```python
# SendingOptionsTypeDef definition

class SendingOptionsTypeDef(TypedDict):
    SendingEnabled: NotRequired[bool],
```

## SuppressionOptionsTypeDef

```python
# SuppressionOptionsTypeDef definition

class SuppressionOptionsTypeDef(TypedDict):
    SuppressedReasons: NotRequired[Sequence[SuppressionListReasonType]],  # (1)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## TrackingOptionsTypeDef

```python
# TrackingOptionsTypeDef definition

class TrackingOptionsTypeDef(TypedDict):
    CustomRedirectDomain: str,
    HttpsPolicy: NotRequired[HttpsPolicyType],  # (1)
```

1. See [:material-code-brackets: HttpsPolicyType](./literals.md#httpspolicytype) 
## TopicTypeDef

```python
# TopicTypeDef definition

class TopicTypeDef(TypedDict):
    TopicName: str,
    DisplayName: str,
    DefaultSubscriptionStatus: SubscriptionStatusType,  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
## CreateCustomVerificationEmailTemplateRequestRequestTypeDef

```python
# CreateCustomVerificationEmailTemplateRequestRequestTypeDef definition

class CreateCustomVerificationEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    FromEmailAddress: str,
    TemplateSubject: str,
    TemplateContent: str,
    SuccessRedirectionURL: str,
    FailureRedirectionURL: str,
```

## CreateEmailIdentityPolicyRequestRequestTypeDef

```python
# CreateEmailIdentityPolicyRequestRequestTypeDef definition

class CreateEmailIdentityPolicyRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
    PolicyName: str,
    Policy: str,
```

## DkimSigningAttributesTypeDef

```python
# DkimSigningAttributesTypeDef definition

class DkimSigningAttributesTypeDef(TypedDict):
    DomainSigningSelector: NotRequired[str],
    DomainSigningPrivateKey: NotRequired[str],
    NextSigningKeyLength: NotRequired[DkimSigningKeyLengthType],  # (1)
    DomainSigningAttributesOrigin: NotRequired[DkimSigningAttributesOriginType],  # (2)
```

1. See [:material-code-brackets: DkimSigningKeyLengthType](./literals.md#dkimsigningkeylengthtype) 
2. See [:material-code-brackets: DkimSigningAttributesOriginType](./literals.md#dkimsigningattributesorigintype) 
## DkimAttributesTypeDef

```python
# DkimAttributesTypeDef definition

class DkimAttributesTypeDef(TypedDict):
    SigningEnabled: NotRequired[bool],
    Status: NotRequired[DkimStatusType],  # (1)
    Tokens: NotRequired[List[str]],
    SigningAttributesOrigin: NotRequired[DkimSigningAttributesOriginType],  # (2)
    NextSigningKeyLength: NotRequired[DkimSigningKeyLengthType],  # (3)
    CurrentSigningKeyLength: NotRequired[DkimSigningKeyLengthType],  # (3)
    LastKeyGenerationTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: DkimStatusType](./literals.md#dkimstatustype) 
2. See [:material-code-brackets: DkimSigningAttributesOriginType](./literals.md#dkimsigningattributesorigintype) 
3. See [:material-code-brackets: DkimSigningKeyLengthType](./literals.md#dkimsigningkeylengthtype) 
4. See [:material-code-brackets: DkimSigningKeyLengthType](./literals.md#dkimsigningkeylengthtype) 
## EmailTemplateContentTypeDef

```python
# EmailTemplateContentTypeDef definition

class EmailTemplateContentTypeDef(TypedDict):
    Subject: NotRequired[str],
    Text: NotRequired[str],
    Html: NotRequired[str],
```

## ExportDestinationTypeDef

```python
# ExportDestinationTypeDef definition

class ExportDestinationTypeDef(TypedDict):
    DataFormat: DataFormatType,  # (1)
    S3Url: NotRequired[str],
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
## ImportDataSourceTypeDef

```python
# ImportDataSourceTypeDef definition

class ImportDataSourceTypeDef(TypedDict):
    S3Url: str,
    DataFormat: DataFormatType,  # (1)
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
## CustomVerificationEmailTemplateMetadataTypeDef

```python
# CustomVerificationEmailTemplateMetadataTypeDef definition

class CustomVerificationEmailTemplateMetadataTypeDef(TypedDict):
    TemplateName: NotRequired[str],
    FromEmailAddress: NotRequired[str],
    TemplateSubject: NotRequired[str],
    SuccessRedirectionURL: NotRequired[str],
    FailureRedirectionURL: NotRequired[str],
```

## DomainIspPlacementTypeDef

```python
# DomainIspPlacementTypeDef definition

class DomainIspPlacementTypeDef(TypedDict):
    IspName: NotRequired[str],
    InboxRawCount: NotRequired[int],
    SpamRawCount: NotRequired[int],
    InboxPercentage: NotRequired[float],
    SpamPercentage: NotRequired[float],
```

## VolumeStatisticsTypeDef

```python
# VolumeStatisticsTypeDef definition

class VolumeStatisticsTypeDef(TypedDict):
    InboxRawCount: NotRequired[int],
    SpamRawCount: NotRequired[int],
    ProjectedInbox: NotRequired[int],
    ProjectedSpam: NotRequired[int],
```

## DashboardAttributesTypeDef

```python
# DashboardAttributesTypeDef definition

class DashboardAttributesTypeDef(TypedDict):
    EngagementMetrics: NotRequired[FeatureStatusType],  # (1)
```

1. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## DashboardOptionsTypeDef

```python
# DashboardOptionsTypeDef definition

class DashboardOptionsTypeDef(TypedDict):
    EngagementMetrics: NotRequired[FeatureStatusType],  # (1)
```

1. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## DedicatedIpPoolTypeDef

```python
# DedicatedIpPoolTypeDef definition

class DedicatedIpPoolTypeDef(TypedDict):
    PoolName: str,
    ScalingMode: ScalingModeType,  # (1)
```

1. See [:material-code-brackets: ScalingModeType](./literals.md#scalingmodetype) 
## DedicatedIpTypeDef

```python
# DedicatedIpTypeDef definition

class DedicatedIpTypeDef(TypedDict):
    Ip: str,
    WarmupStatus: WarmupStatusType,  # (1)
    WarmupPercentage: int,
    PoolName: NotRequired[str],
```

1. See [:material-code-brackets: WarmupStatusType](./literals.md#warmupstatustype) 
## DeleteConfigurationSetEventDestinationRequestRequestTypeDef

```python
# DeleteConfigurationSetEventDestinationRequestRequestTypeDef definition

class DeleteConfigurationSetEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
```

## DeleteConfigurationSetRequestRequestTypeDef

```python
# DeleteConfigurationSetRequestRequestTypeDef definition

class DeleteConfigurationSetRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## DeleteContactListRequestRequestTypeDef

```python
# DeleteContactListRequestRequestTypeDef definition

class DeleteContactListRequestRequestTypeDef(TypedDict):
    ContactListName: str,
```

## DeleteContactRequestRequestTypeDef

```python
# DeleteContactRequestRequestTypeDef definition

class DeleteContactRequestRequestTypeDef(TypedDict):
    ContactListName: str,
    EmailAddress: str,
```

## DeleteCustomVerificationEmailTemplateRequestRequestTypeDef

```python
# DeleteCustomVerificationEmailTemplateRequestRequestTypeDef definition

class DeleteCustomVerificationEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
```

## DeleteDedicatedIpPoolRequestRequestTypeDef

```python
# DeleteDedicatedIpPoolRequestRequestTypeDef definition

class DeleteDedicatedIpPoolRequestRequestTypeDef(TypedDict):
    PoolName: str,
```

## DeleteEmailIdentityPolicyRequestRequestTypeDef

```python
# DeleteEmailIdentityPolicyRequestRequestTypeDef definition

class DeleteEmailIdentityPolicyRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
    PolicyName: str,
```

## DeleteEmailIdentityRequestRequestTypeDef

```python
# DeleteEmailIdentityRequestRequestTypeDef definition

class DeleteEmailIdentityRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
```

## DeleteEmailTemplateRequestRequestTypeDef

```python
# DeleteEmailTemplateRequestRequestTypeDef definition

class DeleteEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
```

## DeleteMultiRegionEndpointRequestRequestTypeDef

```python
# DeleteMultiRegionEndpointRequestRequestTypeDef definition

class DeleteMultiRegionEndpointRequestRequestTypeDef(TypedDict):
    EndpointName: str,
```

## DeleteSuppressedDestinationRequestRequestTypeDef

```python
# DeleteSuppressedDestinationRequestRequestTypeDef definition

class DeleteSuppressedDestinationRequestRequestTypeDef(TypedDict):
    EmailAddress: str,
```

## DeliverabilityTestReportTypeDef

```python
# DeliverabilityTestReportTypeDef definition

class DeliverabilityTestReportTypeDef(TypedDict):
    ReportId: NotRequired[str],
    ReportName: NotRequired[str],
    Subject: NotRequired[str],
    FromEmailAddress: NotRequired[str],
    CreateDate: NotRequired[datetime],
    DeliverabilityTestStatus: NotRequired[DeliverabilityTestStatusType],  # (1)
```

1. See [:material-code-brackets: DeliverabilityTestStatusType](./literals.md#deliverabilityteststatustype) 
## RouteDetailsTypeDef

```python
# RouteDetailsTypeDef definition

class RouteDetailsTypeDef(TypedDict):
    Region: str,
```

## DomainDeliverabilityCampaignTypeDef

```python
# DomainDeliverabilityCampaignTypeDef definition

class DomainDeliverabilityCampaignTypeDef(TypedDict):
    CampaignId: NotRequired[str],
    ImageUrl: NotRequired[str],
    Subject: NotRequired[str],
    FromAddress: NotRequired[str],
    SendingIps: NotRequired[List[str]],
    FirstSeenDateTime: NotRequired[datetime],
    LastSeenDateTime: NotRequired[datetime],
    InboxCount: NotRequired[int],
    SpamCount: NotRequired[int],
    ReadRate: NotRequired[float],
    DeleteRate: NotRequired[float],
    ReadDeleteRate: NotRequired[float],
    ProjectedVolume: NotRequired[int],
    Esps: NotRequired[List[str]],
```

## InboxPlacementTrackingOptionOutputTypeDef

```python
# InboxPlacementTrackingOptionOutputTypeDef definition

class InboxPlacementTrackingOptionOutputTypeDef(TypedDict):
    Global: NotRequired[bool],
    TrackedIsps: NotRequired[List[str]],
```

## EmailTemplateMetadataTypeDef

```python
# EmailTemplateMetadataTypeDef definition

class EmailTemplateMetadataTypeDef(TypedDict):
    TemplateName: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
```

## EventBridgeDestinationTypeDef

```python
# EventBridgeDestinationTypeDef definition

class EventBridgeDestinationTypeDef(TypedDict):
    EventBusArn: str,
```

## KinesisFirehoseDestinationTypeDef

```python
# KinesisFirehoseDestinationTypeDef definition

class KinesisFirehoseDestinationTypeDef(TypedDict):
    IamRoleArn: str,
    DeliveryStreamArn: str,
```

## PinpointDestinationTypeDef

```python
# PinpointDestinationTypeDef definition

class PinpointDestinationTypeDef(TypedDict):
    ApplicationArn: NotRequired[str],
```

## SnsDestinationTypeDef

```python
# SnsDestinationTypeDef definition

class SnsDestinationTypeDef(TypedDict):
    TopicArn: str,
```

## ExportJobSummaryTypeDef

```python
# ExportJobSummaryTypeDef definition

class ExportJobSummaryTypeDef(TypedDict):
    JobId: NotRequired[str],
    ExportSourceType: NotRequired[ExportSourceTypeType],  # (1)
    JobStatus: NotRequired[JobStatusType],  # (2)
    CreatedTimestamp: NotRequired[datetime],
    CompletedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ExportSourceTypeType](./literals.md#exportsourcetypetype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## ExportMetricTypeDef

```python
# ExportMetricTypeDef definition

class ExportMetricTypeDef(TypedDict):
    Name: NotRequired[MetricType],  # (1)
    Aggregation: NotRequired[MetricAggregationType],  # (2)
```

1. See [:material-code-brackets: MetricType](./literals.md#metrictype) 
2. See [:material-code-brackets: MetricAggregationType](./literals.md#metricaggregationtype) 
## ExportStatisticsTypeDef

```python
# ExportStatisticsTypeDef definition

class ExportStatisticsTypeDef(TypedDict):
    ProcessedRecordsCount: NotRequired[int],
    ExportedRecordsCount: NotRequired[int],
```

## FailureInfoTypeDef

```python
# FailureInfoTypeDef definition

class FailureInfoTypeDef(TypedDict):
    FailedRecordsS3Url: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## SendQuotaTypeDef

```python
# SendQuotaTypeDef definition

class SendQuotaTypeDef(TypedDict):
    Max24HourSend: NotRequired[float],
    MaxSendRate: NotRequired[float],
    SentLast24Hours: NotRequired[float],
```

## SuppressionAttributesTypeDef

```python
# SuppressionAttributesTypeDef definition

class SuppressionAttributesTypeDef(TypedDict):
    SuppressedReasons: NotRequired[List[SuppressionListReasonType]],  # (1)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## GetBlacklistReportsRequestRequestTypeDef

```python
# GetBlacklistReportsRequestRequestTypeDef definition

class GetBlacklistReportsRequestRequestTypeDef(TypedDict):
    BlacklistItemNames: Sequence[str],
```

## GetConfigurationSetEventDestinationsRequestRequestTypeDef

```python
# GetConfigurationSetEventDestinationsRequestRequestTypeDef definition

class GetConfigurationSetEventDestinationsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## GetConfigurationSetRequestRequestTypeDef

```python
# GetConfigurationSetRequestRequestTypeDef definition

class GetConfigurationSetRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## ReputationOptionsOutputTypeDef

```python
# ReputationOptionsOutputTypeDef definition

class ReputationOptionsOutputTypeDef(TypedDict):
    ReputationMetricsEnabled: NotRequired[bool],
    LastFreshStart: NotRequired[datetime],
```

## SuppressionOptionsOutputTypeDef

```python
# SuppressionOptionsOutputTypeDef definition

class SuppressionOptionsOutputTypeDef(TypedDict):
    SuppressedReasons: NotRequired[List[SuppressionListReasonType]],  # (1)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## GetContactListRequestRequestTypeDef

```python
# GetContactListRequestRequestTypeDef definition

class GetContactListRequestRequestTypeDef(TypedDict):
    ContactListName: str,
```

## GetContactRequestRequestTypeDef

```python
# GetContactRequestRequestTypeDef definition

class GetContactRequestRequestTypeDef(TypedDict):
    ContactListName: str,
    EmailAddress: str,
```

## GetCustomVerificationEmailTemplateRequestRequestTypeDef

```python
# GetCustomVerificationEmailTemplateRequestRequestTypeDef definition

class GetCustomVerificationEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
```

## GetDedicatedIpPoolRequestRequestTypeDef

```python
# GetDedicatedIpPoolRequestRequestTypeDef definition

class GetDedicatedIpPoolRequestRequestTypeDef(TypedDict):
    PoolName: str,
```

## GetDedicatedIpRequestRequestTypeDef

```python
# GetDedicatedIpRequestRequestTypeDef definition

class GetDedicatedIpRequestRequestTypeDef(TypedDict):
    Ip: str,
```

## GetDedicatedIpsRequestRequestTypeDef

```python
# GetDedicatedIpsRequestRequestTypeDef definition

class GetDedicatedIpsRequestRequestTypeDef(TypedDict):
    PoolName: NotRequired[str],
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## GetDeliverabilityTestReportRequestRequestTypeDef

```python
# GetDeliverabilityTestReportRequestRequestTypeDef definition

class GetDeliverabilityTestReportRequestRequestTypeDef(TypedDict):
    ReportId: str,
```

## PlacementStatisticsTypeDef

```python
# PlacementStatisticsTypeDef definition

class PlacementStatisticsTypeDef(TypedDict):
    InboxPercentage: NotRequired[float],
    SpamPercentage: NotRequired[float],
    MissingPercentage: NotRequired[float],
    SpfPercentage: NotRequired[float],
    DkimPercentage: NotRequired[float],
```

## GetDomainDeliverabilityCampaignRequestRequestTypeDef

```python
# GetDomainDeliverabilityCampaignRequestRequestTypeDef definition

class GetDomainDeliverabilityCampaignRequestRequestTypeDef(TypedDict):
    CampaignId: str,
```

## GetEmailIdentityPoliciesRequestRequestTypeDef

```python
# GetEmailIdentityPoliciesRequestRequestTypeDef definition

class GetEmailIdentityPoliciesRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
```

## GetEmailIdentityRequestRequestTypeDef

```python
# GetEmailIdentityRequestRequestTypeDef definition

class GetEmailIdentityRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
```

## MailFromAttributesTypeDef

```python
# MailFromAttributesTypeDef definition

class MailFromAttributesTypeDef(TypedDict):
    MailFromDomain: str,
    MailFromDomainStatus: MailFromDomainStatusType,  # (1)
    BehaviorOnMxFailure: BehaviorOnMxFailureType,  # (2)
```

1. See [:material-code-brackets: MailFromDomainStatusType](./literals.md#mailfromdomainstatustype) 
2. See [:material-code-brackets: BehaviorOnMxFailureType](./literals.md#behavioronmxfailuretype) 
## GetEmailTemplateRequestRequestTypeDef

```python
# GetEmailTemplateRequestRequestTypeDef definition

class GetEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
```

## GetExportJobRequestRequestTypeDef

```python
# GetExportJobRequestRequestTypeDef definition

class GetExportJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## GetImportJobRequestRequestTypeDef

```python
# GetImportJobRequestRequestTypeDef definition

class GetImportJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## GetMessageInsightsRequestRequestTypeDef

```python
# GetMessageInsightsRequestRequestTypeDef definition

class GetMessageInsightsRequestRequestTypeDef(TypedDict):
    MessageId: str,
```

## GetMultiRegionEndpointRequestRequestTypeDef

```python
# GetMultiRegionEndpointRequestRequestTypeDef definition

class GetMultiRegionEndpointRequestRequestTypeDef(TypedDict):
    EndpointName: str,
```

## RouteTypeDef

```python
# RouteTypeDef definition

class RouteTypeDef(TypedDict):
    Region: str,
```

## GetSuppressedDestinationRequestRequestTypeDef

```python
# GetSuppressedDestinationRequestRequestTypeDef definition

class GetSuppressedDestinationRequestRequestTypeDef(TypedDict):
    EmailAddress: str,
```

## GuardianAttributesTypeDef

```python
# GuardianAttributesTypeDef definition

class GuardianAttributesTypeDef(TypedDict):
    OptimizedSharedDelivery: NotRequired[FeatureStatusType],  # (1)
```

1. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## GuardianOptionsTypeDef

```python
# GuardianOptionsTypeDef definition

class GuardianOptionsTypeDef(TypedDict):
    OptimizedSharedDelivery: NotRequired[FeatureStatusType],  # (1)
```

1. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## IdentityInfoTypeDef

```python
# IdentityInfoTypeDef definition

class IdentityInfoTypeDef(TypedDict):
    IdentityType: NotRequired[IdentityTypeType],  # (1)
    IdentityName: NotRequired[str],
    SendingEnabled: NotRequired[bool],
    VerificationStatus: NotRequired[VerificationStatusType],  # (2)
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-brackets: VerificationStatusType](./literals.md#verificationstatustype) 
## SuppressionListDestinationTypeDef

```python
# SuppressionListDestinationTypeDef definition

class SuppressionListDestinationTypeDef(TypedDict):
    SuppressionListImportAction: SuppressionListImportActionType,  # (1)
```

1. See [:material-code-brackets: SuppressionListImportActionType](./literals.md#suppressionlistimportactiontype) 
## InboxPlacementTrackingOptionTypeDef

```python
# InboxPlacementTrackingOptionTypeDef definition

class InboxPlacementTrackingOptionTypeDef(TypedDict):
    Global: NotRequired[bool],
    TrackedIsps: NotRequired[Sequence[str]],
```

## ListConfigurationSetsRequestRequestTypeDef

```python
# ListConfigurationSetsRequestRequestTypeDef definition

class ListConfigurationSetsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListContactListsRequestRequestTypeDef

```python
# ListContactListsRequestRequestTypeDef definition

class ListContactListsRequestRequestTypeDef(TypedDict):
    PageSize: NotRequired[int],
    NextToken: NotRequired[str],
```

## TopicFilterTypeDef

```python
# TopicFilterTypeDef definition

class TopicFilterTypeDef(TypedDict):
    TopicName: NotRequired[str],
    UseDefaultIfPreferenceUnavailable: NotRequired[bool],
```

## ListCustomVerificationEmailTemplatesRequestRequestTypeDef

```python
# ListCustomVerificationEmailTemplatesRequestRequestTypeDef definition

class ListCustomVerificationEmailTemplatesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListDedicatedIpPoolsRequestRequestTypeDef

```python
# ListDedicatedIpPoolsRequestRequestTypeDef definition

class ListDedicatedIpPoolsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListDeliverabilityTestReportsRequestRequestTypeDef

```python
# ListDeliverabilityTestReportsRequestRequestTypeDef definition

class ListDeliverabilityTestReportsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListEmailIdentitiesRequestRequestTypeDef

```python
# ListEmailIdentitiesRequestRequestTypeDef definition

class ListEmailIdentitiesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListEmailTemplatesRequestRequestTypeDef

```python
# ListEmailTemplatesRequestRequestTypeDef definition

class ListEmailTemplatesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListExportJobsRequestRequestTypeDef

```python
# ListExportJobsRequestRequestTypeDef definition

class ListExportJobsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
    ExportSourceType: NotRequired[ExportSourceTypeType],  # (1)
    JobStatus: NotRequired[JobStatusType],  # (2)
```

1. See [:material-code-brackets: ExportSourceTypeType](./literals.md#exportsourcetypetype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## ListImportJobsRequestRequestTypeDef

```python
# ListImportJobsRequestRequestTypeDef definition

class ListImportJobsRequestRequestTypeDef(TypedDict):
    ImportDestinationType: NotRequired[ImportDestinationTypeType],  # (1)
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

1. See [:material-code-brackets: ImportDestinationTypeType](./literals.md#importdestinationtypetype) 
## ListManagementOptionsTypeDef

```python
# ListManagementOptionsTypeDef definition

class ListManagementOptionsTypeDef(TypedDict):
    ContactListName: str,
    TopicName: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListMultiRegionEndpointsRequestRequestTypeDef

```python
# ListMultiRegionEndpointsRequestRequestTypeDef definition

class ListMultiRegionEndpointsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## MultiRegionEndpointTypeDef

```python
# MultiRegionEndpointTypeDef definition

class MultiRegionEndpointTypeDef(TypedDict):
    EndpointName: NotRequired[str],
    Status: NotRequired[StatusType],  # (1)
    EndpointId: NotRequired[str],
    Regions: NotRequired[List[str]],
    CreatedTimestamp: NotRequired[datetime],
    LastUpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## ListRecommendationsRequestRequestTypeDef

```python
# ListRecommendationsRequestRequestTypeDef definition

class ListRecommendationsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[Mapping[ListRecommendationsFilterKeyType, str]],  # (1)
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

1. See [:material-code-brackets: ListRecommendationsFilterKeyType](./literals.md#listrecommendationsfilterkeytype) 
## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    Type: NotRequired[RecommendationTypeType],  # (1)
    Description: NotRequired[str],
    Status: NotRequired[RecommendationStatusType],  # (2)
    CreatedTimestamp: NotRequired[datetime],
    LastUpdatedTimestamp: NotRequired[datetime],
    Impact: NotRequired[RecommendationImpactType],  # (3)
```

1. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
2. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
3. See [:material-code-brackets: RecommendationImpactType](./literals.md#recommendationimpacttype) 
## SuppressedDestinationSummaryTypeDef

```python
# SuppressedDestinationSummaryTypeDef definition

class SuppressedDestinationSummaryTypeDef(TypedDict):
    EmailAddress: str,
    Reason: SuppressionListReasonType,  # (1)
    LastUpdateTime: datetime,
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## MessageInsightsFiltersOutputTypeDef

```python
# MessageInsightsFiltersOutputTypeDef definition

class MessageInsightsFiltersOutputTypeDef(TypedDict):
    FromEmailAddress: NotRequired[List[str]],
    Destination: NotRequired[List[str]],
    Subject: NotRequired[List[str]],
    Isp: NotRequired[List[str]],
    LastDeliveryEvent: NotRequired[List[DeliveryEventTypeType]],  # (1)
    LastEngagementEvent: NotRequired[List[EngagementEventTypeType]],  # (2)
```

1. See [:material-code-brackets: DeliveryEventTypeType](./literals.md#deliveryeventtypetype) 
2. See [:material-code-brackets: EngagementEventTypeType](./literals.md#engagementeventtypetype) 
## MessageInsightsFiltersTypeDef

```python
# MessageInsightsFiltersTypeDef definition

class MessageInsightsFiltersTypeDef(TypedDict):
    FromEmailAddress: NotRequired[Sequence[str]],
    Destination: NotRequired[Sequence[str]],
    Subject: NotRequired[Sequence[str]],
    Isp: NotRequired[Sequence[str]],
    LastDeliveryEvent: NotRequired[Sequence[DeliveryEventTypeType]],  # (1)
    LastEngagementEvent: NotRequired[Sequence[EngagementEventTypeType]],  # (2)
```

1. See [:material-code-brackets: DeliveryEventTypeType](./literals.md#deliveryeventtypetype) 
2. See [:material-code-brackets: EngagementEventTypeType](./literals.md#engagementeventtypetype) 
## PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef

```python
# PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef definition

class PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef(TypedDict):
    AutoWarmupEnabled: NotRequired[bool],
```

## PutAccountDetailsRequestRequestTypeDef

```python
# PutAccountDetailsRequestRequestTypeDef definition

class PutAccountDetailsRequestRequestTypeDef(TypedDict):
    MailType: MailTypeType,  # (1)
    WebsiteURL: str,
    ContactLanguage: NotRequired[ContactLanguageType],  # (2)
    UseCaseDescription: NotRequired[str],
    AdditionalContactEmailAddresses: NotRequired[Sequence[str]],
    ProductionAccessEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: MailTypeType](./literals.md#mailtypetype) 
2. See [:material-code-brackets: ContactLanguageType](./literals.md#contactlanguagetype) 
## PutAccountSendingAttributesRequestRequestTypeDef

```python
# PutAccountSendingAttributesRequestRequestTypeDef definition

class PutAccountSendingAttributesRequestRequestTypeDef(TypedDict):
    SendingEnabled: NotRequired[bool],
```

## PutAccountSuppressionAttributesRequestRequestTypeDef

```python
# PutAccountSuppressionAttributesRequestRequestTypeDef definition

class PutAccountSuppressionAttributesRequestRequestTypeDef(TypedDict):
    SuppressedReasons: NotRequired[Sequence[SuppressionListReasonType]],  # (1)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## PutConfigurationSetDeliveryOptionsRequestRequestTypeDef

```python
# PutConfigurationSetDeliveryOptionsRequestRequestTypeDef definition

class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    TlsPolicy: NotRequired[TlsPolicyType],  # (1)
    SendingPoolName: NotRequired[str],
    MaxDeliverySeconds: NotRequired[int],
```

1. See [:material-code-brackets: TlsPolicyType](./literals.md#tlspolicytype) 
## PutConfigurationSetReputationOptionsRequestRequestTypeDef

```python
# PutConfigurationSetReputationOptionsRequestRequestTypeDef definition

class PutConfigurationSetReputationOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    ReputationMetricsEnabled: NotRequired[bool],
```

## PutConfigurationSetSendingOptionsRequestRequestTypeDef

```python
# PutConfigurationSetSendingOptionsRequestRequestTypeDef definition

class PutConfigurationSetSendingOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    SendingEnabled: NotRequired[bool],
```

## PutConfigurationSetSuppressionOptionsRequestRequestTypeDef

```python
# PutConfigurationSetSuppressionOptionsRequestRequestTypeDef definition

class PutConfigurationSetSuppressionOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    SuppressedReasons: NotRequired[Sequence[SuppressionListReasonType]],  # (1)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## PutConfigurationSetTrackingOptionsRequestRequestTypeDef

```python
# PutConfigurationSetTrackingOptionsRequestRequestTypeDef definition

class PutConfigurationSetTrackingOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    CustomRedirectDomain: NotRequired[str],
    HttpsPolicy: NotRequired[HttpsPolicyType],  # (1)
```

1. See [:material-code-brackets: HttpsPolicyType](./literals.md#httpspolicytype) 
## PutDedicatedIpInPoolRequestRequestTypeDef

```python
# PutDedicatedIpInPoolRequestRequestTypeDef definition

class PutDedicatedIpInPoolRequestRequestTypeDef(TypedDict):
    Ip: str,
    DestinationPoolName: str,
```

## PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef

```python
# PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef definition

class PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef(TypedDict):
    PoolName: str,
    ScalingMode: ScalingModeType,  # (1)
```

1. See [:material-code-brackets: ScalingModeType](./literals.md#scalingmodetype) 
## PutDedicatedIpWarmupAttributesRequestRequestTypeDef

```python
# PutDedicatedIpWarmupAttributesRequestRequestTypeDef definition

class PutDedicatedIpWarmupAttributesRequestRequestTypeDef(TypedDict):
    Ip: str,
    WarmupPercentage: int,
```

## PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef

```python
# PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef definition

class PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
    ConfigurationSetName: NotRequired[str],
```

## PutEmailIdentityDkimAttributesRequestRequestTypeDef

```python
# PutEmailIdentityDkimAttributesRequestRequestTypeDef definition

class PutEmailIdentityDkimAttributesRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
    SigningEnabled: NotRequired[bool],
```

## PutEmailIdentityFeedbackAttributesRequestRequestTypeDef

```python
# PutEmailIdentityFeedbackAttributesRequestRequestTypeDef definition

class PutEmailIdentityFeedbackAttributesRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
    EmailForwardingEnabled: NotRequired[bool],
```

## PutEmailIdentityMailFromAttributesRequestRequestTypeDef

```python
# PutEmailIdentityMailFromAttributesRequestRequestTypeDef definition

class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
    MailFromDomain: NotRequired[str],
    BehaviorOnMxFailure: NotRequired[BehaviorOnMxFailureType],  # (1)
```

1. See [:material-code-brackets: BehaviorOnMxFailureType](./literals.md#behavioronmxfailuretype) 
## PutSuppressedDestinationRequestRequestTypeDef

```python
# PutSuppressedDestinationRequestRequestTypeDef definition

class PutSuppressedDestinationRequestRequestTypeDef(TypedDict):
    EmailAddress: str,
    Reason: SuppressionListReasonType,  # (1)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## ReplacementTemplateTypeDef

```python
# ReplacementTemplateTypeDef definition

class ReplacementTemplateTypeDef(TypedDict):
    ReplacementTemplateData: NotRequired[str],
```

## SOARecordTypeDef

```python
# SOARecordTypeDef definition

class SOARecordTypeDef(TypedDict):
    PrimaryNameServer: NotRequired[str],
    AdminEmail: NotRequired[str],
    SerialNumber: NotRequired[int],
```

## SendCustomVerificationEmailRequestRequestTypeDef

```python
# SendCustomVerificationEmailRequestRequestTypeDef definition

class SendCustomVerificationEmailRequestRequestTypeDef(TypedDict):
    EmailAddress: str,
    TemplateName: str,
    ConfigurationSetName: NotRequired[str],
```

## SuppressedDestinationAttributesTypeDef

```python
# SuppressedDestinationAttributesTypeDef definition

class SuppressedDestinationAttributesTypeDef(TypedDict):
    MessageId: NotRequired[str],
    FeedbackId: NotRequired[str],
```

## TestRenderEmailTemplateRequestRequestTypeDef

```python
# TestRenderEmailTemplateRequestRequestTypeDef definition

class TestRenderEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    TemplateData: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateCustomVerificationEmailTemplateRequestRequestTypeDef

```python
# UpdateCustomVerificationEmailTemplateRequestRequestTypeDef definition

class UpdateCustomVerificationEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    FromEmailAddress: str,
    TemplateSubject: str,
    TemplateContent: str,
    SuccessRedirectionURL: str,
    FailureRedirectionURL: str,
```

## UpdateEmailIdentityPolicyRequestRequestTypeDef

```python
# UpdateEmailIdentityPolicyRequestRequestTypeDef definition

class UpdateEmailIdentityPolicyRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
    PolicyName: str,
    Policy: str,
```

## AccountDetailsTypeDef

```python
# AccountDetailsTypeDef definition

class AccountDetailsTypeDef(TypedDict):
    MailType: NotRequired[MailTypeType],  # (1)
    WebsiteURL: NotRequired[str],
    ContactLanguage: NotRequired[ContactLanguageType],  # (2)
    UseCaseDescription: NotRequired[str],
    AdditionalContactEmailAddresses: NotRequired[List[str]],
    ReviewDetails: NotRequired[ReviewDetailsTypeDef],  # (3)
```

1. See [:material-code-brackets: MailTypeType](./literals.md#mailtypetype) 
2. See [:material-code-brackets: ContactLanguageType](./literals.md#contactlanguagetype) 
3. See [:material-code-braces: ReviewDetailsTypeDef](./type_defs.md#reviewdetailstypedef) 
## BatchGetMetricDataQueryTypeDef

```python
# BatchGetMetricDataQueryTypeDef definition

class BatchGetMetricDataQueryTypeDef(TypedDict):
    Id: str,
    Namespace: MetricNamespaceType,  # (1)
    Metric: MetricType,  # (2)
    StartDate: TimestampTypeDef,
    EndDate: TimestampTypeDef,
    Dimensions: NotRequired[Mapping[MetricDimensionNameType, str]],  # (3)
```

1. See [:material-code-brackets: MetricNamespaceType](./literals.md#metricnamespacetype) 
2. See [:material-code-brackets: MetricType](./literals.md#metrictype) 
3. See [:material-code-brackets: MetricDimensionNameType](./literals.md#metricdimensionnametype) 
## GetDomainStatisticsReportRequestRequestTypeDef

```python
# GetDomainStatisticsReportRequestRequestTypeDef definition

class GetDomainStatisticsReportRequestRequestTypeDef(TypedDict):
    Domain: str,
    StartDate: TimestampTypeDef,
    EndDate: TimestampTypeDef,
```

## ListDomainDeliverabilityCampaignsRequestRequestTypeDef

```python
# ListDomainDeliverabilityCampaignsRequestRequestTypeDef definition

class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(TypedDict):
    StartDate: TimestampTypeDef,
    EndDate: TimestampTypeDef,
    SubscribedDomain: str,
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListSuppressedDestinationsRequestRequestTypeDef

```python
# ListSuppressedDestinationsRequestRequestTypeDef definition

class ListSuppressedDestinationsRequestRequestTypeDef(TypedDict):
    Reasons: NotRequired[Sequence[SuppressionListReasonType]],  # (1)
    StartDate: NotRequired[TimestampTypeDef],
    EndDate: NotRequired[TimestampTypeDef],
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## ReputationOptionsTypeDef

```python
# ReputationOptionsTypeDef definition

class ReputationOptionsTypeDef(TypedDict):
    ReputationMetricsEnabled: NotRequired[bool],
    LastFreshStart: NotRequired[TimestampTypeDef],
```

## BatchGetMetricDataResponseTypeDef

```python
# BatchGetMetricDataResponseTypeDef definition

class BatchGetMetricDataResponseTypeDef(TypedDict):
    Results: List[MetricDataResultTypeDef],  # (1)
    Errors: List[MetricDataErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MetricDataResultTypeDef](./type_defs.md#metricdataresulttypedef) 
2. See [:material-code-braces: MetricDataErrorTypeDef](./type_defs.md#metricdataerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeliverabilityTestReportResponseTypeDef

```python
# CreateDeliverabilityTestReportResponseTypeDef definition

class CreateDeliverabilityTestReportResponseTypeDef(TypedDict):
    ReportId: str,
    DeliverabilityTestStatus: DeliverabilityTestStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DeliverabilityTestStatusType](./literals.md#deliverabilityteststatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExportJobResponseTypeDef

```python
# CreateExportJobResponseTypeDef definition

class CreateExportJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateImportJobResponseTypeDef

```python
# CreateImportJobResponseTypeDef definition

class CreateImportJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMultiRegionEndpointResponseTypeDef

```python
# CreateMultiRegionEndpointResponseTypeDef definition

class CreateMultiRegionEndpointResponseTypeDef(TypedDict):
    Status: StatusType,  # (1)
    EndpointId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMultiRegionEndpointResponseTypeDef

```python
# DeleteMultiRegionEndpointResponseTypeDef definition

class DeleteMultiRegionEndpointResponseTypeDef(TypedDict):
    Status: StatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCustomVerificationEmailTemplateResponseTypeDef

```python
# GetCustomVerificationEmailTemplateResponseTypeDef definition

class GetCustomVerificationEmailTemplateResponseTypeDef(TypedDict):
    TemplateName: str,
    FromEmailAddress: str,
    TemplateSubject: str,
    TemplateContent: str,
    SuccessRedirectionURL: str,
    FailureRedirectionURL: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEmailIdentityPoliciesResponseTypeDef

```python
# GetEmailIdentityPoliciesResponseTypeDef definition

class GetEmailIdentityPoliciesResponseTypeDef(TypedDict):
    Policies: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationSetsResponseTypeDef

```python
# ListConfigurationSetsResponseTypeDef definition

class ListConfigurationSetsResponseTypeDef(TypedDict):
    ConfigurationSets: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDedicatedIpPoolsResponseTypeDef

```python
# ListDedicatedIpPoolsResponseTypeDef definition

class ListDedicatedIpPoolsResponseTypeDef(TypedDict):
    DedicatedIpPools: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutEmailIdentityDkimSigningAttributesResponseTypeDef

```python
# PutEmailIdentityDkimSigningAttributesResponseTypeDef definition

class PutEmailIdentityDkimSigningAttributesResponseTypeDef(TypedDict):
    DkimStatus: DkimStatusType,  # (1)
    DkimTokens: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DkimStatusType](./literals.md#dkimstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendCustomVerificationEmailResponseTypeDef

```python
# SendCustomVerificationEmailResponseTypeDef definition

class SendCustomVerificationEmailResponseTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendEmailResponseTypeDef

```python
# SendEmailResponseTypeDef definition

class SendEmailResponseTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestRenderEmailTemplateResponseTypeDef

```python
# TestRenderEmailTemplateResponseTypeDef definition

class TestRenderEmailTemplateResponseTypeDef(TypedDict):
    RenderedTemplate: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBlacklistReportsResponseTypeDef

```python
# GetBlacklistReportsResponseTypeDef definition

class GetBlacklistReportsResponseTypeDef(TypedDict):
    BlacklistReport: Dict[str, List[BlacklistEntryTypeDef]],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlacklistEntryTypeDef](./type_defs.md#blacklistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RawMessageTypeDef

```python
# RawMessageTypeDef definition

class RawMessageTypeDef(TypedDict):
    Data: BlobTypeDef,
```

## BodyTypeDef

```python
# BodyTypeDef definition

class BodyTypeDef(TypedDict):
    Text: NotRequired[ContentTypeDef],  # (1)
    Html: NotRequired[ContentTypeDef],  # (1)
```

1. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
2. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
## SendBulkEmailResponseTypeDef

```python
# SendBulkEmailResponseTypeDef definition

class SendBulkEmailResponseTypeDef(TypedDict):
    BulkEmailEntryResults: List[BulkEmailEntryResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BulkEmailEntryResultTypeDef](./type_defs.md#bulkemailentryresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CloudWatchDestinationOutputTypeDef

```python
# CloudWatchDestinationOutputTypeDef definition

class CloudWatchDestinationOutputTypeDef(TypedDict):
    DimensionConfigurations: List[CloudWatchDimensionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CloudWatchDimensionConfigurationTypeDef](./type_defs.md#cloudwatchdimensionconfigurationtypedef) 
## CloudWatchDestinationTypeDef

```python
# CloudWatchDestinationTypeDef definition

class CloudWatchDestinationTypeDef(TypedDict):
    DimensionConfigurations: Sequence[CloudWatchDimensionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CloudWatchDimensionConfigurationTypeDef](./type_defs.md#cloudwatchdimensionconfigurationtypedef) 
## EventDetailsTypeDef

```python
# EventDetailsTypeDef definition

class EventDetailsTypeDef(TypedDict):
    Bounce: NotRequired[BounceTypeDef],  # (1)
    Complaint: NotRequired[ComplaintTypeDef],  # (2)
```

1. See [:material-code-braces: BounceTypeDef](./type_defs.md#bouncetypedef) 
2. See [:material-code-braces: ComplaintTypeDef](./type_defs.md#complainttypedef) 
## ListContactListsResponseTypeDef

```python
# ListContactListsResponseTypeDef definition

class ListContactListsResponseTypeDef(TypedDict):
    ContactLists: List[ContactListTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContactListTypeDef](./type_defs.md#contactlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContactTypeDef

```python
# ContactTypeDef definition

class ContactTypeDef(TypedDict):
    EmailAddress: NotRequired[str],
    TopicPreferences: NotRequired[List[TopicPreferenceTypeDef]],  # (1)
    TopicDefaultPreferences: NotRequired[List[TopicPreferenceTypeDef]],  # (1)
    UnsubscribeAll: NotRequired[bool],
    LastUpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-braces: TopicPreferenceTypeDef](./type_defs.md#topicpreferencetypedef) 
2. See [:material-code-braces: TopicPreferenceTypeDef](./type_defs.md#topicpreferencetypedef) 
## CreateContactRequestRequestTypeDef

```python
# CreateContactRequestRequestTypeDef definition

class CreateContactRequestRequestTypeDef(TypedDict):
    ContactListName: str,
    EmailAddress: str,
    TopicPreferences: NotRequired[Sequence[TopicPreferenceTypeDef]],  # (1)
    UnsubscribeAll: NotRequired[bool],
    AttributesData: NotRequired[str],
```

1. See [:material-code-braces: TopicPreferenceTypeDef](./type_defs.md#topicpreferencetypedef) 
## GetContactResponseTypeDef

```python
# GetContactResponseTypeDef definition

class GetContactResponseTypeDef(TypedDict):
    ContactListName: str,
    EmailAddress: str,
    TopicPreferences: List[TopicPreferenceTypeDef],  # (1)
    TopicDefaultPreferences: List[TopicPreferenceTypeDef],  # (1)
    UnsubscribeAll: bool,
    AttributesData: str,
    CreatedTimestamp: datetime,
    LastUpdatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TopicPreferenceTypeDef](./type_defs.md#topicpreferencetypedef) 
2. See [:material-code-braces: TopicPreferenceTypeDef](./type_defs.md#topicpreferencetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContactRequestRequestTypeDef

```python
# UpdateContactRequestRequestTypeDef definition

class UpdateContactRequestRequestTypeDef(TypedDict):
    ContactListName: str,
    EmailAddress: str,
    TopicPreferences: NotRequired[Sequence[TopicPreferenceTypeDef]],  # (1)
    UnsubscribeAll: NotRequired[bool],
    AttributesData: NotRequired[str],
```

1. See [:material-code-braces: TopicPreferenceTypeDef](./type_defs.md#topicpreferencetypedef) 
## CreateDedicatedIpPoolRequestRequestTypeDef

```python
# CreateDedicatedIpPoolRequestRequestTypeDef definition

class CreateDedicatedIpPoolRequestRequestTypeDef(TypedDict):
    PoolName: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    ScalingMode: NotRequired[ScalingModeType],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: ScalingModeType](./literals.md#scalingmodetype) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
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
## CreateContactListRequestRequestTypeDef

```python
# CreateContactListRequestRequestTypeDef definition

class CreateContactListRequestRequestTypeDef(TypedDict):
    ContactListName: str,
    Topics: NotRequired[Sequence[TopicTypeDef]],  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: TopicTypeDef](./type_defs.md#topictypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetContactListResponseTypeDef

```python
# GetContactListResponseTypeDef definition

class GetContactListResponseTypeDef(TypedDict):
    ContactListName: str,
    Topics: List[TopicTypeDef],  # (1)
    Description: str,
    CreatedTimestamp: datetime,
    LastUpdatedTimestamp: datetime,
    Tags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TopicTypeDef](./type_defs.md#topictypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContactListRequestRequestTypeDef

```python
# UpdateContactListRequestRequestTypeDef definition

class UpdateContactListRequestRequestTypeDef(TypedDict):
    ContactListName: str,
    Topics: NotRequired[Sequence[TopicTypeDef]],  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-braces: TopicTypeDef](./type_defs.md#topictypedef) 
## CreateEmailIdentityRequestRequestTypeDef

```python
# CreateEmailIdentityRequestRequestTypeDef definition

class CreateEmailIdentityRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    DkimSigningAttributes: NotRequired[DkimSigningAttributesTypeDef],  # (2)
    ConfigurationSetName: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: DkimSigningAttributesTypeDef](./type_defs.md#dkimsigningattributestypedef) 
## PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef

```python
# PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef definition

class PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
    SigningAttributesOrigin: DkimSigningAttributesOriginType,  # (1)
    SigningAttributes: NotRequired[DkimSigningAttributesTypeDef],  # (2)
```

1. See [:material-code-brackets: DkimSigningAttributesOriginType](./literals.md#dkimsigningattributesorigintype) 
2. See [:material-code-braces: DkimSigningAttributesTypeDef](./type_defs.md#dkimsigningattributestypedef) 
## CreateEmailIdentityResponseTypeDef

```python
# CreateEmailIdentityResponseTypeDef definition

class CreateEmailIdentityResponseTypeDef(TypedDict):
    IdentityType: IdentityTypeType,  # (1)
    VerifiedForSendingStatus: bool,
    DkimAttributes: DkimAttributesTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-braces: DkimAttributesTypeDef](./type_defs.md#dkimattributestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEmailTemplateRequestRequestTypeDef

```python
# CreateEmailTemplateRequestRequestTypeDef definition

class CreateEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    TemplateContent: EmailTemplateContentTypeDef,  # (1)
```

1. See [:material-code-braces: EmailTemplateContentTypeDef](./type_defs.md#emailtemplatecontenttypedef) 
## GetEmailTemplateResponseTypeDef

```python
# GetEmailTemplateResponseTypeDef definition

class GetEmailTemplateResponseTypeDef(TypedDict):
    TemplateName: str,
    TemplateContent: EmailTemplateContentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EmailTemplateContentTypeDef](./type_defs.md#emailtemplatecontenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TemplateTypeDef

```python
# TemplateTypeDef definition

class TemplateTypeDef(TypedDict):
    TemplateName: NotRequired[str],
    TemplateArn: NotRequired[str],
    TemplateContent: NotRequired[EmailTemplateContentTypeDef],  # (1)
    TemplateData: NotRequired[str],
    Headers: NotRequired[Sequence[MessageHeaderTypeDef]],  # (2)
```

1. See [:material-code-braces: EmailTemplateContentTypeDef](./type_defs.md#emailtemplatecontenttypedef) 
2. See [:material-code-braces: MessageHeaderTypeDef](./type_defs.md#messageheadertypedef) 
## UpdateEmailTemplateRequestRequestTypeDef

```python
# UpdateEmailTemplateRequestRequestTypeDef definition

class UpdateEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    TemplateContent: EmailTemplateContentTypeDef,  # (1)
```

1. See [:material-code-braces: EmailTemplateContentTypeDef](./type_defs.md#emailtemplatecontenttypedef) 
## ListCustomVerificationEmailTemplatesResponseTypeDef

```python
# ListCustomVerificationEmailTemplatesResponseTypeDef definition

class ListCustomVerificationEmailTemplatesResponseTypeDef(TypedDict):
    CustomVerificationEmailTemplates: List[CustomVerificationEmailTemplateMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CustomVerificationEmailTemplateMetadataTypeDef](./type_defs.md#customverificationemailtemplatemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DailyVolumeTypeDef

```python
# DailyVolumeTypeDef definition

class DailyVolumeTypeDef(TypedDict):
    StartDate: NotRequired[datetime],
    VolumeStatistics: NotRequired[VolumeStatisticsTypeDef],  # (1)
    DomainIspPlacements: NotRequired[List[DomainIspPlacementTypeDef]],  # (2)
```

1. See [:material-code-braces: VolumeStatisticsTypeDef](./type_defs.md#volumestatisticstypedef) 
2. See [:material-code-braces: DomainIspPlacementTypeDef](./type_defs.md#domainispplacementtypedef) 
## OverallVolumeTypeDef

```python
# OverallVolumeTypeDef definition

class OverallVolumeTypeDef(TypedDict):
    VolumeStatistics: NotRequired[VolumeStatisticsTypeDef],  # (1)
    ReadRatePercent: NotRequired[float],
    DomainIspPlacements: NotRequired[List[DomainIspPlacementTypeDef]],  # (2)
```

1. See [:material-code-braces: VolumeStatisticsTypeDef](./type_defs.md#volumestatisticstypedef) 
2. See [:material-code-braces: DomainIspPlacementTypeDef](./type_defs.md#domainispplacementtypedef) 
## GetDedicatedIpPoolResponseTypeDef

```python
# GetDedicatedIpPoolResponseTypeDef definition

class GetDedicatedIpPoolResponseTypeDef(TypedDict):
    DedicatedIpPool: DedicatedIpPoolTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DedicatedIpPoolTypeDef](./type_defs.md#dedicatedippooltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDedicatedIpResponseTypeDef

```python
# GetDedicatedIpResponseTypeDef definition

class GetDedicatedIpResponseTypeDef(TypedDict):
    DedicatedIp: DedicatedIpTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DedicatedIpTypeDef](./type_defs.md#dedicatediptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDedicatedIpsResponseTypeDef

```python
# GetDedicatedIpsResponseTypeDef definition

class GetDedicatedIpsResponseTypeDef(TypedDict):
    DedicatedIps: List[DedicatedIpTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DedicatedIpTypeDef](./type_defs.md#dedicatediptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeliverabilityTestReportsResponseTypeDef

```python
# ListDeliverabilityTestReportsResponseTypeDef definition

class ListDeliverabilityTestReportsResponseTypeDef(TypedDict):
    DeliverabilityTestReports: List[DeliverabilityTestReportTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DeliverabilityTestReportTypeDef](./type_defs.md#deliverabilitytestreporttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetailsTypeDef

```python
# DetailsTypeDef definition

class DetailsTypeDef(TypedDict):
    RoutesDetails: Sequence[RouteDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: RouteDetailsTypeDef](./type_defs.md#routedetailstypedef) 
## GetDomainDeliverabilityCampaignResponseTypeDef

```python
# GetDomainDeliverabilityCampaignResponseTypeDef definition

class GetDomainDeliverabilityCampaignResponseTypeDef(TypedDict):
    DomainDeliverabilityCampaign: DomainDeliverabilityCampaignTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainDeliverabilityCampaignTypeDef](./type_defs.md#domaindeliverabilitycampaigntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDomainDeliverabilityCampaignsResponseTypeDef

```python
# ListDomainDeliverabilityCampaignsResponseTypeDef definition

class ListDomainDeliverabilityCampaignsResponseTypeDef(TypedDict):
    DomainDeliverabilityCampaigns: List[DomainDeliverabilityCampaignTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DomainDeliverabilityCampaignTypeDef](./type_defs.md#domaindeliverabilitycampaigntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainDeliverabilityTrackingOptionOutputTypeDef

```python
# DomainDeliverabilityTrackingOptionOutputTypeDef definition

class DomainDeliverabilityTrackingOptionOutputTypeDef(TypedDict):
    Domain: NotRequired[str],
    SubscriptionStartDate: NotRequired[datetime],
    InboxPlacementTrackingOption: NotRequired[InboxPlacementTrackingOptionOutputTypeDef],  # (1)
```

1. See [:material-code-braces: InboxPlacementTrackingOptionOutputTypeDef](./type_defs.md#inboxplacementtrackingoptionoutputtypedef) 
## ListEmailTemplatesResponseTypeDef

```python
# ListEmailTemplatesResponseTypeDef definition

class ListEmailTemplatesResponseTypeDef(TypedDict):
    TemplatesMetadata: List[EmailTemplateMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EmailTemplateMetadataTypeDef](./type_defs.md#emailtemplatemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExportJobsResponseTypeDef

```python
# ListExportJobsResponseTypeDef definition

class ListExportJobsResponseTypeDef(TypedDict):
    ExportJobs: List[ExportJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportJobSummaryTypeDef](./type_defs.md#exportjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricsDataSourceOutputTypeDef

```python
# MetricsDataSourceOutputTypeDef definition

class MetricsDataSourceOutputTypeDef(TypedDict):
    Dimensions: Dict[MetricDimensionNameType, List[str]],  # (1)
    Namespace: MetricNamespaceType,  # (2)
    Metrics: List[ExportMetricTypeDef],  # (3)
    StartDate: datetime,
    EndDate: datetime,
```

1. See [:material-code-brackets: MetricDimensionNameType](./literals.md#metricdimensionnametype) 
2. See [:material-code-brackets: MetricNamespaceType](./literals.md#metricnamespacetype) 
3. See [:material-code-braces: ExportMetricTypeDef](./type_defs.md#exportmetrictypedef) 
## MetricsDataSourceTypeDef

```python
# MetricsDataSourceTypeDef definition

class MetricsDataSourceTypeDef(TypedDict):
    Dimensions: Mapping[MetricDimensionNameType, Sequence[str]],  # (1)
    Namespace: MetricNamespaceType,  # (2)
    Metrics: Sequence[ExportMetricTypeDef],  # (3)
    StartDate: TimestampTypeDef,
    EndDate: TimestampTypeDef,
```

1. See [:material-code-brackets: MetricDimensionNameType](./literals.md#metricdimensionnametype) 
2. See [:material-code-brackets: MetricNamespaceType](./literals.md#metricnamespacetype) 
3. See [:material-code-braces: ExportMetricTypeDef](./type_defs.md#exportmetrictypedef) 
## IspPlacementTypeDef

```python
# IspPlacementTypeDef definition

class IspPlacementTypeDef(TypedDict):
    IspName: NotRequired[str],
    PlacementStatistics: NotRequired[PlacementStatisticsTypeDef],  # (1)
```

1. See [:material-code-braces: PlacementStatisticsTypeDef](./type_defs.md#placementstatisticstypedef) 
## GetMultiRegionEndpointResponseTypeDef

```python
# GetMultiRegionEndpointResponseTypeDef definition

class GetMultiRegionEndpointResponseTypeDef(TypedDict):
    EndpointName: str,
    EndpointId: str,
    Routes: List[RouteTypeDef],  # (1)
    Status: StatusType,  # (2)
    CreatedTimestamp: datetime,
    LastUpdatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VdmAttributesTypeDef

```python
# VdmAttributesTypeDef definition

class VdmAttributesTypeDef(TypedDict):
    VdmEnabled: FeatureStatusType,  # (1)
    DashboardAttributes: NotRequired[DashboardAttributesTypeDef],  # (2)
    GuardianAttributes: NotRequired[GuardianAttributesTypeDef],  # (3)
```

1. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
2. See [:material-code-braces: DashboardAttributesTypeDef](./type_defs.md#dashboardattributestypedef) 
3. See [:material-code-braces: GuardianAttributesTypeDef](./type_defs.md#guardianattributestypedef) 
## VdmOptionsTypeDef

```python
# VdmOptionsTypeDef definition

class VdmOptionsTypeDef(TypedDict):
    DashboardOptions: NotRequired[DashboardOptionsTypeDef],  # (1)
    GuardianOptions: NotRequired[GuardianOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: DashboardOptionsTypeDef](./type_defs.md#dashboardoptionstypedef) 
2. See [:material-code-braces: GuardianOptionsTypeDef](./type_defs.md#guardianoptionstypedef) 
## ListEmailIdentitiesResponseTypeDef

```python
# ListEmailIdentitiesResponseTypeDef definition

class ListEmailIdentitiesResponseTypeDef(TypedDict):
    EmailIdentities: List[IdentityInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityInfoTypeDef](./type_defs.md#identityinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportDestinationTypeDef

```python
# ImportDestinationTypeDef definition

class ImportDestinationTypeDef(TypedDict):
    SuppressionListDestination: NotRequired[SuppressionListDestinationTypeDef],  # (1)
    ContactListDestination: NotRequired[ContactListDestinationTypeDef],  # (2)
```

1. See [:material-code-braces: SuppressionListDestinationTypeDef](./type_defs.md#suppressionlistdestinationtypedef) 
2. See [:material-code-braces: ContactListDestinationTypeDef](./type_defs.md#contactlistdestinationtypedef) 
## ListContactsFilterTypeDef

```python
# ListContactsFilterTypeDef definition

class ListContactsFilterTypeDef(TypedDict):
    FilteredStatus: NotRequired[SubscriptionStatusType],  # (1)
    TopicFilter: NotRequired[TopicFilterTypeDef],  # (2)
```

1. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
2. See [:material-code-braces: TopicFilterTypeDef](./type_defs.md#topicfiltertypedef) 
## ListMultiRegionEndpointsRequestPaginateTypeDef

```python
# ListMultiRegionEndpointsRequestPaginateTypeDef definition

class ListMultiRegionEndpointsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMultiRegionEndpointsResponseTypeDef

```python
# ListMultiRegionEndpointsResponseTypeDef definition

class ListMultiRegionEndpointsResponseTypeDef(TypedDict):
    MultiRegionEndpoints: List[MultiRegionEndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MultiRegionEndpointTypeDef](./type_defs.md#multiregionendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecommendationsResponseTypeDef

```python
# ListRecommendationsResponseTypeDef definition

class ListRecommendationsResponseTypeDef(TypedDict):
    Recommendations: List[RecommendationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSuppressedDestinationsResponseTypeDef

```python
# ListSuppressedDestinationsResponseTypeDef definition

class ListSuppressedDestinationsResponseTypeDef(TypedDict):
    SuppressedDestinationSummaries: List[SuppressedDestinationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SuppressedDestinationSummaryTypeDef](./type_defs.md#suppresseddestinationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MessageInsightsDataSourceOutputTypeDef

```python
# MessageInsightsDataSourceOutputTypeDef definition

class MessageInsightsDataSourceOutputTypeDef(TypedDict):
    StartDate: datetime,
    EndDate: datetime,
    Include: NotRequired[MessageInsightsFiltersOutputTypeDef],  # (1)
    Exclude: NotRequired[MessageInsightsFiltersOutputTypeDef],  # (1)
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: MessageInsightsFiltersOutputTypeDef](./type_defs.md#messageinsightsfiltersoutputtypedef) 
2. See [:material-code-braces: MessageInsightsFiltersOutputTypeDef](./type_defs.md#messageinsightsfiltersoutputtypedef) 
## ReplacementEmailContentTypeDef

```python
# ReplacementEmailContentTypeDef definition

class ReplacementEmailContentTypeDef(TypedDict):
    ReplacementTemplate: NotRequired[ReplacementTemplateTypeDef],  # (1)
```

1. See [:material-code-braces: ReplacementTemplateTypeDef](./type_defs.md#replacementtemplatetypedef) 
## VerificationInfoTypeDef

```python
# VerificationInfoTypeDef definition

class VerificationInfoTypeDef(TypedDict):
    LastCheckedTimestamp: NotRequired[datetime],
    LastSuccessTimestamp: NotRequired[datetime],
    ErrorType: NotRequired[VerificationErrorType],  # (1)
    SOARecord: NotRequired[SOARecordTypeDef],  # (2)
```

1. See [:material-code-brackets: VerificationErrorType](./literals.md#verificationerrortype) 
2. See [:material-code-braces: SOARecordTypeDef](./type_defs.md#soarecordtypedef) 
## SuppressedDestinationTypeDef

```python
# SuppressedDestinationTypeDef definition

class SuppressedDestinationTypeDef(TypedDict):
    EmailAddress: str,
    Reason: SuppressionListReasonType,  # (1)
    LastUpdateTime: datetime,
    Attributes: NotRequired[SuppressedDestinationAttributesTypeDef],  # (2)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
2. See [:material-code-braces: SuppressedDestinationAttributesTypeDef](./type_defs.md#suppresseddestinationattributestypedef) 
## BatchGetMetricDataRequestRequestTypeDef

```python
# BatchGetMetricDataRequestRequestTypeDef definition

class BatchGetMetricDataRequestRequestTypeDef(TypedDict):
    Queries: Sequence[BatchGetMetricDataQueryTypeDef],  # (1)
```

1. See [:material-code-braces: BatchGetMetricDataQueryTypeDef](./type_defs.md#batchgetmetricdataquerytypedef) 
## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    Subject: ContentTypeDef,  # (1)
    Body: BodyTypeDef,  # (2)
    Headers: NotRequired[Sequence[MessageHeaderTypeDef]],  # (3)
```

1. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
2. See [:material-code-braces: BodyTypeDef](./type_defs.md#bodytypedef) 
3. See [:material-code-braces: MessageHeaderTypeDef](./type_defs.md#messageheadertypedef) 
## EventDestinationTypeDef

```python
# EventDestinationTypeDef definition

class EventDestinationTypeDef(TypedDict):
    Name: str,
    MatchingEventTypes: List[EventTypeType],  # (1)
    Enabled: NotRequired[bool],
    KinesisFirehoseDestination: NotRequired[KinesisFirehoseDestinationTypeDef],  # (2)
    CloudWatchDestination: NotRequired[CloudWatchDestinationOutputTypeDef],  # (3)
    SnsDestination: NotRequired[SnsDestinationTypeDef],  # (4)
    EventBridgeDestination: NotRequired[EventBridgeDestinationTypeDef],  # (5)
    PinpointDestination: NotRequired[PinpointDestinationTypeDef],  # (6)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-braces: KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef) 
3. See [:material-code-braces: CloudWatchDestinationOutputTypeDef](./type_defs.md#cloudwatchdestinationoutputtypedef) 
4. See [:material-code-braces: SnsDestinationTypeDef](./type_defs.md#snsdestinationtypedef) 
5. See [:material-code-braces: EventBridgeDestinationTypeDef](./type_defs.md#eventbridgedestinationtypedef) 
6. See [:material-code-braces: PinpointDestinationTypeDef](./type_defs.md#pinpointdestinationtypedef) 
## InsightsEventTypeDef

```python
# InsightsEventTypeDef definition

class InsightsEventTypeDef(TypedDict):
    Timestamp: NotRequired[datetime],
    Type: NotRequired[EventTypeType],  # (1)
    Details: NotRequired[EventDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-braces: EventDetailsTypeDef](./type_defs.md#eventdetailstypedef) 
## ListContactsResponseTypeDef

```python
# ListContactsResponseTypeDef definition

class ListContactsResponseTypeDef(TypedDict):
    Contacts: List[ContactTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BulkEmailContentTypeDef

```python
# BulkEmailContentTypeDef definition

class BulkEmailContentTypeDef(TypedDict):
    Template: NotRequired[TemplateTypeDef],  # (1)
```

1. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
## GetDomainStatisticsReportResponseTypeDef

```python
# GetDomainStatisticsReportResponseTypeDef definition

class GetDomainStatisticsReportResponseTypeDef(TypedDict):
    OverallVolume: OverallVolumeTypeDef,  # (1)
    DailyVolumes: List[DailyVolumeTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: OverallVolumeTypeDef](./type_defs.md#overallvolumetypedef) 
2. See [:material-code-braces: DailyVolumeTypeDef](./type_defs.md#dailyvolumetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMultiRegionEndpointRequestRequestTypeDef

```python
# CreateMultiRegionEndpointRequestRequestTypeDef definition

class CreateMultiRegionEndpointRequestRequestTypeDef(TypedDict):
    EndpointName: str,
    Details: DetailsTypeDef,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: DetailsTypeDef](./type_defs.md#detailstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetDeliverabilityDashboardOptionsResponseTypeDef

```python
# GetDeliverabilityDashboardOptionsResponseTypeDef definition

class GetDeliverabilityDashboardOptionsResponseTypeDef(TypedDict):
    DashboardEnabled: bool,
    SubscriptionExpiryDate: datetime,
    AccountStatus: DeliverabilityDashboardAccountStatusType,  # (1)
    ActiveSubscribedDomains: List[DomainDeliverabilityTrackingOptionOutputTypeDef],  # (2)
    PendingExpirationSubscribedDomains: List[DomainDeliverabilityTrackingOptionOutputTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: DeliverabilityDashboardAccountStatusType](./literals.md#deliverabilitydashboardaccountstatustype) 
2. See [:material-code-braces: DomainDeliverabilityTrackingOptionOutputTypeDef](./type_defs.md#domaindeliverabilitytrackingoptionoutputtypedef) 
3. See [:material-code-braces: DomainDeliverabilityTrackingOptionOutputTypeDef](./type_defs.md#domaindeliverabilitytrackingoptionoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeliverabilityTestReportResponseTypeDef

```python
# GetDeliverabilityTestReportResponseTypeDef definition

class GetDeliverabilityTestReportResponseTypeDef(TypedDict):
    DeliverabilityTestReport: DeliverabilityTestReportTypeDef,  # (1)
    OverallPlacement: PlacementStatisticsTypeDef,  # (2)
    IspPlacements: List[IspPlacementTypeDef],  # (3)
    Message: str,
    Tags: List[TagTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DeliverabilityTestReportTypeDef](./type_defs.md#deliverabilitytestreporttypedef) 
2. See [:material-code-braces: PlacementStatisticsTypeDef](./type_defs.md#placementstatisticstypedef) 
3. See [:material-code-braces: IspPlacementTypeDef](./type_defs.md#ispplacementtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountResponseTypeDef

```python
# GetAccountResponseTypeDef definition

class GetAccountResponseTypeDef(TypedDict):
    DedicatedIpAutoWarmupEnabled: bool,
    EnforcementStatus: str,
    ProductionAccessEnabled: bool,
    SendQuota: SendQuotaTypeDef,  # (1)
    SendingEnabled: bool,
    SuppressionAttributes: SuppressionAttributesTypeDef,  # (2)
    Details: AccountDetailsTypeDef,  # (3)
    VdmAttributes: VdmAttributesTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SendQuotaTypeDef](./type_defs.md#sendquotatypedef) 
2. See [:material-code-braces: SuppressionAttributesTypeDef](./type_defs.md#suppressionattributestypedef) 
3. See [:material-code-braces: AccountDetailsTypeDef](./type_defs.md#accountdetailstypedef) 
4. See [:material-code-braces: VdmAttributesTypeDef](./type_defs.md#vdmattributestypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAccountVdmAttributesRequestRequestTypeDef

```python
# PutAccountVdmAttributesRequestRequestTypeDef definition

class PutAccountVdmAttributesRequestRequestTypeDef(TypedDict):
    VdmAttributes: VdmAttributesTypeDef,  # (1)
```

1. See [:material-code-braces: VdmAttributesTypeDef](./type_defs.md#vdmattributestypedef) 
## CreateConfigurationSetRequestRequestTypeDef

```python
# CreateConfigurationSetRequestRequestTypeDef definition

class CreateConfigurationSetRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    TrackingOptions: NotRequired[TrackingOptionsTypeDef],  # (1)
    DeliveryOptions: NotRequired[DeliveryOptionsTypeDef],  # (2)
    ReputationOptions: NotRequired[ReputationOptionsTypeDef],  # (3)
    SendingOptions: NotRequired[SendingOptionsTypeDef],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
    SuppressionOptions: NotRequired[SuppressionOptionsTypeDef],  # (6)
    VdmOptions: NotRequired[VdmOptionsTypeDef],  # (7)
```

1. See [:material-code-braces: TrackingOptionsTypeDef](./type_defs.md#trackingoptionstypedef) 
2. See [:material-code-braces: DeliveryOptionsTypeDef](./type_defs.md#deliveryoptionstypedef) 
3. See [:material-code-braces: ReputationOptionsTypeDef](./type_defs.md#reputationoptionstypedef) 
4. See [:material-code-braces: SendingOptionsTypeDef](./type_defs.md#sendingoptionstypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: SuppressionOptionsTypeDef](./type_defs.md#suppressionoptionstypedef) 
7. See [:material-code-braces: VdmOptionsTypeDef](./type_defs.md#vdmoptionstypedef) 
## GetConfigurationSetResponseTypeDef

```python
# GetConfigurationSetResponseTypeDef definition

class GetConfigurationSetResponseTypeDef(TypedDict):
    ConfigurationSetName: str,
    TrackingOptions: TrackingOptionsTypeDef,  # (1)
    DeliveryOptions: DeliveryOptionsTypeDef,  # (2)
    ReputationOptions: ReputationOptionsOutputTypeDef,  # (3)
    SendingOptions: SendingOptionsTypeDef,  # (4)
    Tags: List[TagTypeDef],  # (5)
    SuppressionOptions: SuppressionOptionsOutputTypeDef,  # (6)
    VdmOptions: VdmOptionsTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: TrackingOptionsTypeDef](./type_defs.md#trackingoptionstypedef) 
2. See [:material-code-braces: DeliveryOptionsTypeDef](./type_defs.md#deliveryoptionstypedef) 
3. See [:material-code-braces: ReputationOptionsOutputTypeDef](./type_defs.md#reputationoptionsoutputtypedef) 
4. See [:material-code-braces: SendingOptionsTypeDef](./type_defs.md#sendingoptionstypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: SuppressionOptionsOutputTypeDef](./type_defs.md#suppressionoptionsoutputtypedef) 
7. See [:material-code-braces: VdmOptionsTypeDef](./type_defs.md#vdmoptionstypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutConfigurationSetVdmOptionsRequestRequestTypeDef

```python
# PutConfigurationSetVdmOptionsRequestRequestTypeDef definition

class PutConfigurationSetVdmOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    VdmOptions: NotRequired[VdmOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: VdmOptionsTypeDef](./type_defs.md#vdmoptionstypedef) 
## CreateImportJobRequestRequestTypeDef

```python
# CreateImportJobRequestRequestTypeDef definition

class CreateImportJobRequestRequestTypeDef(TypedDict):
    ImportDestination: ImportDestinationTypeDef,  # (1)
    ImportDataSource: ImportDataSourceTypeDef,  # (2)
```

1. See [:material-code-braces: ImportDestinationTypeDef](./type_defs.md#importdestinationtypedef) 
2. See [:material-code-braces: ImportDataSourceTypeDef](./type_defs.md#importdatasourcetypedef) 
## GetImportJobResponseTypeDef

```python
# GetImportJobResponseTypeDef definition

class GetImportJobResponseTypeDef(TypedDict):
    JobId: str,
    ImportDestination: ImportDestinationTypeDef,  # (1)
    ImportDataSource: ImportDataSourceTypeDef,  # (2)
    FailureInfo: FailureInfoTypeDef,  # (3)
    JobStatus: JobStatusType,  # (4)
    CreatedTimestamp: datetime,
    CompletedTimestamp: datetime,
    ProcessedRecordsCount: int,
    FailedRecordsCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ImportDestinationTypeDef](./type_defs.md#importdestinationtypedef) 
2. See [:material-code-braces: ImportDataSourceTypeDef](./type_defs.md#importdatasourcetypedef) 
3. See [:material-code-braces: FailureInfoTypeDef](./type_defs.md#failureinfotypedef) 
4. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportJobSummaryTypeDef

```python
# ImportJobSummaryTypeDef definition

class ImportJobSummaryTypeDef(TypedDict):
    JobId: NotRequired[str],
    ImportDestination: NotRequired[ImportDestinationTypeDef],  # (1)
    JobStatus: NotRequired[JobStatusType],  # (2)
    CreatedTimestamp: NotRequired[datetime],
    ProcessedRecordsCount: NotRequired[int],
    FailedRecordsCount: NotRequired[int],
```

1. See [:material-code-braces: ImportDestinationTypeDef](./type_defs.md#importdestinationtypedef) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## DomainDeliverabilityTrackingOptionTypeDef

```python
# DomainDeliverabilityTrackingOptionTypeDef definition

class DomainDeliverabilityTrackingOptionTypeDef(TypedDict):
    Domain: NotRequired[str],
    SubscriptionStartDate: NotRequired[TimestampTypeDef],
    InboxPlacementTrackingOption: NotRequired[InboxPlacementTrackingOptionUnionTypeDef],  # (1)
```

1. See [:material-code-braces: InboxPlacementTrackingOptionTypeDef](./type_defs.md#inboxplacementtrackingoptiontypedef) [:material-code-braces: InboxPlacementTrackingOptionOutputTypeDef](./type_defs.md#inboxplacementtrackingoptionoutputtypedef) 
## ListContactsRequestRequestTypeDef

```python
# ListContactsRequestRequestTypeDef definition

class ListContactsRequestRequestTypeDef(TypedDict):
    ContactListName: str,
    Filter: NotRequired[ListContactsFilterTypeDef],  # (1)
    PageSize: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListContactsFilterTypeDef](./type_defs.md#listcontactsfiltertypedef) 
## ExportDataSourceOutputTypeDef

```python
# ExportDataSourceOutputTypeDef definition

class ExportDataSourceOutputTypeDef(TypedDict):
    MetricsDataSource: NotRequired[MetricsDataSourceOutputTypeDef],  # (1)
    MessageInsightsDataSource: NotRequired[MessageInsightsDataSourceOutputTypeDef],  # (2)
```

1. See [:material-code-braces: MetricsDataSourceOutputTypeDef](./type_defs.md#metricsdatasourceoutputtypedef) 
2. See [:material-code-braces: MessageInsightsDataSourceOutputTypeDef](./type_defs.md#messageinsightsdatasourceoutputtypedef) 
## MessageInsightsDataSourceTypeDef

```python
# MessageInsightsDataSourceTypeDef definition

class MessageInsightsDataSourceTypeDef(TypedDict):
    StartDate: TimestampTypeDef,
    EndDate: TimestampTypeDef,
    Include: NotRequired[MessageInsightsFiltersUnionTypeDef],  # (1)
    Exclude: NotRequired[MessageInsightsFiltersUnionTypeDef],  # (1)
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: MessageInsightsFiltersTypeDef](./type_defs.md#messageinsightsfilterstypedef) [:material-code-braces: MessageInsightsFiltersOutputTypeDef](./type_defs.md#messageinsightsfiltersoutputtypedef) 
2. See [:material-code-braces: MessageInsightsFiltersTypeDef](./type_defs.md#messageinsightsfilterstypedef) [:material-code-braces: MessageInsightsFiltersOutputTypeDef](./type_defs.md#messageinsightsfiltersoutputtypedef) 
## BulkEmailEntryTypeDef

```python
# BulkEmailEntryTypeDef definition

class BulkEmailEntryTypeDef(TypedDict):
    Destination: DestinationTypeDef,  # (1)
    ReplacementTags: NotRequired[Sequence[MessageTagTypeDef]],  # (2)
    ReplacementEmailContent: NotRequired[ReplacementEmailContentTypeDef],  # (3)
    ReplacementHeaders: NotRequired[Sequence[MessageHeaderTypeDef]],  # (4)
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: MessageTagTypeDef](./type_defs.md#messagetagtypedef) 
3. See [:material-code-braces: ReplacementEmailContentTypeDef](./type_defs.md#replacementemailcontenttypedef) 
4. See [:material-code-braces: MessageHeaderTypeDef](./type_defs.md#messageheadertypedef) 
## GetEmailIdentityResponseTypeDef

```python
# GetEmailIdentityResponseTypeDef definition

class GetEmailIdentityResponseTypeDef(TypedDict):
    IdentityType: IdentityTypeType,  # (1)
    FeedbackForwardingStatus: bool,
    VerifiedForSendingStatus: bool,
    DkimAttributes: DkimAttributesTypeDef,  # (2)
    MailFromAttributes: MailFromAttributesTypeDef,  # (3)
    Policies: Dict[str, str],
    Tags: List[TagTypeDef],  # (4)
    ConfigurationSetName: str,
    VerificationStatus: VerificationStatusType,  # (5)
    VerificationInfo: VerificationInfoTypeDef,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-braces: DkimAttributesTypeDef](./type_defs.md#dkimattributestypedef) 
3. See [:material-code-braces: MailFromAttributesTypeDef](./type_defs.md#mailfromattributestypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-brackets: VerificationStatusType](./literals.md#verificationstatustype) 
6. See [:material-code-braces: VerificationInfoTypeDef](./type_defs.md#verificationinfotypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSuppressedDestinationResponseTypeDef

```python
# GetSuppressedDestinationResponseTypeDef definition

class GetSuppressedDestinationResponseTypeDef(TypedDict):
    SuppressedDestination: SuppressedDestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SuppressedDestinationTypeDef](./type_defs.md#suppresseddestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmailContentTypeDef

```python
# EmailContentTypeDef definition

class EmailContentTypeDef(TypedDict):
    Simple: NotRequired[MessageTypeDef],  # (1)
    Raw: NotRequired[RawMessageTypeDef],  # (2)
    Template: NotRequired[TemplateTypeDef],  # (3)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: RawMessageTypeDef](./type_defs.md#rawmessagetypedef) 
3. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
## GetConfigurationSetEventDestinationsResponseTypeDef

```python
# GetConfigurationSetEventDestinationsResponseTypeDef definition

class GetConfigurationSetEventDestinationsResponseTypeDef(TypedDict):
    EventDestinations: List[EventDestinationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventDestinationDefinitionTypeDef

```python
# EventDestinationDefinitionTypeDef definition

class EventDestinationDefinitionTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    MatchingEventTypes: NotRequired[Sequence[EventTypeType]],  # (1)
    KinesisFirehoseDestination: NotRequired[KinesisFirehoseDestinationTypeDef],  # (2)
    CloudWatchDestination: NotRequired[CloudWatchDestinationUnionTypeDef],  # (3)
    SnsDestination: NotRequired[SnsDestinationTypeDef],  # (4)
    EventBridgeDestination: NotRequired[EventBridgeDestinationTypeDef],  # (5)
    PinpointDestination: NotRequired[PinpointDestinationTypeDef],  # (6)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-braces: KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef) 
3. See [:material-code-braces: CloudWatchDestinationTypeDef](./type_defs.md#cloudwatchdestinationtypedef) [:material-code-braces: CloudWatchDestinationOutputTypeDef](./type_defs.md#cloudwatchdestinationoutputtypedef) 
4. See [:material-code-braces: SnsDestinationTypeDef](./type_defs.md#snsdestinationtypedef) 
5. See [:material-code-braces: EventBridgeDestinationTypeDef](./type_defs.md#eventbridgedestinationtypedef) 
6. See [:material-code-braces: PinpointDestinationTypeDef](./type_defs.md#pinpointdestinationtypedef) 
## EmailInsightsTypeDef

```python
# EmailInsightsTypeDef definition

class EmailInsightsTypeDef(TypedDict):
    Destination: NotRequired[str],
    Isp: NotRequired[str],
    Events: NotRequired[List[InsightsEventTypeDef]],  # (1)
```

1. See [:material-code-braces: InsightsEventTypeDef](./type_defs.md#insightseventtypedef) 
## ListImportJobsResponseTypeDef

```python
# ListImportJobsResponseTypeDef definition

class ListImportJobsResponseTypeDef(TypedDict):
    ImportJobs: List[ImportJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportJobSummaryTypeDef](./type_defs.md#importjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExportJobResponseTypeDef

```python
# GetExportJobResponseTypeDef definition

class GetExportJobResponseTypeDef(TypedDict):
    JobId: str,
    ExportSourceType: ExportSourceTypeType,  # (1)
    JobStatus: JobStatusType,  # (2)
    ExportDestination: ExportDestinationTypeDef,  # (3)
    ExportDataSource: ExportDataSourceOutputTypeDef,  # (4)
    CreatedTimestamp: datetime,
    CompletedTimestamp: datetime,
    FailureInfo: FailureInfoTypeDef,  # (5)
    Statistics: ExportStatisticsTypeDef,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: ExportSourceTypeType](./literals.md#exportsourcetypetype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: ExportDestinationTypeDef](./type_defs.md#exportdestinationtypedef) 
4. See [:material-code-braces: ExportDataSourceOutputTypeDef](./type_defs.md#exportdatasourceoutputtypedef) 
5. See [:material-code-braces: FailureInfoTypeDef](./type_defs.md#failureinfotypedef) 
6. See [:material-code-braces: ExportStatisticsTypeDef](./type_defs.md#exportstatisticstypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendBulkEmailRequestRequestTypeDef

```python
# SendBulkEmailRequestRequestTypeDef definition

class SendBulkEmailRequestRequestTypeDef(TypedDict):
    DefaultContent: BulkEmailContentTypeDef,  # (1)
    BulkEmailEntries: Sequence[BulkEmailEntryTypeDef],  # (2)
    FromEmailAddress: NotRequired[str],
    FromEmailAddressIdentityArn: NotRequired[str],
    ReplyToAddresses: NotRequired[Sequence[str]],
    FeedbackForwardingEmailAddress: NotRequired[str],
    FeedbackForwardingEmailAddressIdentityArn: NotRequired[str],
    DefaultEmailTags: NotRequired[Sequence[MessageTagTypeDef]],  # (3)
    ConfigurationSetName: NotRequired[str],
    EndpointId: NotRequired[str],
```

1. See [:material-code-braces: BulkEmailContentTypeDef](./type_defs.md#bulkemailcontenttypedef) 
2. See [:material-code-braces: BulkEmailEntryTypeDef](./type_defs.md#bulkemailentrytypedef) 
3. See [:material-code-braces: MessageTagTypeDef](./type_defs.md#messagetagtypedef) 
## CreateDeliverabilityTestReportRequestRequestTypeDef

```python
# CreateDeliverabilityTestReportRequestRequestTypeDef definition

class CreateDeliverabilityTestReportRequestRequestTypeDef(TypedDict):
    FromEmailAddress: str,
    Content: EmailContentTypeDef,  # (1)
    ReportName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: EmailContentTypeDef](./type_defs.md#emailcontenttypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## SendEmailRequestRequestTypeDef

```python
# SendEmailRequestRequestTypeDef definition

class SendEmailRequestRequestTypeDef(TypedDict):
    Content: EmailContentTypeDef,  # (1)
    FromEmailAddress: NotRequired[str],
    FromEmailAddressIdentityArn: NotRequired[str],
    Destination: NotRequired[DestinationTypeDef],  # (2)
    ReplyToAddresses: NotRequired[Sequence[str]],
    FeedbackForwardingEmailAddress: NotRequired[str],
    FeedbackForwardingEmailAddressIdentityArn: NotRequired[str],
    EmailTags: NotRequired[Sequence[MessageTagTypeDef]],  # (3)
    ConfigurationSetName: NotRequired[str],
    EndpointId: NotRequired[str],
    ListManagementOptions: NotRequired[ListManagementOptionsTypeDef],  # (4)
```

1. See [:material-code-braces: EmailContentTypeDef](./type_defs.md#emailcontenttypedef) 
2. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
3. See [:material-code-braces: MessageTagTypeDef](./type_defs.md#messagetagtypedef) 
4. See [:material-code-braces: ListManagementOptionsTypeDef](./type_defs.md#listmanagementoptionstypedef) 
## CreateConfigurationSetEventDestinationRequestRequestTypeDef

```python
# CreateConfigurationSetEventDestinationRequestRequestTypeDef definition

class CreateConfigurationSetEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
    EventDestination: EventDestinationDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 
## UpdateConfigurationSetEventDestinationRequestRequestTypeDef

```python
# UpdateConfigurationSetEventDestinationRequestRequestTypeDef definition

class UpdateConfigurationSetEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
    EventDestination: EventDestinationDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 
## GetMessageInsightsResponseTypeDef

```python
# GetMessageInsightsResponseTypeDef definition

class GetMessageInsightsResponseTypeDef(TypedDict):
    MessageId: str,
    FromEmailAddress: str,
    Subject: str,
    EmailTags: List[MessageTagTypeDef],  # (1)
    Insights: List[EmailInsightsTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MessageTagTypeDef](./type_defs.md#messagetagtypedef) 
2. See [:material-code-braces: EmailInsightsTypeDef](./type_defs.md#emailinsightstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDeliverabilityDashboardOptionRequestRequestTypeDef

```python
# PutDeliverabilityDashboardOptionRequestRequestTypeDef definition

class PutDeliverabilityDashboardOptionRequestRequestTypeDef(TypedDict):
    DashboardEnabled: bool,
    SubscribedDomains: NotRequired[Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: DomainDeliverabilityTrackingOptionTypeDef](./type_defs.md#domaindeliverabilitytrackingoptiontypedef) [:material-code-braces: DomainDeliverabilityTrackingOptionOutputTypeDef](./type_defs.md#domaindeliverabilitytrackingoptionoutputtypedef) 
## ExportDataSourceTypeDef

```python
# ExportDataSourceTypeDef definition

class ExportDataSourceTypeDef(TypedDict):
    MetricsDataSource: NotRequired[MetricsDataSourceUnionTypeDef],  # (1)
    MessageInsightsDataSource: NotRequired[MessageInsightsDataSourceUnionTypeDef],  # (2)
```

1. See [:material-code-braces: MetricsDataSourceTypeDef](./type_defs.md#metricsdatasourcetypedef) [:material-code-braces: MetricsDataSourceOutputTypeDef](./type_defs.md#metricsdatasourceoutputtypedef) 
2. See [:material-code-braces: MessageInsightsDataSourceTypeDef](./type_defs.md#messageinsightsdatasourcetypedef) [:material-code-braces: MessageInsightsDataSourceOutputTypeDef](./type_defs.md#messageinsightsdatasourceoutputtypedef) 
## CreateExportJobRequestRequestTypeDef

```python
# CreateExportJobRequestRequestTypeDef definition

class CreateExportJobRequestRequestTypeDef(TypedDict):
    ExportDataSource: ExportDataSourceTypeDef,  # (1)
    ExportDestination: ExportDestinationTypeDef,  # (2)
```

1. See [:material-code-braces: ExportDataSourceTypeDef](./type_defs.md#exportdatasourcetypedef) 
2. See [:material-code-braces: ExportDestinationTypeDef](./type_defs.md#exportdestinationtypedef) 
