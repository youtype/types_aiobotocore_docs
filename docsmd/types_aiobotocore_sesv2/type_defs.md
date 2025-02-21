# Type definitions

> [Index](../README.md) > [SESV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SESV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#sesv2)
    type annotations stubs module [types-aiobotocore-sesv2](https://pypi.org/project/types-aiobotocore-sesv2/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_sesv2.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_sesv2.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


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
# InboxPlacementTrackingOptionUnionTypeDef Union usage example

from types_aiobotocore_sesv2.type_defs import InboxPlacementTrackingOptionUnionTypeDef


def get_value() -> InboxPlacementTrackingOptionUnionTypeDef:
    return ...


# InboxPlacementTrackingOptionUnionTypeDef definition

InboxPlacementTrackingOptionUnionTypeDef = Union[
    InboxPlacementTrackingOptionTypeDef,  # (1)
    InboxPlacementTrackingOptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InboxPlacementTrackingOptionTypeDef](./type_defs.md#inboxplacementtrackingoptiontypedef) 
2. See [:material-code-braces: InboxPlacementTrackingOptionOutputTypeDef](./type_defs.md#inboxplacementtrackingoptionoutputtypedef) 

## SuppressionOptionsUnionTypeDef

```python
# SuppressionOptionsUnionTypeDef Union usage example

from types_aiobotocore_sesv2.type_defs import SuppressionOptionsUnionTypeDef


def get_value() -> SuppressionOptionsUnionTypeDef:
    return ...


# SuppressionOptionsUnionTypeDef definition

SuppressionOptionsUnionTypeDef = Union[
    SuppressionOptionsTypeDef,  # (1)
    SuppressionOptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SuppressionOptionsTypeDef](./type_defs.md#suppressionoptionstypedef) 
2. See [:material-code-braces: SuppressionOptionsOutputTypeDef](./type_defs.md#suppressionoptionsoutputtypedef) 

## ReputationOptionsUnionTypeDef

```python
# ReputationOptionsUnionTypeDef Union usage example

from types_aiobotocore_sesv2.type_defs import ReputationOptionsUnionTypeDef


def get_value() -> ReputationOptionsUnionTypeDef:
    return ...


# ReputationOptionsUnionTypeDef definition

ReputationOptionsUnionTypeDef = Union[
    ReputationOptionsTypeDef,  # (1)
    ReputationOptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ReputationOptionsTypeDef](./type_defs.md#reputationoptionstypedef) 
2. See [:material-code-braces: ReputationOptionsOutputTypeDef](./type_defs.md#reputationoptionsoutputtypedef) 

## CloudWatchDestinationUnionTypeDef

```python
# CloudWatchDestinationUnionTypeDef Union usage example

from types_aiobotocore_sesv2.type_defs import CloudWatchDestinationUnionTypeDef


def get_value() -> CloudWatchDestinationUnionTypeDef:
    return ...


# CloudWatchDestinationUnionTypeDef definition

CloudWatchDestinationUnionTypeDef = Union[
    CloudWatchDestinationTypeDef,  # (1)
    CloudWatchDestinationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CloudWatchDestinationTypeDef](./type_defs.md#cloudwatchdestinationtypedef) 
2. See [:material-code-braces: CloudWatchDestinationOutputTypeDef](./type_defs.md#cloudwatchdestinationoutputtypedef) 

## DomainDeliverabilityTrackingOptionUnionTypeDef

```python
# DomainDeliverabilityTrackingOptionUnionTypeDef Union usage example

from types_aiobotocore_sesv2.type_defs import DomainDeliverabilityTrackingOptionUnionTypeDef


def get_value() -> DomainDeliverabilityTrackingOptionUnionTypeDef:
    return ...


# DomainDeliverabilityTrackingOptionUnionTypeDef definition

DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
    DomainDeliverabilityTrackingOptionTypeDef,  # (1)
    DomainDeliverabilityTrackingOptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DomainDeliverabilityTrackingOptionTypeDef](./type_defs.md#domaindeliverabilitytrackingoptiontypedef) 
2. See [:material-code-braces: DomainDeliverabilityTrackingOptionOutputTypeDef](./type_defs.md#domaindeliverabilitytrackingoptionoutputtypedef) 

## ExportDataSourceUnionTypeDef

```python
# ExportDataSourceUnionTypeDef Union usage example

from types_aiobotocore_sesv2.type_defs import ExportDataSourceUnionTypeDef


def get_value() -> ExportDataSourceUnionTypeDef:
    return ...


# ExportDataSourceUnionTypeDef definition

ExportDataSourceUnionTypeDef = Union[
    ExportDataSourceTypeDef,  # (1)
    ExportDataSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ExportDataSourceTypeDef](./type_defs.md#exportdatasourcetypedef) 
2. See [:material-code-braces: ExportDataSourceOutputTypeDef](./type_defs.md#exportdatasourceoutputtypedef) 



## ReviewDetailsTypeDef

```python
# ReviewDetailsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ReviewDetailsTypeDef


def get_value() -> ReviewDetailsTypeDef:
    return {
        "Status": ...,
    }


# ReviewDetailsTypeDef definition

class ReviewDetailsTypeDef(TypedDict):
    Status: NotRequired[ReviewStatusType],  # (1)
    CaseId: NotRequired[str],
```

1. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
## ArchivingOptionsTypeDef

```python
# ArchivingOptionsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ArchivingOptionsTypeDef


def get_value() -> ArchivingOptionsTypeDef:
    return {
        "ArchiveArn": ...,
    }


# ArchivingOptionsTypeDef definition

class ArchivingOptionsTypeDef(TypedDict):
    ArchiveArn: NotRequired[str],
```

## MetricDataErrorTypeDef

```python
# MetricDataErrorTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import MetricDataErrorTypeDef


def get_value() -> MetricDataErrorTypeDef:
    return {
        "Id": ...,
    }


# MetricDataErrorTypeDef definition

class MetricDataErrorTypeDef(TypedDict):
    Id: NotRequired[str],
    Code: NotRequired[QueryErrorCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: QueryErrorCodeType](./literals.md#queryerrorcodetype) 
## MetricDataResultTypeDef

```python
# MetricDataResultTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import MetricDataResultTypeDef


def get_value() -> MetricDataResultTypeDef:
    return {
        "Id": ...,
    }


# MetricDataResultTypeDef definition

class MetricDataResultTypeDef(TypedDict):
    Id: NotRequired[str],
    Timestamps: NotRequired[List[datetime]],
    Values: NotRequired[List[int]],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


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
# BlacklistEntryTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import BlacklistEntryTypeDef


def get_value() -> BlacklistEntryTypeDef:
    return {
        "RblName": ...,
    }


# BlacklistEntryTypeDef definition

class BlacklistEntryTypeDef(TypedDict):
    RblName: NotRequired[str],
    ListingTime: NotRequired[datetime],
    Description: NotRequired[str],
```

## ContentTypeDef

```python
# ContentTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ContentTypeDef


def get_value() -> ContentTypeDef:
    return {
        "Data": ...,
    }


# ContentTypeDef definition

class ContentTypeDef(TypedDict):
    Data: str,
    Charset: NotRequired[str],
```

## BounceTypeDef

```python
# BounceTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import BounceTypeDef


def get_value() -> BounceTypeDef:
    return {
        "BounceType": ...,
    }


# BounceTypeDef definition

class BounceTypeDef(TypedDict):
    BounceType: NotRequired[BounceTypeType],  # (1)
    BounceSubType: NotRequired[str],
    DiagnosticCode: NotRequired[str],
```

1. See [:material-code-brackets: BounceTypeType](./literals.md#bouncetypetype) 
## BulkEmailEntryResultTypeDef

```python
# BulkEmailEntryResultTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import BulkEmailEntryResultTypeDef


def get_value() -> BulkEmailEntryResultTypeDef:
    return {
        "Status": ...,
    }


# BulkEmailEntryResultTypeDef definition

class BulkEmailEntryResultTypeDef(TypedDict):
    Status: NotRequired[BulkEmailStatusType],  # (1)
    Error: NotRequired[str],
    MessageId: NotRequired[str],
```

1. See [:material-code-brackets: BulkEmailStatusType](./literals.md#bulkemailstatustype) 
## DestinationTypeDef

```python
# DestinationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DestinationTypeDef


def get_value() -> DestinationTypeDef:
    return {
        "ToAddresses": ...,
    }


# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    ToAddresses: NotRequired[Sequence[str]],
    CcAddresses: NotRequired[Sequence[str]],
    BccAddresses: NotRequired[Sequence[str]],
```

## MessageHeaderTypeDef

```python
# MessageHeaderTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import MessageHeaderTypeDef


def get_value() -> MessageHeaderTypeDef:
    return {
        "Name": ...,
    }


# MessageHeaderTypeDef definition

class MessageHeaderTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## MessageTagTypeDef

```python
# MessageTagTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import MessageTagTypeDef


def get_value() -> MessageTagTypeDef:
    return {
        "Name": ...,
    }


# MessageTagTypeDef definition

class MessageTagTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## CancelExportJobRequestTypeDef

```python
# CancelExportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CancelExportJobRequestTypeDef


def get_value() -> CancelExportJobRequestTypeDef:
    return {
        "JobId": ...,
    }


# CancelExportJobRequestTypeDef definition

class CancelExportJobRequestTypeDef(TypedDict):
    JobId: str,
```

## CloudWatchDimensionConfigurationTypeDef

```python
# CloudWatchDimensionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CloudWatchDimensionConfigurationTypeDef


def get_value() -> CloudWatchDimensionConfigurationTypeDef:
    return {
        "DimensionName": ...,
    }


# CloudWatchDimensionConfigurationTypeDef definition

class CloudWatchDimensionConfigurationTypeDef(TypedDict):
    DimensionName: str,
    DimensionValueSource: DimensionValueSourceType,  # (1)
    DefaultDimensionValue: str,
```

1. See [:material-code-brackets: DimensionValueSourceType](./literals.md#dimensionvaluesourcetype) 
## ComplaintTypeDef

```python
# ComplaintTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ComplaintTypeDef


def get_value() -> ComplaintTypeDef:
    return {
        "ComplaintSubType": ...,
    }


# ComplaintTypeDef definition

class ComplaintTypeDef(TypedDict):
    ComplaintSubType: NotRequired[str],
    ComplaintFeedbackType: NotRequired[str],
```

## ContactListDestinationTypeDef

```python
# ContactListDestinationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ContactListDestinationTypeDef


def get_value() -> ContactListDestinationTypeDef:
    return {
        "ContactListName": ...,
    }


# ContactListDestinationTypeDef definition

class ContactListDestinationTypeDef(TypedDict):
    ContactListName: str,
    ContactListImportAction: ContactListImportActionType,  # (1)
```

1. See [:material-code-brackets: ContactListImportActionType](./literals.md#contactlistimportactiontype) 
## ContactListTypeDef

```python
# ContactListTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ContactListTypeDef


def get_value() -> ContactListTypeDef:
    return {
        "ContactListName": ...,
    }


# ContactListTypeDef definition

class ContactListTypeDef(TypedDict):
    ContactListName: NotRequired[str],
    LastUpdatedTimestamp: NotRequired[datetime],
```

## TopicPreferenceTypeDef

```python
# TopicPreferenceTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import TopicPreferenceTypeDef


def get_value() -> TopicPreferenceTypeDef:
    return {
        "TopicName": ...,
    }


# TopicPreferenceTypeDef definition

class TopicPreferenceTypeDef(TypedDict):
    TopicName: str,
    SubscriptionStatus: SubscriptionStatusType,  # (1)
```

1. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
## DeliveryOptionsTypeDef

```python
# DeliveryOptionsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeliveryOptionsTypeDef


def get_value() -> DeliveryOptionsTypeDef:
    return {
        "TlsPolicy": ...,
    }


# DeliveryOptionsTypeDef definition

class DeliveryOptionsTypeDef(TypedDict):
    TlsPolicy: NotRequired[TlsPolicyType],  # (1)
    SendingPoolName: NotRequired[str],
    MaxDeliverySeconds: NotRequired[int],
```

1. See [:material-code-brackets: TlsPolicyType](./literals.md#tlspolicytype) 
## SendingOptionsTypeDef

```python
# SendingOptionsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SendingOptionsTypeDef


def get_value() -> SendingOptionsTypeDef:
    return {
        "SendingEnabled": ...,
    }


# SendingOptionsTypeDef definition

class SendingOptionsTypeDef(TypedDict):
    SendingEnabled: NotRequired[bool],
```

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## TrackingOptionsTypeDef

```python
# TrackingOptionsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import TrackingOptionsTypeDef


def get_value() -> TrackingOptionsTypeDef:
    return {
        "CustomRedirectDomain": ...,
    }


# TrackingOptionsTypeDef definition

class TrackingOptionsTypeDef(TypedDict):
    CustomRedirectDomain: str,
    HttpsPolicy: NotRequired[HttpsPolicyType],  # (1)
```

1. See [:material-code-brackets: HttpsPolicyType](./literals.md#httpspolicytype) 
## TopicTypeDef

```python
# TopicTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import TopicTypeDef


def get_value() -> TopicTypeDef:
    return {
        "TopicName": ...,
    }


# TopicTypeDef definition

class TopicTypeDef(TypedDict):
    TopicName: str,
    DisplayName: str,
    DefaultSubscriptionStatus: SubscriptionStatusType,  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
## CreateCustomVerificationEmailTemplateRequestTypeDef

```python
# CreateCustomVerificationEmailTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateCustomVerificationEmailTemplateRequestTypeDef


def get_value() -> CreateCustomVerificationEmailTemplateRequestTypeDef:
    return {
        "TemplateName": ...,
    }


# CreateCustomVerificationEmailTemplateRequestTypeDef definition

class CreateCustomVerificationEmailTemplateRequestTypeDef(TypedDict):
    TemplateName: str,
    FromEmailAddress: str,
    TemplateSubject: str,
    TemplateContent: str,
    SuccessRedirectionURL: str,
    FailureRedirectionURL: str,
```

## CreateEmailIdentityPolicyRequestTypeDef

```python
# CreateEmailIdentityPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateEmailIdentityPolicyRequestTypeDef


def get_value() -> CreateEmailIdentityPolicyRequestTypeDef:
    return {
        "EmailIdentity": ...,
    }


# CreateEmailIdentityPolicyRequestTypeDef definition

class CreateEmailIdentityPolicyRequestTypeDef(TypedDict):
    EmailIdentity: str,
    PolicyName: str,
    Policy: str,
```

## DkimSigningAttributesTypeDef

```python
# DkimSigningAttributesTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DkimSigningAttributesTypeDef


def get_value() -> DkimSigningAttributesTypeDef:
    return {
        "DomainSigningSelector": ...,
    }


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
# DkimAttributesTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DkimAttributesTypeDef


def get_value() -> DkimAttributesTypeDef:
    return {
        "SigningEnabled": ...,
    }


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
# EmailTemplateContentTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import EmailTemplateContentTypeDef


def get_value() -> EmailTemplateContentTypeDef:
    return {
        "Subject": ...,
    }


# EmailTemplateContentTypeDef definition

class EmailTemplateContentTypeDef(TypedDict):
    Subject: NotRequired[str],
    Text: NotRequired[str],
    Html: NotRequired[str],
```

## ExportDestinationTypeDef

```python
# ExportDestinationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ExportDestinationTypeDef


def get_value() -> ExportDestinationTypeDef:
    return {
        "DataFormat": ...,
    }


# ExportDestinationTypeDef definition

class ExportDestinationTypeDef(TypedDict):
    DataFormat: DataFormatType,  # (1)
    S3Url: NotRequired[str],
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
## ImportDataSourceTypeDef

```python
# ImportDataSourceTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ImportDataSourceTypeDef


def get_value() -> ImportDataSourceTypeDef:
    return {
        "S3Url": ...,
    }


# ImportDataSourceTypeDef definition

class ImportDataSourceTypeDef(TypedDict):
    S3Url: str,
    DataFormat: DataFormatType,  # (1)
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
## CustomVerificationEmailTemplateMetadataTypeDef

```python
# CustomVerificationEmailTemplateMetadataTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CustomVerificationEmailTemplateMetadataTypeDef


def get_value() -> CustomVerificationEmailTemplateMetadataTypeDef:
    return {
        "TemplateName": ...,
    }


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
# DomainIspPlacementTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DomainIspPlacementTypeDef


def get_value() -> DomainIspPlacementTypeDef:
    return {
        "IspName": ...,
    }


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
# VolumeStatisticsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import VolumeStatisticsTypeDef


def get_value() -> VolumeStatisticsTypeDef:
    return {
        "InboxRawCount": ...,
    }


# VolumeStatisticsTypeDef definition

class VolumeStatisticsTypeDef(TypedDict):
    InboxRawCount: NotRequired[int],
    SpamRawCount: NotRequired[int],
    ProjectedInbox: NotRequired[int],
    ProjectedSpam: NotRequired[int],
```

## DashboardAttributesTypeDef

```python
# DashboardAttributesTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DashboardAttributesTypeDef


def get_value() -> DashboardAttributesTypeDef:
    return {
        "EngagementMetrics": ...,
    }


# DashboardAttributesTypeDef definition

class DashboardAttributesTypeDef(TypedDict):
    EngagementMetrics: NotRequired[FeatureStatusType],  # (1)
```

1. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## DashboardOptionsTypeDef

```python
# DashboardOptionsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DashboardOptionsTypeDef


def get_value() -> DashboardOptionsTypeDef:
    return {
        "EngagementMetrics": ...,
    }


# DashboardOptionsTypeDef definition

class DashboardOptionsTypeDef(TypedDict):
    EngagementMetrics: NotRequired[FeatureStatusType],  # (1)
```

1. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## DedicatedIpPoolTypeDef

```python
# DedicatedIpPoolTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DedicatedIpPoolTypeDef


def get_value() -> DedicatedIpPoolTypeDef:
    return {
        "PoolName": ...,
    }


# DedicatedIpPoolTypeDef definition

class DedicatedIpPoolTypeDef(TypedDict):
    PoolName: str,
    ScalingMode: ScalingModeType,  # (1)
```

1. See [:material-code-brackets: ScalingModeType](./literals.md#scalingmodetype) 
## DedicatedIpTypeDef

```python
# DedicatedIpTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DedicatedIpTypeDef


def get_value() -> DedicatedIpTypeDef:
    return {
        "Ip": ...,
    }


# DedicatedIpTypeDef definition

class DedicatedIpTypeDef(TypedDict):
    Ip: str,
    WarmupStatus: WarmupStatusType,  # (1)
    WarmupPercentage: int,
    PoolName: NotRequired[str],
```

1. See [:material-code-brackets: WarmupStatusType](./literals.md#warmupstatustype) 
## DeleteConfigurationSetEventDestinationRequestTypeDef

```python
# DeleteConfigurationSetEventDestinationRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeleteConfigurationSetEventDestinationRequestTypeDef


def get_value() -> DeleteConfigurationSetEventDestinationRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# DeleteConfigurationSetEventDestinationRequestTypeDef definition

class DeleteConfigurationSetEventDestinationRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
```

## DeleteConfigurationSetRequestTypeDef

```python
# DeleteConfigurationSetRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeleteConfigurationSetRequestTypeDef


def get_value() -> DeleteConfigurationSetRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# DeleteConfigurationSetRequestTypeDef definition

class DeleteConfigurationSetRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## DeleteContactListRequestTypeDef

```python
# DeleteContactListRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeleteContactListRequestTypeDef


def get_value() -> DeleteContactListRequestTypeDef:
    return {
        "ContactListName": ...,
    }


# DeleteContactListRequestTypeDef definition

class DeleteContactListRequestTypeDef(TypedDict):
    ContactListName: str,
```

## DeleteContactRequestTypeDef

```python
# DeleteContactRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeleteContactRequestTypeDef


def get_value() -> DeleteContactRequestTypeDef:
    return {
        "ContactListName": ...,
    }


# DeleteContactRequestTypeDef definition

class DeleteContactRequestTypeDef(TypedDict):
    ContactListName: str,
    EmailAddress: str,
```

## DeleteCustomVerificationEmailTemplateRequestTypeDef

```python
# DeleteCustomVerificationEmailTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeleteCustomVerificationEmailTemplateRequestTypeDef


def get_value() -> DeleteCustomVerificationEmailTemplateRequestTypeDef:
    return {
        "TemplateName": ...,
    }


# DeleteCustomVerificationEmailTemplateRequestTypeDef definition

class DeleteCustomVerificationEmailTemplateRequestTypeDef(TypedDict):
    TemplateName: str,
```

## DeleteDedicatedIpPoolRequestTypeDef

```python
# DeleteDedicatedIpPoolRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeleteDedicatedIpPoolRequestTypeDef


def get_value() -> DeleteDedicatedIpPoolRequestTypeDef:
    return {
        "PoolName": ...,
    }


# DeleteDedicatedIpPoolRequestTypeDef definition

class DeleteDedicatedIpPoolRequestTypeDef(TypedDict):
    PoolName: str,
```

## DeleteEmailIdentityPolicyRequestTypeDef

```python
# DeleteEmailIdentityPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeleteEmailIdentityPolicyRequestTypeDef


def get_value() -> DeleteEmailIdentityPolicyRequestTypeDef:
    return {
        "EmailIdentity": ...,
    }


# DeleteEmailIdentityPolicyRequestTypeDef definition

class DeleteEmailIdentityPolicyRequestTypeDef(TypedDict):
    EmailIdentity: str,
    PolicyName: str,
```

## DeleteEmailIdentityRequestTypeDef

```python
# DeleteEmailIdentityRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeleteEmailIdentityRequestTypeDef


def get_value() -> DeleteEmailIdentityRequestTypeDef:
    return {
        "EmailIdentity": ...,
    }


# DeleteEmailIdentityRequestTypeDef definition

class DeleteEmailIdentityRequestTypeDef(TypedDict):
    EmailIdentity: str,
```

## DeleteEmailTemplateRequestTypeDef

```python
# DeleteEmailTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeleteEmailTemplateRequestTypeDef


def get_value() -> DeleteEmailTemplateRequestTypeDef:
    return {
        "TemplateName": ...,
    }


# DeleteEmailTemplateRequestTypeDef definition

class DeleteEmailTemplateRequestTypeDef(TypedDict):
    TemplateName: str,
```

## DeleteMultiRegionEndpointRequestTypeDef

```python
# DeleteMultiRegionEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeleteMultiRegionEndpointRequestTypeDef


def get_value() -> DeleteMultiRegionEndpointRequestTypeDef:
    return {
        "EndpointName": ...,
    }


# DeleteMultiRegionEndpointRequestTypeDef definition

class DeleteMultiRegionEndpointRequestTypeDef(TypedDict):
    EndpointName: str,
```

## DeleteSuppressedDestinationRequestTypeDef

```python
# DeleteSuppressedDestinationRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeleteSuppressedDestinationRequestTypeDef


def get_value() -> DeleteSuppressedDestinationRequestTypeDef:
    return {
        "EmailAddress": ...,
    }


# DeleteSuppressedDestinationRequestTypeDef definition

class DeleteSuppressedDestinationRequestTypeDef(TypedDict):
    EmailAddress: str,
```

## DeliverabilityTestReportTypeDef

```python
# DeliverabilityTestReportTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeliverabilityTestReportTypeDef


def get_value() -> DeliverabilityTestReportTypeDef:
    return {
        "ReportId": ...,
    }


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
# RouteDetailsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import RouteDetailsTypeDef


def get_value() -> RouteDetailsTypeDef:
    return {
        "Region": ...,
    }


# RouteDetailsTypeDef definition

class RouteDetailsTypeDef(TypedDict):
    Region: str,
```

## DomainDeliverabilityCampaignTypeDef

```python
# DomainDeliverabilityCampaignTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DomainDeliverabilityCampaignTypeDef


def get_value() -> DomainDeliverabilityCampaignTypeDef:
    return {
        "CampaignId": ...,
    }


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
# InboxPlacementTrackingOptionOutputTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import InboxPlacementTrackingOptionOutputTypeDef


def get_value() -> InboxPlacementTrackingOptionOutputTypeDef:
    return {
        "Global": ...,
    }


# InboxPlacementTrackingOptionOutputTypeDef definition

class InboxPlacementTrackingOptionOutputTypeDef(TypedDict):
    Global: NotRequired[bool],
    TrackedIsps: NotRequired[List[str]],
```

## EmailTemplateMetadataTypeDef

```python
# EmailTemplateMetadataTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import EmailTemplateMetadataTypeDef


def get_value() -> EmailTemplateMetadataTypeDef:
    return {
        "TemplateName": ...,
    }


# EmailTemplateMetadataTypeDef definition

class EmailTemplateMetadataTypeDef(TypedDict):
    TemplateName: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
```

## EventBridgeDestinationTypeDef

```python
# EventBridgeDestinationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import EventBridgeDestinationTypeDef


def get_value() -> EventBridgeDestinationTypeDef:
    return {
        "EventBusArn": ...,
    }


# EventBridgeDestinationTypeDef definition

class EventBridgeDestinationTypeDef(TypedDict):
    EventBusArn: str,
```

## KinesisFirehoseDestinationTypeDef

```python
# KinesisFirehoseDestinationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import KinesisFirehoseDestinationTypeDef


def get_value() -> KinesisFirehoseDestinationTypeDef:
    return {
        "IamRoleArn": ...,
    }


# KinesisFirehoseDestinationTypeDef definition

class KinesisFirehoseDestinationTypeDef(TypedDict):
    IamRoleArn: str,
    DeliveryStreamArn: str,
```

## PinpointDestinationTypeDef

```python
# PinpointDestinationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PinpointDestinationTypeDef


def get_value() -> PinpointDestinationTypeDef:
    return {
        "ApplicationArn": ...,
    }


# PinpointDestinationTypeDef definition

class PinpointDestinationTypeDef(TypedDict):
    ApplicationArn: NotRequired[str],
```

## SnsDestinationTypeDef

```python
# SnsDestinationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SnsDestinationTypeDef


def get_value() -> SnsDestinationTypeDef:
    return {
        "TopicArn": ...,
    }


# SnsDestinationTypeDef definition

class SnsDestinationTypeDef(TypedDict):
    TopicArn: str,
```

## ExportJobSummaryTypeDef

```python
# ExportJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ExportJobSummaryTypeDef


def get_value() -> ExportJobSummaryTypeDef:
    return {
        "JobId": ...,
    }


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
# ExportMetricTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ExportMetricTypeDef


def get_value() -> ExportMetricTypeDef:
    return {
        "Name": ...,
    }


# ExportMetricTypeDef definition

class ExportMetricTypeDef(TypedDict):
    Name: NotRequired[MetricType],  # (1)
    Aggregation: NotRequired[MetricAggregationType],  # (2)
```

1. See [:material-code-brackets: MetricType](./literals.md#metrictype) 
2. See [:material-code-brackets: MetricAggregationType](./literals.md#metricaggregationtype) 
## ExportStatisticsTypeDef

```python
# ExportStatisticsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ExportStatisticsTypeDef


def get_value() -> ExportStatisticsTypeDef:
    return {
        "ProcessedRecordsCount": ...,
    }


# ExportStatisticsTypeDef definition

class ExportStatisticsTypeDef(TypedDict):
    ProcessedRecordsCount: NotRequired[int],
    ExportedRecordsCount: NotRequired[int],
```

## FailureInfoTypeDef

```python
# FailureInfoTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import FailureInfoTypeDef


def get_value() -> FailureInfoTypeDef:
    return {
        "FailedRecordsS3Url": ...,
    }


# FailureInfoTypeDef definition

class FailureInfoTypeDef(TypedDict):
    FailedRecordsS3Url: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## SendQuotaTypeDef

```python
# SendQuotaTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SendQuotaTypeDef


def get_value() -> SendQuotaTypeDef:
    return {
        "Max24HourSend": ...,
    }


# SendQuotaTypeDef definition

class SendQuotaTypeDef(TypedDict):
    Max24HourSend: NotRequired[float],
    MaxSendRate: NotRequired[float],
    SentLast24Hours: NotRequired[float],
```

## SuppressionAttributesTypeDef

```python
# SuppressionAttributesTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SuppressionAttributesTypeDef


def get_value() -> SuppressionAttributesTypeDef:
    return {
        "SuppressedReasons": ...,
    }


# SuppressionAttributesTypeDef definition

class SuppressionAttributesTypeDef(TypedDict):
    SuppressedReasons: NotRequired[List[SuppressionListReasonType]],  # (1)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## GetBlacklistReportsRequestTypeDef

```python
# GetBlacklistReportsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetBlacklistReportsRequestTypeDef


def get_value() -> GetBlacklistReportsRequestTypeDef:
    return {
        "BlacklistItemNames": ...,
    }


# GetBlacklistReportsRequestTypeDef definition

class GetBlacklistReportsRequestTypeDef(TypedDict):
    BlacklistItemNames: Sequence[str],
```

## GetConfigurationSetEventDestinationsRequestTypeDef

```python
# GetConfigurationSetEventDestinationsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetConfigurationSetEventDestinationsRequestTypeDef


def get_value() -> GetConfigurationSetEventDestinationsRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# GetConfigurationSetEventDestinationsRequestTypeDef definition

class GetConfigurationSetEventDestinationsRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## GetConfigurationSetRequestTypeDef

```python
# GetConfigurationSetRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetConfigurationSetRequestTypeDef


def get_value() -> GetConfigurationSetRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# GetConfigurationSetRequestTypeDef definition

class GetConfigurationSetRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## ReputationOptionsOutputTypeDef

```python
# ReputationOptionsOutputTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ReputationOptionsOutputTypeDef


def get_value() -> ReputationOptionsOutputTypeDef:
    return {
        "ReputationMetricsEnabled": ...,
    }


# ReputationOptionsOutputTypeDef definition

class ReputationOptionsOutputTypeDef(TypedDict):
    ReputationMetricsEnabled: NotRequired[bool],
    LastFreshStart: NotRequired[datetime],
```

## SuppressionOptionsOutputTypeDef

```python
# SuppressionOptionsOutputTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SuppressionOptionsOutputTypeDef


def get_value() -> SuppressionOptionsOutputTypeDef:
    return {
        "SuppressedReasons": ...,
    }


# SuppressionOptionsOutputTypeDef definition

class SuppressionOptionsOutputTypeDef(TypedDict):
    SuppressedReasons: NotRequired[List[SuppressionListReasonType]],  # (1)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## GetContactListRequestTypeDef

```python
# GetContactListRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetContactListRequestTypeDef


def get_value() -> GetContactListRequestTypeDef:
    return {
        "ContactListName": ...,
    }


# GetContactListRequestTypeDef definition

class GetContactListRequestTypeDef(TypedDict):
    ContactListName: str,
```

## GetContactRequestTypeDef

```python
# GetContactRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetContactRequestTypeDef


def get_value() -> GetContactRequestTypeDef:
    return {
        "ContactListName": ...,
    }


# GetContactRequestTypeDef definition

class GetContactRequestTypeDef(TypedDict):
    ContactListName: str,
    EmailAddress: str,
```

## GetCustomVerificationEmailTemplateRequestTypeDef

```python
# GetCustomVerificationEmailTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetCustomVerificationEmailTemplateRequestTypeDef


def get_value() -> GetCustomVerificationEmailTemplateRequestTypeDef:
    return {
        "TemplateName": ...,
    }


# GetCustomVerificationEmailTemplateRequestTypeDef definition

class GetCustomVerificationEmailTemplateRequestTypeDef(TypedDict):
    TemplateName: str,
```

## GetDedicatedIpPoolRequestTypeDef

```python
# GetDedicatedIpPoolRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetDedicatedIpPoolRequestTypeDef


def get_value() -> GetDedicatedIpPoolRequestTypeDef:
    return {
        "PoolName": ...,
    }


# GetDedicatedIpPoolRequestTypeDef definition

class GetDedicatedIpPoolRequestTypeDef(TypedDict):
    PoolName: str,
```

## GetDedicatedIpRequestTypeDef

```python
# GetDedicatedIpRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetDedicatedIpRequestTypeDef


def get_value() -> GetDedicatedIpRequestTypeDef:
    return {
        "Ip": ...,
    }


# GetDedicatedIpRequestTypeDef definition

class GetDedicatedIpRequestTypeDef(TypedDict):
    Ip: str,
```

## GetDedicatedIpsRequestTypeDef

```python
# GetDedicatedIpsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetDedicatedIpsRequestTypeDef


def get_value() -> GetDedicatedIpsRequestTypeDef:
    return {
        "PoolName": ...,
    }


# GetDedicatedIpsRequestTypeDef definition

class GetDedicatedIpsRequestTypeDef(TypedDict):
    PoolName: NotRequired[str],
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## GetDeliverabilityTestReportRequestTypeDef

```python
# GetDeliverabilityTestReportRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetDeliverabilityTestReportRequestTypeDef


def get_value() -> GetDeliverabilityTestReportRequestTypeDef:
    return {
        "ReportId": ...,
    }


# GetDeliverabilityTestReportRequestTypeDef definition

class GetDeliverabilityTestReportRequestTypeDef(TypedDict):
    ReportId: str,
```

## PlacementStatisticsTypeDef

```python
# PlacementStatisticsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PlacementStatisticsTypeDef


def get_value() -> PlacementStatisticsTypeDef:
    return {
        "InboxPercentage": ...,
    }


# PlacementStatisticsTypeDef definition

class PlacementStatisticsTypeDef(TypedDict):
    InboxPercentage: NotRequired[float],
    SpamPercentage: NotRequired[float],
    MissingPercentage: NotRequired[float],
    SpfPercentage: NotRequired[float],
    DkimPercentage: NotRequired[float],
```

## GetDomainDeliverabilityCampaignRequestTypeDef

```python
# GetDomainDeliverabilityCampaignRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetDomainDeliverabilityCampaignRequestTypeDef


def get_value() -> GetDomainDeliverabilityCampaignRequestTypeDef:
    return {
        "CampaignId": ...,
    }


# GetDomainDeliverabilityCampaignRequestTypeDef definition

class GetDomainDeliverabilityCampaignRequestTypeDef(TypedDict):
    CampaignId: str,
```

## GetEmailIdentityPoliciesRequestTypeDef

```python
# GetEmailIdentityPoliciesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetEmailIdentityPoliciesRequestTypeDef


def get_value() -> GetEmailIdentityPoliciesRequestTypeDef:
    return {
        "EmailIdentity": ...,
    }


# GetEmailIdentityPoliciesRequestTypeDef definition

class GetEmailIdentityPoliciesRequestTypeDef(TypedDict):
    EmailIdentity: str,
```

## GetEmailIdentityRequestTypeDef

```python
# GetEmailIdentityRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetEmailIdentityRequestTypeDef


def get_value() -> GetEmailIdentityRequestTypeDef:
    return {
        "EmailIdentity": ...,
    }


# GetEmailIdentityRequestTypeDef definition

class GetEmailIdentityRequestTypeDef(TypedDict):
    EmailIdentity: str,
```

## MailFromAttributesTypeDef

```python
# MailFromAttributesTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import MailFromAttributesTypeDef


def get_value() -> MailFromAttributesTypeDef:
    return {
        "MailFromDomain": ...,
    }


# MailFromAttributesTypeDef definition

class MailFromAttributesTypeDef(TypedDict):
    MailFromDomain: str,
    MailFromDomainStatus: MailFromDomainStatusType,  # (1)
    BehaviorOnMxFailure: BehaviorOnMxFailureType,  # (2)
```

1. See [:material-code-brackets: MailFromDomainStatusType](./literals.md#mailfromdomainstatustype) 
2. See [:material-code-brackets: BehaviorOnMxFailureType](./literals.md#behavioronmxfailuretype) 
## GetEmailTemplateRequestTypeDef

```python
# GetEmailTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetEmailTemplateRequestTypeDef


def get_value() -> GetEmailTemplateRequestTypeDef:
    return {
        "TemplateName": ...,
    }


# GetEmailTemplateRequestTypeDef definition

class GetEmailTemplateRequestTypeDef(TypedDict):
    TemplateName: str,
```

## GetExportJobRequestTypeDef

```python
# GetExportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetExportJobRequestTypeDef


def get_value() -> GetExportJobRequestTypeDef:
    return {
        "JobId": ...,
    }


# GetExportJobRequestTypeDef definition

class GetExportJobRequestTypeDef(TypedDict):
    JobId: str,
```

## GetImportJobRequestTypeDef

```python
# GetImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetImportJobRequestTypeDef


def get_value() -> GetImportJobRequestTypeDef:
    return {
        "JobId": ...,
    }


# GetImportJobRequestTypeDef definition

class GetImportJobRequestTypeDef(TypedDict):
    JobId: str,
```

## GetMessageInsightsRequestTypeDef

```python
# GetMessageInsightsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetMessageInsightsRequestTypeDef


def get_value() -> GetMessageInsightsRequestTypeDef:
    return {
        "MessageId": ...,
    }


# GetMessageInsightsRequestTypeDef definition

class GetMessageInsightsRequestTypeDef(TypedDict):
    MessageId: str,
```

## GetMultiRegionEndpointRequestTypeDef

```python
# GetMultiRegionEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetMultiRegionEndpointRequestTypeDef


def get_value() -> GetMultiRegionEndpointRequestTypeDef:
    return {
        "EndpointName": ...,
    }


# GetMultiRegionEndpointRequestTypeDef definition

class GetMultiRegionEndpointRequestTypeDef(TypedDict):
    EndpointName: str,
```

## RouteTypeDef

```python
# RouteTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import RouteTypeDef


def get_value() -> RouteTypeDef:
    return {
        "Region": ...,
    }


# RouteTypeDef definition

class RouteTypeDef(TypedDict):
    Region: str,
```

## GetSuppressedDestinationRequestTypeDef

```python
# GetSuppressedDestinationRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetSuppressedDestinationRequestTypeDef


def get_value() -> GetSuppressedDestinationRequestTypeDef:
    return {
        "EmailAddress": ...,
    }


# GetSuppressedDestinationRequestTypeDef definition

class GetSuppressedDestinationRequestTypeDef(TypedDict):
    EmailAddress: str,
```

## GuardianAttributesTypeDef

```python
# GuardianAttributesTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GuardianAttributesTypeDef


def get_value() -> GuardianAttributesTypeDef:
    return {
        "OptimizedSharedDelivery": ...,
    }


# GuardianAttributesTypeDef definition

class GuardianAttributesTypeDef(TypedDict):
    OptimizedSharedDelivery: NotRequired[FeatureStatusType],  # (1)
```

1. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## GuardianOptionsTypeDef

```python
# GuardianOptionsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GuardianOptionsTypeDef


def get_value() -> GuardianOptionsTypeDef:
    return {
        "OptimizedSharedDelivery": ...,
    }


# GuardianOptionsTypeDef definition

class GuardianOptionsTypeDef(TypedDict):
    OptimizedSharedDelivery: NotRequired[FeatureStatusType],  # (1)
```

1. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## IdentityInfoTypeDef

```python
# IdentityInfoTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import IdentityInfoTypeDef


def get_value() -> IdentityInfoTypeDef:
    return {
        "IdentityType": ...,
    }


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
# SuppressionListDestinationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SuppressionListDestinationTypeDef


def get_value() -> SuppressionListDestinationTypeDef:
    return {
        "SuppressionListImportAction": ...,
    }


# SuppressionListDestinationTypeDef definition

class SuppressionListDestinationTypeDef(TypedDict):
    SuppressionListImportAction: SuppressionListImportActionType,  # (1)
```

1. See [:material-code-brackets: SuppressionListImportActionType](./literals.md#suppressionlistimportactiontype) 
## InboxPlacementTrackingOptionTypeDef

```python
# InboxPlacementTrackingOptionTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import InboxPlacementTrackingOptionTypeDef


def get_value() -> InboxPlacementTrackingOptionTypeDef:
    return {
        "Global": ...,
    }


# InboxPlacementTrackingOptionTypeDef definition

class InboxPlacementTrackingOptionTypeDef(TypedDict):
    Global: NotRequired[bool],
    TrackedIsps: NotRequired[Sequence[str]],
```

## ListConfigurationSetsRequestTypeDef

```python
# ListConfigurationSetsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListConfigurationSetsRequestTypeDef


def get_value() -> ListConfigurationSetsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListConfigurationSetsRequestTypeDef definition

class ListConfigurationSetsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListContactListsRequestTypeDef

```python
# ListContactListsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListContactListsRequestTypeDef


def get_value() -> ListContactListsRequestTypeDef:
    return {
        "PageSize": ...,
    }


# ListContactListsRequestTypeDef definition

class ListContactListsRequestTypeDef(TypedDict):
    PageSize: NotRequired[int],
    NextToken: NotRequired[str],
```

## TopicFilterTypeDef

```python
# TopicFilterTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import TopicFilterTypeDef


def get_value() -> TopicFilterTypeDef:
    return {
        "TopicName": ...,
    }


# TopicFilterTypeDef definition

class TopicFilterTypeDef(TypedDict):
    TopicName: NotRequired[str],
    UseDefaultIfPreferenceUnavailable: NotRequired[bool],
```

## ListCustomVerificationEmailTemplatesRequestTypeDef

```python
# ListCustomVerificationEmailTemplatesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListCustomVerificationEmailTemplatesRequestTypeDef


def get_value() -> ListCustomVerificationEmailTemplatesRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListCustomVerificationEmailTemplatesRequestTypeDef definition

class ListCustomVerificationEmailTemplatesRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListDedicatedIpPoolsRequestTypeDef

```python
# ListDedicatedIpPoolsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListDedicatedIpPoolsRequestTypeDef


def get_value() -> ListDedicatedIpPoolsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListDedicatedIpPoolsRequestTypeDef definition

class ListDedicatedIpPoolsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListDeliverabilityTestReportsRequestTypeDef

```python
# ListDeliverabilityTestReportsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListDeliverabilityTestReportsRequestTypeDef


def get_value() -> ListDeliverabilityTestReportsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListDeliverabilityTestReportsRequestTypeDef definition

class ListDeliverabilityTestReportsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListEmailIdentitiesRequestTypeDef

```python
# ListEmailIdentitiesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListEmailIdentitiesRequestTypeDef


def get_value() -> ListEmailIdentitiesRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListEmailIdentitiesRequestTypeDef definition

class ListEmailIdentitiesRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListEmailTemplatesRequestTypeDef

```python
# ListEmailTemplatesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListEmailTemplatesRequestTypeDef


def get_value() -> ListEmailTemplatesRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListEmailTemplatesRequestTypeDef definition

class ListEmailTemplatesRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListExportJobsRequestTypeDef

```python
# ListExportJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListExportJobsRequestTypeDef


def get_value() -> ListExportJobsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListExportJobsRequestTypeDef definition

class ListExportJobsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
    ExportSourceType: NotRequired[ExportSourceTypeType],  # (1)
    JobStatus: NotRequired[JobStatusType],  # (2)
```

1. See [:material-code-brackets: ExportSourceTypeType](./literals.md#exportsourcetypetype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## ListImportJobsRequestTypeDef

```python
# ListImportJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListImportJobsRequestTypeDef


def get_value() -> ListImportJobsRequestTypeDef:
    return {
        "ImportDestinationType": ...,
    }


# ListImportJobsRequestTypeDef definition

class ListImportJobsRequestTypeDef(TypedDict):
    ImportDestinationType: NotRequired[ImportDestinationTypeType],  # (1)
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

1. See [:material-code-brackets: ImportDestinationTypeType](./literals.md#importdestinationtypetype) 
## ListManagementOptionsTypeDef

```python
# ListManagementOptionsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListManagementOptionsTypeDef


def get_value() -> ListManagementOptionsTypeDef:
    return {
        "ContactListName": ...,
    }


# ListManagementOptionsTypeDef definition

class ListManagementOptionsTypeDef(TypedDict):
    ContactListName: str,
    TopicName: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListMultiRegionEndpointsRequestTypeDef

```python
# ListMultiRegionEndpointsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListMultiRegionEndpointsRequestTypeDef


def get_value() -> ListMultiRegionEndpointsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListMultiRegionEndpointsRequestTypeDef definition

class ListMultiRegionEndpointsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## MultiRegionEndpointTypeDef

```python
# MultiRegionEndpointTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import MultiRegionEndpointTypeDef


def get_value() -> MultiRegionEndpointTypeDef:
    return {
        "EndpointName": ...,
    }


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
## ListRecommendationsRequestTypeDef

```python
# ListRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListRecommendationsRequestTypeDef


def get_value() -> ListRecommendationsRequestTypeDef:
    return {
        "Filter": ...,
    }


# ListRecommendationsRequestTypeDef definition

class ListRecommendationsRequestTypeDef(TypedDict):
    Filter: NotRequired[Mapping[ListRecommendationsFilterKeyType, str]],  # (1)
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

1. See [:material-code-brackets: ListRecommendationsFilterKeyType](./literals.md#listrecommendationsfilterkeytype) 
## RecommendationTypeDef

```python
# RecommendationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import RecommendationTypeDef


def get_value() -> RecommendationTypeDef:
    return {
        "ResourceArn": ...,
    }


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
# SuppressedDestinationSummaryTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SuppressedDestinationSummaryTypeDef


def get_value() -> SuppressedDestinationSummaryTypeDef:
    return {
        "EmailAddress": ...,
    }


# SuppressedDestinationSummaryTypeDef definition

class SuppressedDestinationSummaryTypeDef(TypedDict):
    EmailAddress: str,
    Reason: SuppressionListReasonType,  # (1)
    LastUpdateTime: datetime,
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## MessageInsightsFiltersOutputTypeDef

```python
# MessageInsightsFiltersOutputTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import MessageInsightsFiltersOutputTypeDef


def get_value() -> MessageInsightsFiltersOutputTypeDef:
    return {
        "FromEmailAddress": ...,
    }


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
# MessageInsightsFiltersTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import MessageInsightsFiltersTypeDef


def get_value() -> MessageInsightsFiltersTypeDef:
    return {
        "FromEmailAddress": ...,
    }


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
## PutAccountDedicatedIpWarmupAttributesRequestTypeDef

```python
# PutAccountDedicatedIpWarmupAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutAccountDedicatedIpWarmupAttributesRequestTypeDef


def get_value() -> PutAccountDedicatedIpWarmupAttributesRequestTypeDef:
    return {
        "AutoWarmupEnabled": ...,
    }


# PutAccountDedicatedIpWarmupAttributesRequestTypeDef definition

class PutAccountDedicatedIpWarmupAttributesRequestTypeDef(TypedDict):
    AutoWarmupEnabled: NotRequired[bool],
```

## PutAccountDetailsRequestTypeDef

```python
# PutAccountDetailsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutAccountDetailsRequestTypeDef


def get_value() -> PutAccountDetailsRequestTypeDef:
    return {
        "MailType": ...,
    }


# PutAccountDetailsRequestTypeDef definition

class PutAccountDetailsRequestTypeDef(TypedDict):
    MailType: MailTypeType,  # (1)
    WebsiteURL: str,
    ContactLanguage: NotRequired[ContactLanguageType],  # (2)
    UseCaseDescription: NotRequired[str],
    AdditionalContactEmailAddresses: NotRequired[Sequence[str]],
    ProductionAccessEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: MailTypeType](./literals.md#mailtypetype) 
2. See [:material-code-brackets: ContactLanguageType](./literals.md#contactlanguagetype) 
## PutAccountSendingAttributesRequestTypeDef

```python
# PutAccountSendingAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutAccountSendingAttributesRequestTypeDef


def get_value() -> PutAccountSendingAttributesRequestTypeDef:
    return {
        "SendingEnabled": ...,
    }


# PutAccountSendingAttributesRequestTypeDef definition

class PutAccountSendingAttributesRequestTypeDef(TypedDict):
    SendingEnabled: NotRequired[bool],
```

## PutAccountSuppressionAttributesRequestTypeDef

```python
# PutAccountSuppressionAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutAccountSuppressionAttributesRequestTypeDef


def get_value() -> PutAccountSuppressionAttributesRequestTypeDef:
    return {
        "SuppressedReasons": ...,
    }


# PutAccountSuppressionAttributesRequestTypeDef definition

class PutAccountSuppressionAttributesRequestTypeDef(TypedDict):
    SuppressedReasons: NotRequired[Sequence[SuppressionListReasonType]],  # (1)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## PutConfigurationSetArchivingOptionsRequestTypeDef

```python
# PutConfigurationSetArchivingOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutConfigurationSetArchivingOptionsRequestTypeDef


def get_value() -> PutConfigurationSetArchivingOptionsRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# PutConfigurationSetArchivingOptionsRequestTypeDef definition

class PutConfigurationSetArchivingOptionsRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    ArchiveArn: NotRequired[str],
```

## PutConfigurationSetDeliveryOptionsRequestTypeDef

```python
# PutConfigurationSetDeliveryOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutConfigurationSetDeliveryOptionsRequestTypeDef


def get_value() -> PutConfigurationSetDeliveryOptionsRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# PutConfigurationSetDeliveryOptionsRequestTypeDef definition

class PutConfigurationSetDeliveryOptionsRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    TlsPolicy: NotRequired[TlsPolicyType],  # (1)
    SendingPoolName: NotRequired[str],
    MaxDeliverySeconds: NotRequired[int],
```

1. See [:material-code-brackets: TlsPolicyType](./literals.md#tlspolicytype) 
## PutConfigurationSetReputationOptionsRequestTypeDef

```python
# PutConfigurationSetReputationOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutConfigurationSetReputationOptionsRequestTypeDef


def get_value() -> PutConfigurationSetReputationOptionsRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# PutConfigurationSetReputationOptionsRequestTypeDef definition

class PutConfigurationSetReputationOptionsRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    ReputationMetricsEnabled: NotRequired[bool],
```

## PutConfigurationSetSendingOptionsRequestTypeDef

```python
# PutConfigurationSetSendingOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutConfigurationSetSendingOptionsRequestTypeDef


def get_value() -> PutConfigurationSetSendingOptionsRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# PutConfigurationSetSendingOptionsRequestTypeDef definition

class PutConfigurationSetSendingOptionsRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    SendingEnabled: NotRequired[bool],
```

## PutConfigurationSetSuppressionOptionsRequestTypeDef

```python
# PutConfigurationSetSuppressionOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutConfigurationSetSuppressionOptionsRequestTypeDef


def get_value() -> PutConfigurationSetSuppressionOptionsRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# PutConfigurationSetSuppressionOptionsRequestTypeDef definition

class PutConfigurationSetSuppressionOptionsRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    SuppressedReasons: NotRequired[Sequence[SuppressionListReasonType]],  # (1)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## PutConfigurationSetTrackingOptionsRequestTypeDef

```python
# PutConfigurationSetTrackingOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutConfigurationSetTrackingOptionsRequestTypeDef


def get_value() -> PutConfigurationSetTrackingOptionsRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# PutConfigurationSetTrackingOptionsRequestTypeDef definition

class PutConfigurationSetTrackingOptionsRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    CustomRedirectDomain: NotRequired[str],
    HttpsPolicy: NotRequired[HttpsPolicyType],  # (1)
```

1. See [:material-code-brackets: HttpsPolicyType](./literals.md#httpspolicytype) 
## PutDedicatedIpInPoolRequestTypeDef

```python
# PutDedicatedIpInPoolRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutDedicatedIpInPoolRequestTypeDef


def get_value() -> PutDedicatedIpInPoolRequestTypeDef:
    return {
        "Ip": ...,
    }


# PutDedicatedIpInPoolRequestTypeDef definition

class PutDedicatedIpInPoolRequestTypeDef(TypedDict):
    Ip: str,
    DestinationPoolName: str,
```

## PutDedicatedIpPoolScalingAttributesRequestTypeDef

```python
# PutDedicatedIpPoolScalingAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutDedicatedIpPoolScalingAttributesRequestTypeDef


def get_value() -> PutDedicatedIpPoolScalingAttributesRequestTypeDef:
    return {
        "PoolName": ...,
    }


# PutDedicatedIpPoolScalingAttributesRequestTypeDef definition

class PutDedicatedIpPoolScalingAttributesRequestTypeDef(TypedDict):
    PoolName: str,
    ScalingMode: ScalingModeType,  # (1)
```

1. See [:material-code-brackets: ScalingModeType](./literals.md#scalingmodetype) 
## PutDedicatedIpWarmupAttributesRequestTypeDef

```python
# PutDedicatedIpWarmupAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutDedicatedIpWarmupAttributesRequestTypeDef


def get_value() -> PutDedicatedIpWarmupAttributesRequestTypeDef:
    return {
        "Ip": ...,
    }


# PutDedicatedIpWarmupAttributesRequestTypeDef definition

class PutDedicatedIpWarmupAttributesRequestTypeDef(TypedDict):
    Ip: str,
    WarmupPercentage: int,
```

## PutEmailIdentityConfigurationSetAttributesRequestTypeDef

```python
# PutEmailIdentityConfigurationSetAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutEmailIdentityConfigurationSetAttributesRequestTypeDef


def get_value() -> PutEmailIdentityConfigurationSetAttributesRequestTypeDef:
    return {
        "EmailIdentity": ...,
    }


# PutEmailIdentityConfigurationSetAttributesRequestTypeDef definition

class PutEmailIdentityConfigurationSetAttributesRequestTypeDef(TypedDict):
    EmailIdentity: str,
    ConfigurationSetName: NotRequired[str],
```

## PutEmailIdentityDkimAttributesRequestTypeDef

```python
# PutEmailIdentityDkimAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutEmailIdentityDkimAttributesRequestTypeDef


def get_value() -> PutEmailIdentityDkimAttributesRequestTypeDef:
    return {
        "EmailIdentity": ...,
    }


# PutEmailIdentityDkimAttributesRequestTypeDef definition

class PutEmailIdentityDkimAttributesRequestTypeDef(TypedDict):
    EmailIdentity: str,
    SigningEnabled: NotRequired[bool],
```

## PutEmailIdentityFeedbackAttributesRequestTypeDef

```python
# PutEmailIdentityFeedbackAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutEmailIdentityFeedbackAttributesRequestTypeDef


def get_value() -> PutEmailIdentityFeedbackAttributesRequestTypeDef:
    return {
        "EmailIdentity": ...,
    }


# PutEmailIdentityFeedbackAttributesRequestTypeDef definition

class PutEmailIdentityFeedbackAttributesRequestTypeDef(TypedDict):
    EmailIdentity: str,
    EmailForwardingEnabled: NotRequired[bool],
```

## PutEmailIdentityMailFromAttributesRequestTypeDef

```python
# PutEmailIdentityMailFromAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutEmailIdentityMailFromAttributesRequestTypeDef


def get_value() -> PutEmailIdentityMailFromAttributesRequestTypeDef:
    return {
        "EmailIdentity": ...,
    }


# PutEmailIdentityMailFromAttributesRequestTypeDef definition

class PutEmailIdentityMailFromAttributesRequestTypeDef(TypedDict):
    EmailIdentity: str,
    MailFromDomain: NotRequired[str],
    BehaviorOnMxFailure: NotRequired[BehaviorOnMxFailureType],  # (1)
```

1. See [:material-code-brackets: BehaviorOnMxFailureType](./literals.md#behavioronmxfailuretype) 
## PutSuppressedDestinationRequestTypeDef

```python
# PutSuppressedDestinationRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutSuppressedDestinationRequestTypeDef


def get_value() -> PutSuppressedDestinationRequestTypeDef:
    return {
        "EmailAddress": ...,
    }


# PutSuppressedDestinationRequestTypeDef definition

class PutSuppressedDestinationRequestTypeDef(TypedDict):
    EmailAddress: str,
    Reason: SuppressionListReasonType,  # (1)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## ReplacementTemplateTypeDef

```python
# ReplacementTemplateTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ReplacementTemplateTypeDef


def get_value() -> ReplacementTemplateTypeDef:
    return {
        "ReplacementTemplateData": ...,
    }


# ReplacementTemplateTypeDef definition

class ReplacementTemplateTypeDef(TypedDict):
    ReplacementTemplateData: NotRequired[str],
```

## SOARecordTypeDef

```python
# SOARecordTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SOARecordTypeDef


def get_value() -> SOARecordTypeDef:
    return {
        "PrimaryNameServer": ...,
    }


# SOARecordTypeDef definition

class SOARecordTypeDef(TypedDict):
    PrimaryNameServer: NotRequired[str],
    AdminEmail: NotRequired[str],
    SerialNumber: NotRequired[int],
```

## SendCustomVerificationEmailRequestTypeDef

```python
# SendCustomVerificationEmailRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SendCustomVerificationEmailRequestTypeDef


def get_value() -> SendCustomVerificationEmailRequestTypeDef:
    return {
        "EmailAddress": ...,
    }


# SendCustomVerificationEmailRequestTypeDef definition

class SendCustomVerificationEmailRequestTypeDef(TypedDict):
    EmailAddress: str,
    TemplateName: str,
    ConfigurationSetName: NotRequired[str],
```

## SuppressedDestinationAttributesTypeDef

```python
# SuppressedDestinationAttributesTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SuppressedDestinationAttributesTypeDef


def get_value() -> SuppressedDestinationAttributesTypeDef:
    return {
        "MessageId": ...,
    }


# SuppressedDestinationAttributesTypeDef definition

class SuppressedDestinationAttributesTypeDef(TypedDict):
    MessageId: NotRequired[str],
    FeedbackId: NotRequired[str],
```

## SuppressionOptionsTypeDef

```python
# SuppressionOptionsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SuppressionOptionsTypeDef


def get_value() -> SuppressionOptionsTypeDef:
    return {
        "SuppressedReasons": ...,
    }


# SuppressionOptionsTypeDef definition

class SuppressionOptionsTypeDef(TypedDict):
    SuppressedReasons: NotRequired[Sequence[SuppressionListReasonType]],  # (1)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## TestRenderEmailTemplateRequestTypeDef

```python
# TestRenderEmailTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import TestRenderEmailTemplateRequestTypeDef


def get_value() -> TestRenderEmailTemplateRequestTypeDef:
    return {
        "TemplateName": ...,
    }


# TestRenderEmailTemplateRequestTypeDef definition

class TestRenderEmailTemplateRequestTypeDef(TypedDict):
    TemplateName: str,
    TemplateData: str,
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateCustomVerificationEmailTemplateRequestTypeDef

```python
# UpdateCustomVerificationEmailTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import UpdateCustomVerificationEmailTemplateRequestTypeDef


def get_value() -> UpdateCustomVerificationEmailTemplateRequestTypeDef:
    return {
        "TemplateName": ...,
    }


# UpdateCustomVerificationEmailTemplateRequestTypeDef definition

class UpdateCustomVerificationEmailTemplateRequestTypeDef(TypedDict):
    TemplateName: str,
    FromEmailAddress: str,
    TemplateSubject: str,
    TemplateContent: str,
    SuccessRedirectionURL: str,
    FailureRedirectionURL: str,
```

## UpdateEmailIdentityPolicyRequestTypeDef

```python
# UpdateEmailIdentityPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import UpdateEmailIdentityPolicyRequestTypeDef


def get_value() -> UpdateEmailIdentityPolicyRequestTypeDef:
    return {
        "EmailIdentity": ...,
    }


# UpdateEmailIdentityPolicyRequestTypeDef definition

class UpdateEmailIdentityPolicyRequestTypeDef(TypedDict):
    EmailIdentity: str,
    PolicyName: str,
    Policy: str,
```

## AccountDetailsTypeDef

```python
# AccountDetailsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import AccountDetailsTypeDef


def get_value() -> AccountDetailsTypeDef:
    return {
        "MailType": ...,
    }


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
# BatchGetMetricDataQueryTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import BatchGetMetricDataQueryTypeDef


def get_value() -> BatchGetMetricDataQueryTypeDef:
    return {
        "Id": ...,
    }


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
## GetDomainStatisticsReportRequestTypeDef

```python
# GetDomainStatisticsReportRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetDomainStatisticsReportRequestTypeDef


def get_value() -> GetDomainStatisticsReportRequestTypeDef:
    return {
        "Domain": ...,
    }


# GetDomainStatisticsReportRequestTypeDef definition

class GetDomainStatisticsReportRequestTypeDef(TypedDict):
    Domain: str,
    StartDate: TimestampTypeDef,
    EndDate: TimestampTypeDef,
```

## ListDomainDeliverabilityCampaignsRequestTypeDef

```python
# ListDomainDeliverabilityCampaignsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListDomainDeliverabilityCampaignsRequestTypeDef


def get_value() -> ListDomainDeliverabilityCampaignsRequestTypeDef:
    return {
        "StartDate": ...,
    }


# ListDomainDeliverabilityCampaignsRequestTypeDef definition

class ListDomainDeliverabilityCampaignsRequestTypeDef(TypedDict):
    StartDate: TimestampTypeDef,
    EndDate: TimestampTypeDef,
    SubscribedDomain: str,
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListSuppressedDestinationsRequestTypeDef

```python
# ListSuppressedDestinationsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListSuppressedDestinationsRequestTypeDef


def get_value() -> ListSuppressedDestinationsRequestTypeDef:
    return {
        "Reasons": ...,
    }


# ListSuppressedDestinationsRequestTypeDef definition

class ListSuppressedDestinationsRequestTypeDef(TypedDict):
    Reasons: NotRequired[Sequence[SuppressionListReasonType]],  # (1)
    StartDate: NotRequired[TimestampTypeDef],
    EndDate: NotRequired[TimestampTypeDef],
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
## ReputationOptionsTypeDef

```python
# ReputationOptionsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ReputationOptionsTypeDef


def get_value() -> ReputationOptionsTypeDef:
    return {
        "ReputationMetricsEnabled": ...,
    }


# ReputationOptionsTypeDef definition

class ReputationOptionsTypeDef(TypedDict):
    ReputationMetricsEnabled: NotRequired[bool],
    LastFreshStart: NotRequired[TimestampTypeDef],
```

## BatchGetMetricDataResponseTypeDef

```python
# BatchGetMetricDataResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import BatchGetMetricDataResponseTypeDef


def get_value() -> BatchGetMetricDataResponseTypeDef:
    return {
        "Results": ...,
    }


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
# CreateDeliverabilityTestReportResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateDeliverabilityTestReportResponseTypeDef


def get_value() -> CreateDeliverabilityTestReportResponseTypeDef:
    return {
        "ReportId": ...,
    }


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
# CreateExportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateExportJobResponseTypeDef


def get_value() -> CreateExportJobResponseTypeDef:
    return {
        "JobId": ...,
    }


# CreateExportJobResponseTypeDef definition

class CreateExportJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateImportJobResponseTypeDef

```python
# CreateImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateImportJobResponseTypeDef


def get_value() -> CreateImportJobResponseTypeDef:
    return {
        "JobId": ...,
    }


# CreateImportJobResponseTypeDef definition

class CreateImportJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMultiRegionEndpointResponseTypeDef

```python
# CreateMultiRegionEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateMultiRegionEndpointResponseTypeDef


def get_value() -> CreateMultiRegionEndpointResponseTypeDef:
    return {
        "Status": ...,
    }


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
# DeleteMultiRegionEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DeleteMultiRegionEndpointResponseTypeDef


def get_value() -> DeleteMultiRegionEndpointResponseTypeDef:
    return {
        "Status": ...,
    }


# DeleteMultiRegionEndpointResponseTypeDef definition

class DeleteMultiRegionEndpointResponseTypeDef(TypedDict):
    Status: StatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCustomVerificationEmailTemplateResponseTypeDef

```python
# GetCustomVerificationEmailTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetCustomVerificationEmailTemplateResponseTypeDef


def get_value() -> GetCustomVerificationEmailTemplateResponseTypeDef:
    return {
        "TemplateName": ...,
    }


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
# GetEmailIdentityPoliciesResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetEmailIdentityPoliciesResponseTypeDef


def get_value() -> GetEmailIdentityPoliciesResponseTypeDef:
    return {
        "Policies": ...,
    }


# GetEmailIdentityPoliciesResponseTypeDef definition

class GetEmailIdentityPoliciesResponseTypeDef(TypedDict):
    Policies: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationSetsResponseTypeDef

```python
# ListConfigurationSetsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListConfigurationSetsResponseTypeDef


def get_value() -> ListConfigurationSetsResponseTypeDef:
    return {
        "ConfigurationSets": ...,
    }


# ListConfigurationSetsResponseTypeDef definition

class ListConfigurationSetsResponseTypeDef(TypedDict):
    ConfigurationSets: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDedicatedIpPoolsResponseTypeDef

```python
# ListDedicatedIpPoolsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListDedicatedIpPoolsResponseTypeDef


def get_value() -> ListDedicatedIpPoolsResponseTypeDef:
    return {
        "DedicatedIpPools": ...,
    }


# ListDedicatedIpPoolsResponseTypeDef definition

class ListDedicatedIpPoolsResponseTypeDef(TypedDict):
    DedicatedIpPools: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutEmailIdentityDkimSigningAttributesResponseTypeDef

```python
# PutEmailIdentityDkimSigningAttributesResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutEmailIdentityDkimSigningAttributesResponseTypeDef


def get_value() -> PutEmailIdentityDkimSigningAttributesResponseTypeDef:
    return {
        "DkimStatus": ...,
    }


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
# SendCustomVerificationEmailResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SendCustomVerificationEmailResponseTypeDef


def get_value() -> SendCustomVerificationEmailResponseTypeDef:
    return {
        "MessageId": ...,
    }


# SendCustomVerificationEmailResponseTypeDef definition

class SendCustomVerificationEmailResponseTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendEmailResponseTypeDef

```python
# SendEmailResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SendEmailResponseTypeDef


def get_value() -> SendEmailResponseTypeDef:
    return {
        "MessageId": ...,
    }


# SendEmailResponseTypeDef definition

class SendEmailResponseTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestRenderEmailTemplateResponseTypeDef

```python
# TestRenderEmailTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import TestRenderEmailTemplateResponseTypeDef


def get_value() -> TestRenderEmailTemplateResponseTypeDef:
    return {
        "RenderedTemplate": ...,
    }


# TestRenderEmailTemplateResponseTypeDef definition

class TestRenderEmailTemplateResponseTypeDef(TypedDict):
    RenderedTemplate: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBlacklistReportsResponseTypeDef

```python
# GetBlacklistReportsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetBlacklistReportsResponseTypeDef


def get_value() -> GetBlacklistReportsResponseTypeDef:
    return {
        "BlacklistReport": ...,
    }


# GetBlacklistReportsResponseTypeDef definition

class GetBlacklistReportsResponseTypeDef(TypedDict):
    BlacklistReport: Dict[str, List[BlacklistEntryTypeDef]],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlacklistEntryTypeDef](./type_defs.md#blacklistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RawMessageTypeDef

```python
# RawMessageTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import RawMessageTypeDef


def get_value() -> RawMessageTypeDef:
    return {
        "Data": ...,
    }


# RawMessageTypeDef definition

class RawMessageTypeDef(TypedDict):
    Data: BlobTypeDef,
```

## BodyTypeDef

```python
# BodyTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import BodyTypeDef


def get_value() -> BodyTypeDef:
    return {
        "Text": ...,
    }


# BodyTypeDef definition

class BodyTypeDef(TypedDict):
    Text: NotRequired[ContentTypeDef],  # (1)
    Html: NotRequired[ContentTypeDef],  # (1)
```

1. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
2. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
## SendBulkEmailResponseTypeDef

```python
# SendBulkEmailResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SendBulkEmailResponseTypeDef


def get_value() -> SendBulkEmailResponseTypeDef:
    return {
        "BulkEmailEntryResults": ...,
    }


# SendBulkEmailResponseTypeDef definition

class SendBulkEmailResponseTypeDef(TypedDict):
    BulkEmailEntryResults: List[BulkEmailEntryResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BulkEmailEntryResultTypeDef](./type_defs.md#bulkemailentryresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CloudWatchDestinationOutputTypeDef

```python
# CloudWatchDestinationOutputTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CloudWatchDestinationOutputTypeDef


def get_value() -> CloudWatchDestinationOutputTypeDef:
    return {
        "DimensionConfigurations": ...,
    }


# CloudWatchDestinationOutputTypeDef definition

class CloudWatchDestinationOutputTypeDef(TypedDict):
    DimensionConfigurations: List[CloudWatchDimensionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CloudWatchDimensionConfigurationTypeDef](./type_defs.md#cloudwatchdimensionconfigurationtypedef) 
## CloudWatchDestinationTypeDef

```python
# CloudWatchDestinationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CloudWatchDestinationTypeDef


def get_value() -> CloudWatchDestinationTypeDef:
    return {
        "DimensionConfigurations": ...,
    }


# CloudWatchDestinationTypeDef definition

class CloudWatchDestinationTypeDef(TypedDict):
    DimensionConfigurations: Sequence[CloudWatchDimensionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CloudWatchDimensionConfigurationTypeDef](./type_defs.md#cloudwatchdimensionconfigurationtypedef) 
## EventDetailsTypeDef

```python
# EventDetailsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import EventDetailsTypeDef


def get_value() -> EventDetailsTypeDef:
    return {
        "Bounce": ...,
    }


# EventDetailsTypeDef definition

class EventDetailsTypeDef(TypedDict):
    Bounce: NotRequired[BounceTypeDef],  # (1)
    Complaint: NotRequired[ComplaintTypeDef],  # (2)
```

1. See [:material-code-braces: BounceTypeDef](./type_defs.md#bouncetypedef) 
2. See [:material-code-braces: ComplaintTypeDef](./type_defs.md#complainttypedef) 
## ListContactListsResponseTypeDef

```python
# ListContactListsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListContactListsResponseTypeDef


def get_value() -> ListContactListsResponseTypeDef:
    return {
        "ContactLists": ...,
    }


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
# ContactTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ContactTypeDef


def get_value() -> ContactTypeDef:
    return {
        "EmailAddress": ...,
    }


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
## CreateContactRequestTypeDef

```python
# CreateContactRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateContactRequestTypeDef


def get_value() -> CreateContactRequestTypeDef:
    return {
        "ContactListName": ...,
    }


# CreateContactRequestTypeDef definition

class CreateContactRequestTypeDef(TypedDict):
    ContactListName: str,
    EmailAddress: str,
    TopicPreferences: NotRequired[Sequence[TopicPreferenceTypeDef]],  # (1)
    UnsubscribeAll: NotRequired[bool],
    AttributesData: NotRequired[str],
```

1. See [:material-code-braces: TopicPreferenceTypeDef](./type_defs.md#topicpreferencetypedef) 
## GetContactResponseTypeDef

```python
# GetContactResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetContactResponseTypeDef


def get_value() -> GetContactResponseTypeDef:
    return {
        "ContactListName": ...,
    }


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
## UpdateContactRequestTypeDef

```python
# UpdateContactRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import UpdateContactRequestTypeDef


def get_value() -> UpdateContactRequestTypeDef:
    return {
        "ContactListName": ...,
    }


# UpdateContactRequestTypeDef definition

class UpdateContactRequestTypeDef(TypedDict):
    ContactListName: str,
    EmailAddress: str,
    TopicPreferences: NotRequired[Sequence[TopicPreferenceTypeDef]],  # (1)
    UnsubscribeAll: NotRequired[bool],
    AttributesData: NotRequired[str],
```

1. See [:material-code-braces: TopicPreferenceTypeDef](./type_defs.md#topicpreferencetypedef) 
## CreateDedicatedIpPoolRequestTypeDef

```python
# CreateDedicatedIpPoolRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateDedicatedIpPoolRequestTypeDef


def get_value() -> CreateDedicatedIpPoolRequestTypeDef:
    return {
        "PoolName": ...,
    }


# CreateDedicatedIpPoolRequestTypeDef definition

class CreateDedicatedIpPoolRequestTypeDef(TypedDict):
    PoolName: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    ScalingMode: NotRequired[ScalingModeType],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: ScalingModeType](./literals.md#scalingmodetype) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateContactListRequestTypeDef

```python
# CreateContactListRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateContactListRequestTypeDef


def get_value() -> CreateContactListRequestTypeDef:
    return {
        "ContactListName": ...,
    }


# CreateContactListRequestTypeDef definition

class CreateContactListRequestTypeDef(TypedDict):
    ContactListName: str,
    Topics: NotRequired[Sequence[TopicTypeDef]],  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: TopicTypeDef](./type_defs.md#topictypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetContactListResponseTypeDef

```python
# GetContactListResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetContactListResponseTypeDef


def get_value() -> GetContactListResponseTypeDef:
    return {
        "ContactListName": ...,
    }


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
## UpdateContactListRequestTypeDef

```python
# UpdateContactListRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import UpdateContactListRequestTypeDef


def get_value() -> UpdateContactListRequestTypeDef:
    return {
        "ContactListName": ...,
    }


# UpdateContactListRequestTypeDef definition

class UpdateContactListRequestTypeDef(TypedDict):
    ContactListName: str,
    Topics: NotRequired[Sequence[TopicTypeDef]],  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-braces: TopicTypeDef](./type_defs.md#topictypedef) 
## CreateEmailIdentityRequestTypeDef

```python
# CreateEmailIdentityRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateEmailIdentityRequestTypeDef


def get_value() -> CreateEmailIdentityRequestTypeDef:
    return {
        "EmailIdentity": ...,
    }


# CreateEmailIdentityRequestTypeDef definition

class CreateEmailIdentityRequestTypeDef(TypedDict):
    EmailIdentity: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    DkimSigningAttributes: NotRequired[DkimSigningAttributesTypeDef],  # (2)
    ConfigurationSetName: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: DkimSigningAttributesTypeDef](./type_defs.md#dkimsigningattributestypedef) 
## PutEmailIdentityDkimSigningAttributesRequestTypeDef

```python
# PutEmailIdentityDkimSigningAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutEmailIdentityDkimSigningAttributesRequestTypeDef


def get_value() -> PutEmailIdentityDkimSigningAttributesRequestTypeDef:
    return {
        "EmailIdentity": ...,
    }


# PutEmailIdentityDkimSigningAttributesRequestTypeDef definition

class PutEmailIdentityDkimSigningAttributesRequestTypeDef(TypedDict):
    EmailIdentity: str,
    SigningAttributesOrigin: DkimSigningAttributesOriginType,  # (1)
    SigningAttributes: NotRequired[DkimSigningAttributesTypeDef],  # (2)
```

1. See [:material-code-brackets: DkimSigningAttributesOriginType](./literals.md#dkimsigningattributesorigintype) 
2. See [:material-code-braces: DkimSigningAttributesTypeDef](./type_defs.md#dkimsigningattributestypedef) 
## CreateEmailIdentityResponseTypeDef

```python
# CreateEmailIdentityResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateEmailIdentityResponseTypeDef


def get_value() -> CreateEmailIdentityResponseTypeDef:
    return {
        "IdentityType": ...,
    }


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
## CreateEmailTemplateRequestTypeDef

```python
# CreateEmailTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateEmailTemplateRequestTypeDef


def get_value() -> CreateEmailTemplateRequestTypeDef:
    return {
        "TemplateName": ...,
    }


# CreateEmailTemplateRequestTypeDef definition

class CreateEmailTemplateRequestTypeDef(TypedDict):
    TemplateName: str,
    TemplateContent: EmailTemplateContentTypeDef,  # (1)
```

1. See [:material-code-braces: EmailTemplateContentTypeDef](./type_defs.md#emailtemplatecontenttypedef) 
## GetEmailTemplateResponseTypeDef

```python
# GetEmailTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetEmailTemplateResponseTypeDef


def get_value() -> GetEmailTemplateResponseTypeDef:
    return {
        "TemplateName": ...,
    }


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
# TemplateTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import TemplateTypeDef


def get_value() -> TemplateTypeDef:
    return {
        "TemplateName": ...,
    }


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
## UpdateEmailTemplateRequestTypeDef

```python
# UpdateEmailTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import UpdateEmailTemplateRequestTypeDef


def get_value() -> UpdateEmailTemplateRequestTypeDef:
    return {
        "TemplateName": ...,
    }


# UpdateEmailTemplateRequestTypeDef definition

class UpdateEmailTemplateRequestTypeDef(TypedDict):
    TemplateName: str,
    TemplateContent: EmailTemplateContentTypeDef,  # (1)
```

1. See [:material-code-braces: EmailTemplateContentTypeDef](./type_defs.md#emailtemplatecontenttypedef) 
## ListCustomVerificationEmailTemplatesResponseTypeDef

```python
# ListCustomVerificationEmailTemplatesResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListCustomVerificationEmailTemplatesResponseTypeDef


def get_value() -> ListCustomVerificationEmailTemplatesResponseTypeDef:
    return {
        "CustomVerificationEmailTemplates": ...,
    }


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
# DailyVolumeTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DailyVolumeTypeDef


def get_value() -> DailyVolumeTypeDef:
    return {
        "StartDate": ...,
    }


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
# OverallVolumeTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import OverallVolumeTypeDef


def get_value() -> OverallVolumeTypeDef:
    return {
        "VolumeStatistics": ...,
    }


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
# GetDedicatedIpPoolResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetDedicatedIpPoolResponseTypeDef


def get_value() -> GetDedicatedIpPoolResponseTypeDef:
    return {
        "DedicatedIpPool": ...,
    }


# GetDedicatedIpPoolResponseTypeDef definition

class GetDedicatedIpPoolResponseTypeDef(TypedDict):
    DedicatedIpPool: DedicatedIpPoolTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DedicatedIpPoolTypeDef](./type_defs.md#dedicatedippooltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDedicatedIpResponseTypeDef

```python
# GetDedicatedIpResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetDedicatedIpResponseTypeDef


def get_value() -> GetDedicatedIpResponseTypeDef:
    return {
        "DedicatedIp": ...,
    }


# GetDedicatedIpResponseTypeDef definition

class GetDedicatedIpResponseTypeDef(TypedDict):
    DedicatedIp: DedicatedIpTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DedicatedIpTypeDef](./type_defs.md#dedicatediptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDedicatedIpsResponseTypeDef

```python
# GetDedicatedIpsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetDedicatedIpsResponseTypeDef


def get_value() -> GetDedicatedIpsResponseTypeDef:
    return {
        "DedicatedIps": ...,
    }


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
# ListDeliverabilityTestReportsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListDeliverabilityTestReportsResponseTypeDef


def get_value() -> ListDeliverabilityTestReportsResponseTypeDef:
    return {
        "DeliverabilityTestReports": ...,
    }


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
# DetailsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DetailsTypeDef


def get_value() -> DetailsTypeDef:
    return {
        "RoutesDetails": ...,
    }


# DetailsTypeDef definition

class DetailsTypeDef(TypedDict):
    RoutesDetails: Sequence[RouteDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: RouteDetailsTypeDef](./type_defs.md#routedetailstypedef) 
## GetDomainDeliverabilityCampaignResponseTypeDef

```python
# GetDomainDeliverabilityCampaignResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetDomainDeliverabilityCampaignResponseTypeDef


def get_value() -> GetDomainDeliverabilityCampaignResponseTypeDef:
    return {
        "DomainDeliverabilityCampaign": ...,
    }


# GetDomainDeliverabilityCampaignResponseTypeDef definition

class GetDomainDeliverabilityCampaignResponseTypeDef(TypedDict):
    DomainDeliverabilityCampaign: DomainDeliverabilityCampaignTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainDeliverabilityCampaignTypeDef](./type_defs.md#domaindeliverabilitycampaigntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDomainDeliverabilityCampaignsResponseTypeDef

```python
# ListDomainDeliverabilityCampaignsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListDomainDeliverabilityCampaignsResponseTypeDef


def get_value() -> ListDomainDeliverabilityCampaignsResponseTypeDef:
    return {
        "DomainDeliverabilityCampaigns": ...,
    }


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
# DomainDeliverabilityTrackingOptionOutputTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DomainDeliverabilityTrackingOptionOutputTypeDef


def get_value() -> DomainDeliverabilityTrackingOptionOutputTypeDef:
    return {
        "Domain": ...,
    }


# DomainDeliverabilityTrackingOptionOutputTypeDef definition

class DomainDeliverabilityTrackingOptionOutputTypeDef(TypedDict):
    Domain: NotRequired[str],
    SubscriptionStartDate: NotRequired[datetime],
    InboxPlacementTrackingOption: NotRequired[InboxPlacementTrackingOptionOutputTypeDef],  # (1)
```

1. See [:material-code-braces: InboxPlacementTrackingOptionOutputTypeDef](./type_defs.md#inboxplacementtrackingoptionoutputtypedef) 
## ListEmailTemplatesResponseTypeDef

```python
# ListEmailTemplatesResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListEmailTemplatesResponseTypeDef


def get_value() -> ListEmailTemplatesResponseTypeDef:
    return {
        "TemplatesMetadata": ...,
    }


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
# ListExportJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListExportJobsResponseTypeDef


def get_value() -> ListExportJobsResponseTypeDef:
    return {
        "ExportJobs": ...,
    }


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
# MetricsDataSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import MetricsDataSourceOutputTypeDef


def get_value() -> MetricsDataSourceOutputTypeDef:
    return {
        "Dimensions": ...,
    }


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
# MetricsDataSourceTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import MetricsDataSourceTypeDef


def get_value() -> MetricsDataSourceTypeDef:
    return {
        "Dimensions": ...,
    }


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
# IspPlacementTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import IspPlacementTypeDef


def get_value() -> IspPlacementTypeDef:
    return {
        "IspName": ...,
    }


# IspPlacementTypeDef definition

class IspPlacementTypeDef(TypedDict):
    IspName: NotRequired[str],
    PlacementStatistics: NotRequired[PlacementStatisticsTypeDef],  # (1)
```

1. See [:material-code-braces: PlacementStatisticsTypeDef](./type_defs.md#placementstatisticstypedef) 
## GetMultiRegionEndpointResponseTypeDef

```python
# GetMultiRegionEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetMultiRegionEndpointResponseTypeDef


def get_value() -> GetMultiRegionEndpointResponseTypeDef:
    return {
        "EndpointName": ...,
    }


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
# VdmAttributesTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import VdmAttributesTypeDef


def get_value() -> VdmAttributesTypeDef:
    return {
        "VdmEnabled": ...,
    }


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
# VdmOptionsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import VdmOptionsTypeDef


def get_value() -> VdmOptionsTypeDef:
    return {
        "DashboardOptions": ...,
    }


# VdmOptionsTypeDef definition

class VdmOptionsTypeDef(TypedDict):
    DashboardOptions: NotRequired[DashboardOptionsTypeDef],  # (1)
    GuardianOptions: NotRequired[GuardianOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: DashboardOptionsTypeDef](./type_defs.md#dashboardoptionstypedef) 
2. See [:material-code-braces: GuardianOptionsTypeDef](./type_defs.md#guardianoptionstypedef) 
## ListEmailIdentitiesResponseTypeDef

```python
# ListEmailIdentitiesResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListEmailIdentitiesResponseTypeDef


def get_value() -> ListEmailIdentitiesResponseTypeDef:
    return {
        "EmailIdentities": ...,
    }


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
# ImportDestinationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ImportDestinationTypeDef


def get_value() -> ImportDestinationTypeDef:
    return {
        "SuppressionListDestination": ...,
    }


# ImportDestinationTypeDef definition

class ImportDestinationTypeDef(TypedDict):
    SuppressionListDestination: NotRequired[SuppressionListDestinationTypeDef],  # (1)
    ContactListDestination: NotRequired[ContactListDestinationTypeDef],  # (2)
```

1. See [:material-code-braces: SuppressionListDestinationTypeDef](./type_defs.md#suppressionlistdestinationtypedef) 
2. See [:material-code-braces: ContactListDestinationTypeDef](./type_defs.md#contactlistdestinationtypedef) 
## ListContactsFilterTypeDef

```python
# ListContactsFilterTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListContactsFilterTypeDef


def get_value() -> ListContactsFilterTypeDef:
    return {
        "FilteredStatus": ...,
    }


# ListContactsFilterTypeDef definition

class ListContactsFilterTypeDef(TypedDict):
    FilteredStatus: NotRequired[SubscriptionStatusType],  # (1)
    TopicFilter: NotRequired[TopicFilterTypeDef],  # (2)
```

1. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
2. See [:material-code-braces: TopicFilterTypeDef](./type_defs.md#topicfiltertypedef) 
## ListMultiRegionEndpointsRequestPaginateTypeDef

```python
# ListMultiRegionEndpointsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListMultiRegionEndpointsRequestPaginateTypeDef


def get_value() -> ListMultiRegionEndpointsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListMultiRegionEndpointsRequestPaginateTypeDef definition

class ListMultiRegionEndpointsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMultiRegionEndpointsResponseTypeDef

```python
# ListMultiRegionEndpointsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListMultiRegionEndpointsResponseTypeDef


def get_value() -> ListMultiRegionEndpointsResponseTypeDef:
    return {
        "MultiRegionEndpoints": ...,
    }


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
# ListRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListRecommendationsResponseTypeDef


def get_value() -> ListRecommendationsResponseTypeDef:
    return {
        "Recommendations": ...,
    }


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
# ListSuppressedDestinationsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListSuppressedDestinationsResponseTypeDef


def get_value() -> ListSuppressedDestinationsResponseTypeDef:
    return {
        "SuppressedDestinationSummaries": ...,
    }


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
# MessageInsightsDataSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import MessageInsightsDataSourceOutputTypeDef


def get_value() -> MessageInsightsDataSourceOutputTypeDef:
    return {
        "StartDate": ...,
    }


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
## MessageInsightsDataSourceTypeDef

```python
# MessageInsightsDataSourceTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import MessageInsightsDataSourceTypeDef


def get_value() -> MessageInsightsDataSourceTypeDef:
    return {
        "StartDate": ...,
    }


# MessageInsightsDataSourceTypeDef definition

class MessageInsightsDataSourceTypeDef(TypedDict):
    StartDate: TimestampTypeDef,
    EndDate: TimestampTypeDef,
    Include: NotRequired[MessageInsightsFiltersTypeDef],  # (1)
    Exclude: NotRequired[MessageInsightsFiltersTypeDef],  # (1)
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: MessageInsightsFiltersTypeDef](./type_defs.md#messageinsightsfilterstypedef) 
2. See [:material-code-braces: MessageInsightsFiltersTypeDef](./type_defs.md#messageinsightsfilterstypedef) 
## ReplacementEmailContentTypeDef

```python
# ReplacementEmailContentTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ReplacementEmailContentTypeDef


def get_value() -> ReplacementEmailContentTypeDef:
    return {
        "ReplacementTemplate": ...,
    }


# ReplacementEmailContentTypeDef definition

class ReplacementEmailContentTypeDef(TypedDict):
    ReplacementTemplate: NotRequired[ReplacementTemplateTypeDef],  # (1)
```

1. See [:material-code-braces: ReplacementTemplateTypeDef](./type_defs.md#replacementtemplatetypedef) 
## VerificationInfoTypeDef

```python
# VerificationInfoTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import VerificationInfoTypeDef


def get_value() -> VerificationInfoTypeDef:
    return {
        "LastCheckedTimestamp": ...,
    }


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
# SuppressedDestinationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SuppressedDestinationTypeDef


def get_value() -> SuppressedDestinationTypeDef:
    return {
        "EmailAddress": ...,
    }


# SuppressedDestinationTypeDef definition

class SuppressedDestinationTypeDef(TypedDict):
    EmailAddress: str,
    Reason: SuppressionListReasonType,  # (1)
    LastUpdateTime: datetime,
    Attributes: NotRequired[SuppressedDestinationAttributesTypeDef],  # (2)
```

1. See [:material-code-brackets: SuppressionListReasonType](./literals.md#suppressionlistreasontype) 
2. See [:material-code-braces: SuppressedDestinationAttributesTypeDef](./type_defs.md#suppresseddestinationattributestypedef) 
## BatchGetMetricDataRequestTypeDef

```python
# BatchGetMetricDataRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import BatchGetMetricDataRequestTypeDef


def get_value() -> BatchGetMetricDataRequestTypeDef:
    return {
        "Queries": ...,
    }


# BatchGetMetricDataRequestTypeDef definition

class BatchGetMetricDataRequestTypeDef(TypedDict):
    Queries: Sequence[BatchGetMetricDataQueryTypeDef],  # (1)
```

1. See [:material-code-braces: BatchGetMetricDataQueryTypeDef](./type_defs.md#batchgetmetricdataquerytypedef) 
## MessageTypeDef

```python
# MessageTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import MessageTypeDef


def get_value() -> MessageTypeDef:
    return {
        "Subject": ...,
    }


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
# EventDestinationTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import EventDestinationTypeDef


def get_value() -> EventDestinationTypeDef:
    return {
        "Name": ...,
    }


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
# InsightsEventTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import InsightsEventTypeDef


def get_value() -> InsightsEventTypeDef:
    return {
        "Timestamp": ...,
    }


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
# ListContactsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListContactsResponseTypeDef


def get_value() -> ListContactsResponseTypeDef:
    return {
        "Contacts": ...,
    }


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
# BulkEmailContentTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import BulkEmailContentTypeDef


def get_value() -> BulkEmailContentTypeDef:
    return {
        "Template": ...,
    }


# BulkEmailContentTypeDef definition

class BulkEmailContentTypeDef(TypedDict):
    Template: NotRequired[TemplateTypeDef],  # (1)
```

1. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
## GetDomainStatisticsReportResponseTypeDef

```python
# GetDomainStatisticsReportResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetDomainStatisticsReportResponseTypeDef


def get_value() -> GetDomainStatisticsReportResponseTypeDef:
    return {
        "OverallVolume": ...,
    }


# GetDomainStatisticsReportResponseTypeDef definition

class GetDomainStatisticsReportResponseTypeDef(TypedDict):
    OverallVolume: OverallVolumeTypeDef,  # (1)
    DailyVolumes: List[DailyVolumeTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: OverallVolumeTypeDef](./type_defs.md#overallvolumetypedef) 
2. See [:material-code-braces: DailyVolumeTypeDef](./type_defs.md#dailyvolumetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMultiRegionEndpointRequestTypeDef

```python
# CreateMultiRegionEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateMultiRegionEndpointRequestTypeDef


def get_value() -> CreateMultiRegionEndpointRequestTypeDef:
    return {
        "EndpointName": ...,
    }


# CreateMultiRegionEndpointRequestTypeDef definition

class CreateMultiRegionEndpointRequestTypeDef(TypedDict):
    EndpointName: str,
    Details: DetailsTypeDef,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: DetailsTypeDef](./type_defs.md#detailstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetDeliverabilityDashboardOptionsResponseTypeDef

```python
# GetDeliverabilityDashboardOptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetDeliverabilityDashboardOptionsResponseTypeDef


def get_value() -> GetDeliverabilityDashboardOptionsResponseTypeDef:
    return {
        "DashboardEnabled": ...,
    }


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
# GetDeliverabilityTestReportResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetDeliverabilityTestReportResponseTypeDef


def get_value() -> GetDeliverabilityTestReportResponseTypeDef:
    return {
        "DeliverabilityTestReport": ...,
    }


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
# GetAccountResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetAccountResponseTypeDef


def get_value() -> GetAccountResponseTypeDef:
    return {
        "DedicatedIpAutoWarmupEnabled": ...,
    }


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
## PutAccountVdmAttributesRequestTypeDef

```python
# PutAccountVdmAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutAccountVdmAttributesRequestTypeDef


def get_value() -> PutAccountVdmAttributesRequestTypeDef:
    return {
        "VdmAttributes": ...,
    }


# PutAccountVdmAttributesRequestTypeDef definition

class PutAccountVdmAttributesRequestTypeDef(TypedDict):
    VdmAttributes: VdmAttributesTypeDef,  # (1)
```

1. See [:material-code-braces: VdmAttributesTypeDef](./type_defs.md#vdmattributestypedef) 
## GetConfigurationSetResponseTypeDef

```python
# GetConfigurationSetResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetConfigurationSetResponseTypeDef


def get_value() -> GetConfigurationSetResponseTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


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
    ArchivingOptions: ArchivingOptionsTypeDef,  # (8)
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-braces: TrackingOptionsTypeDef](./type_defs.md#trackingoptionstypedef) 
2. See [:material-code-braces: DeliveryOptionsTypeDef](./type_defs.md#deliveryoptionstypedef) 
3. See [:material-code-braces: ReputationOptionsOutputTypeDef](./type_defs.md#reputationoptionsoutputtypedef) 
4. See [:material-code-braces: SendingOptionsTypeDef](./type_defs.md#sendingoptionstypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: SuppressionOptionsOutputTypeDef](./type_defs.md#suppressionoptionsoutputtypedef) 
7. See [:material-code-braces: VdmOptionsTypeDef](./type_defs.md#vdmoptionstypedef) 
8. See [:material-code-braces: ArchivingOptionsTypeDef](./type_defs.md#archivingoptionstypedef) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutConfigurationSetVdmOptionsRequestTypeDef

```python
# PutConfigurationSetVdmOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutConfigurationSetVdmOptionsRequestTypeDef


def get_value() -> PutConfigurationSetVdmOptionsRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# PutConfigurationSetVdmOptionsRequestTypeDef definition

class PutConfigurationSetVdmOptionsRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    VdmOptions: NotRequired[VdmOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: VdmOptionsTypeDef](./type_defs.md#vdmoptionstypedef) 
## CreateImportJobRequestTypeDef

```python
# CreateImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateImportJobRequestTypeDef


def get_value() -> CreateImportJobRequestTypeDef:
    return {
        "ImportDestination": ...,
    }


# CreateImportJobRequestTypeDef definition

class CreateImportJobRequestTypeDef(TypedDict):
    ImportDestination: ImportDestinationTypeDef,  # (1)
    ImportDataSource: ImportDataSourceTypeDef,  # (2)
```

1. See [:material-code-braces: ImportDestinationTypeDef](./type_defs.md#importdestinationtypedef) 
2. See [:material-code-braces: ImportDataSourceTypeDef](./type_defs.md#importdatasourcetypedef) 
## GetImportJobResponseTypeDef

```python
# GetImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetImportJobResponseTypeDef


def get_value() -> GetImportJobResponseTypeDef:
    return {
        "JobId": ...,
    }


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
# ImportJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ImportJobSummaryTypeDef


def get_value() -> ImportJobSummaryTypeDef:
    return {
        "JobId": ...,
    }


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
# DomainDeliverabilityTrackingOptionTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import DomainDeliverabilityTrackingOptionTypeDef


def get_value() -> DomainDeliverabilityTrackingOptionTypeDef:
    return {
        "Domain": ...,
    }


# DomainDeliverabilityTrackingOptionTypeDef definition

class DomainDeliverabilityTrackingOptionTypeDef(TypedDict):
    Domain: NotRequired[str],
    SubscriptionStartDate: NotRequired[TimestampTypeDef],
    InboxPlacementTrackingOption: NotRequired[InboxPlacementTrackingOptionUnionTypeDef],  # (1)
```

1. See [:material-code-braces: InboxPlacementTrackingOptionTypeDef](./type_defs.md#inboxplacementtrackingoptiontypedef) [:material-code-braces: InboxPlacementTrackingOptionOutputTypeDef](./type_defs.md#inboxplacementtrackingoptionoutputtypedef) 
## ListContactsRequestTypeDef

```python
# ListContactsRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListContactsRequestTypeDef


def get_value() -> ListContactsRequestTypeDef:
    return {
        "ContactListName": ...,
    }


# ListContactsRequestTypeDef definition

class ListContactsRequestTypeDef(TypedDict):
    ContactListName: str,
    Filter: NotRequired[ListContactsFilterTypeDef],  # (1)
    PageSize: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListContactsFilterTypeDef](./type_defs.md#listcontactsfiltertypedef) 
## ExportDataSourceOutputTypeDef

```python
# ExportDataSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ExportDataSourceOutputTypeDef


def get_value() -> ExportDataSourceOutputTypeDef:
    return {
        "MetricsDataSource": ...,
    }


# ExportDataSourceOutputTypeDef definition

class ExportDataSourceOutputTypeDef(TypedDict):
    MetricsDataSource: NotRequired[MetricsDataSourceOutputTypeDef],  # (1)
    MessageInsightsDataSource: NotRequired[MessageInsightsDataSourceOutputTypeDef],  # (2)
```

1. See [:material-code-braces: MetricsDataSourceOutputTypeDef](./type_defs.md#metricsdatasourceoutputtypedef) 
2. See [:material-code-braces: MessageInsightsDataSourceOutputTypeDef](./type_defs.md#messageinsightsdatasourceoutputtypedef) 
## ExportDataSourceTypeDef

```python
# ExportDataSourceTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ExportDataSourceTypeDef


def get_value() -> ExportDataSourceTypeDef:
    return {
        "MetricsDataSource": ...,
    }


# ExportDataSourceTypeDef definition

class ExportDataSourceTypeDef(TypedDict):
    MetricsDataSource: NotRequired[MetricsDataSourceTypeDef],  # (1)
    MessageInsightsDataSource: NotRequired[MessageInsightsDataSourceTypeDef],  # (2)
```

1. See [:material-code-braces: MetricsDataSourceTypeDef](./type_defs.md#metricsdatasourcetypedef) 
2. See [:material-code-braces: MessageInsightsDataSourceTypeDef](./type_defs.md#messageinsightsdatasourcetypedef) 
## BulkEmailEntryTypeDef

```python
# BulkEmailEntryTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import BulkEmailEntryTypeDef


def get_value() -> BulkEmailEntryTypeDef:
    return {
        "Destination": ...,
    }


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
# GetEmailIdentityResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetEmailIdentityResponseTypeDef


def get_value() -> GetEmailIdentityResponseTypeDef:
    return {
        "IdentityType": ...,
    }


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
# GetSuppressedDestinationResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetSuppressedDestinationResponseTypeDef


def get_value() -> GetSuppressedDestinationResponseTypeDef:
    return {
        "SuppressedDestination": ...,
    }


# GetSuppressedDestinationResponseTypeDef definition

class GetSuppressedDestinationResponseTypeDef(TypedDict):
    SuppressedDestination: SuppressedDestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SuppressedDestinationTypeDef](./type_defs.md#suppresseddestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfigurationSetRequestTypeDef

```python
# CreateConfigurationSetRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateConfigurationSetRequestTypeDef


def get_value() -> CreateConfigurationSetRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# CreateConfigurationSetRequestTypeDef definition

class CreateConfigurationSetRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    TrackingOptions: NotRequired[TrackingOptionsTypeDef],  # (1)
    DeliveryOptions: NotRequired[DeliveryOptionsTypeDef],  # (2)
    ReputationOptions: NotRequired[ReputationOptionsUnionTypeDef],  # (3)
    SendingOptions: NotRequired[SendingOptionsTypeDef],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
    SuppressionOptions: NotRequired[SuppressionOptionsUnionTypeDef],  # (6)
    VdmOptions: NotRequired[VdmOptionsTypeDef],  # (7)
    ArchivingOptions: NotRequired[ArchivingOptionsTypeDef],  # (8)
```

1. See [:material-code-braces: TrackingOptionsTypeDef](./type_defs.md#trackingoptionstypedef) 
2. See [:material-code-braces: DeliveryOptionsTypeDef](./type_defs.md#deliveryoptionstypedef) 
3. See [:material-code-braces: ReputationOptionsTypeDef](./type_defs.md#reputationoptionstypedef) [:material-code-braces: ReputationOptionsOutputTypeDef](./type_defs.md#reputationoptionsoutputtypedef) 
4. See [:material-code-braces: SendingOptionsTypeDef](./type_defs.md#sendingoptionstypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: SuppressionOptionsTypeDef](./type_defs.md#suppressionoptionstypedef) [:material-code-braces: SuppressionOptionsOutputTypeDef](./type_defs.md#suppressionoptionsoutputtypedef) 
7. See [:material-code-braces: VdmOptionsTypeDef](./type_defs.md#vdmoptionstypedef) 
8. See [:material-code-braces: ArchivingOptionsTypeDef](./type_defs.md#archivingoptionstypedef) 
## EmailContentTypeDef

```python
# EmailContentTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import EmailContentTypeDef


def get_value() -> EmailContentTypeDef:
    return {
        "Simple": ...,
    }


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
# GetConfigurationSetEventDestinationsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetConfigurationSetEventDestinationsResponseTypeDef


def get_value() -> GetConfigurationSetEventDestinationsResponseTypeDef:
    return {
        "EventDestinations": ...,
    }


# GetConfigurationSetEventDestinationsResponseTypeDef definition

class GetConfigurationSetEventDestinationsResponseTypeDef(TypedDict):
    EventDestinations: List[EventDestinationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventDestinationDefinitionTypeDef

```python
# EventDestinationDefinitionTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import EventDestinationDefinitionTypeDef


def get_value() -> EventDestinationDefinitionTypeDef:
    return {
        "Enabled": ...,
    }


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
# EmailInsightsTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import EmailInsightsTypeDef


def get_value() -> EmailInsightsTypeDef:
    return {
        "Destination": ...,
    }


# EmailInsightsTypeDef definition

class EmailInsightsTypeDef(TypedDict):
    Destination: NotRequired[str],
    Isp: NotRequired[str],
    Events: NotRequired[List[InsightsEventTypeDef]],  # (1)
```

1. See [:material-code-braces: InsightsEventTypeDef](./type_defs.md#insightseventtypedef) 
## ListImportJobsResponseTypeDef

```python
# ListImportJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import ListImportJobsResponseTypeDef


def get_value() -> ListImportJobsResponseTypeDef:
    return {
        "ImportJobs": ...,
    }


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
# GetExportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetExportJobResponseTypeDef


def get_value() -> GetExportJobResponseTypeDef:
    return {
        "JobId": ...,
    }


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
## SendBulkEmailRequestTypeDef

```python
# SendBulkEmailRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SendBulkEmailRequestTypeDef


def get_value() -> SendBulkEmailRequestTypeDef:
    return {
        "DefaultContent": ...,
    }


# SendBulkEmailRequestTypeDef definition

class SendBulkEmailRequestTypeDef(TypedDict):
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
## CreateDeliverabilityTestReportRequestTypeDef

```python
# CreateDeliverabilityTestReportRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateDeliverabilityTestReportRequestTypeDef


def get_value() -> CreateDeliverabilityTestReportRequestTypeDef:
    return {
        "FromEmailAddress": ...,
    }


# CreateDeliverabilityTestReportRequestTypeDef definition

class CreateDeliverabilityTestReportRequestTypeDef(TypedDict):
    FromEmailAddress: str,
    Content: EmailContentTypeDef,  # (1)
    ReportName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: EmailContentTypeDef](./type_defs.md#emailcontenttypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## SendEmailRequestTypeDef

```python
# SendEmailRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import SendEmailRequestTypeDef


def get_value() -> SendEmailRequestTypeDef:
    return {
        "Content": ...,
    }


# SendEmailRequestTypeDef definition

class SendEmailRequestTypeDef(TypedDict):
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
## CreateConfigurationSetEventDestinationRequestTypeDef

```python
# CreateConfigurationSetEventDestinationRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateConfigurationSetEventDestinationRequestTypeDef


def get_value() -> CreateConfigurationSetEventDestinationRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# CreateConfigurationSetEventDestinationRequestTypeDef definition

class CreateConfigurationSetEventDestinationRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
    EventDestination: EventDestinationDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 
## UpdateConfigurationSetEventDestinationRequestTypeDef

```python
# UpdateConfigurationSetEventDestinationRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import UpdateConfigurationSetEventDestinationRequestTypeDef


def get_value() -> UpdateConfigurationSetEventDestinationRequestTypeDef:
    return {
        "ConfigurationSetName": ...,
    }


# UpdateConfigurationSetEventDestinationRequestTypeDef definition

class UpdateConfigurationSetEventDestinationRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
    EventDestination: EventDestinationDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 
## GetMessageInsightsResponseTypeDef

```python
# GetMessageInsightsResponseTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import GetMessageInsightsResponseTypeDef


def get_value() -> GetMessageInsightsResponseTypeDef:
    return {
        "MessageId": ...,
    }


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
## PutDeliverabilityDashboardOptionRequestTypeDef

```python
# PutDeliverabilityDashboardOptionRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import PutDeliverabilityDashboardOptionRequestTypeDef


def get_value() -> PutDeliverabilityDashboardOptionRequestTypeDef:
    return {
        "DashboardEnabled": ...,
    }


# PutDeliverabilityDashboardOptionRequestTypeDef definition

class PutDeliverabilityDashboardOptionRequestTypeDef(TypedDict):
    DashboardEnabled: bool,
    SubscribedDomains: NotRequired[Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: DomainDeliverabilityTrackingOptionTypeDef](./type_defs.md#domaindeliverabilitytrackingoptiontypedef) [:material-code-braces: DomainDeliverabilityTrackingOptionOutputTypeDef](./type_defs.md#domaindeliverabilitytrackingoptionoutputtypedef) 
## CreateExportJobRequestTypeDef

```python
# CreateExportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_sesv2.type_defs import CreateExportJobRequestTypeDef


def get_value() -> CreateExportJobRequestTypeDef:
    return {
        "ExportDataSource": ...,
    }


# CreateExportJobRequestTypeDef definition

class CreateExportJobRequestTypeDef(TypedDict):
    ExportDataSource: ExportDataSourceUnionTypeDef,  # (1)
    ExportDestination: ExportDestinationTypeDef,  # (2)
```

1. See [:material-code-braces: ExportDataSourceTypeDef](./type_defs.md#exportdatasourcetypedef) [:material-code-braces: ExportDataSourceOutputTypeDef](./type_defs.md#exportdatasourceoutputtypedef) 
2. See [:material-code-braces: ExportDestinationTypeDef](./type_defs.md#exportdestinationtypedef) 
