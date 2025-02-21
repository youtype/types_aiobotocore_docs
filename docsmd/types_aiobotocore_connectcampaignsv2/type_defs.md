# Type definitions

> [Index](../README.md) > [ConnectCampaignServiceV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ConnectCampaignServiceV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaignsv2.html#connectcampaignservicev2)
    type annotations stubs module [types-aiobotocore-connectcampaignsv2](https://pypi.org/project/types-aiobotocore-connectcampaignsv2/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_connectcampaignsv2.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ScheduleUnionTypeDef

```python
# ScheduleUnionTypeDef Union usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ScheduleUnionTypeDef


def get_value() -> ScheduleUnionTypeDef:
    return ...


# ScheduleUnionTypeDef definition

ScheduleUnionTypeDef = Union[
    ScheduleTypeDef,  # (1)
    ScheduleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
2. See [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 

## CommunicationLimitsConfigUnionTypeDef

```python
# CommunicationLimitsConfigUnionTypeDef Union usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CommunicationLimitsConfigUnionTypeDef


def get_value() -> CommunicationLimitsConfigUnionTypeDef:
    return ...


# CommunicationLimitsConfigUnionTypeDef definition

CommunicationLimitsConfigUnionTypeDef = Union[
    CommunicationLimitsConfigTypeDef,  # (1)
    CommunicationLimitsConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CommunicationLimitsConfigTypeDef](./type_defs.md#communicationlimitsconfigtypedef) 
2. See [:material-code-braces: CommunicationLimitsConfigOutputTypeDef](./type_defs.md#communicationlimitsconfigoutputtypedef) 

## ChannelSubtypeConfigUnionTypeDef

```python
# ChannelSubtypeConfigUnionTypeDef Union usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ChannelSubtypeConfigUnionTypeDef


def get_value() -> ChannelSubtypeConfigUnionTypeDef:
    return ...


# ChannelSubtypeConfigUnionTypeDef definition

ChannelSubtypeConfigUnionTypeDef = Union[
    ChannelSubtypeConfigTypeDef,  # (1)
    ChannelSubtypeConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ChannelSubtypeConfigTypeDef](./type_defs.md#channelsubtypeconfigtypedef) 
2. See [:material-code-braces: ChannelSubtypeConfigOutputTypeDef](./type_defs.md#channelsubtypeconfigoutputtypedef) 

## CommunicationTimeConfigUnionTypeDef

```python
# CommunicationTimeConfigUnionTypeDef Union usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CommunicationTimeConfigUnionTypeDef


def get_value() -> CommunicationTimeConfigUnionTypeDef:
    return ...


# CommunicationTimeConfigUnionTypeDef definition

CommunicationTimeConfigUnionTypeDef = Union[
    CommunicationTimeConfigTypeDef,  # (1)
    CommunicationTimeConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CommunicationTimeConfigTypeDef](./type_defs.md#communicationtimeconfigtypedef) 
2. See [:material-code-braces: CommunicationTimeConfigOutputTypeDef](./type_defs.md#communicationtimeconfigoutputtypedef) 



## AnswerMachineDetectionConfigTypeDef

```python
# AnswerMachineDetectionConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import AnswerMachineDetectionConfigTypeDef


def get_value() -> AnswerMachineDetectionConfigTypeDef:
    return {
        "enableAnswerMachineDetection": ...,
    }


# AnswerMachineDetectionConfigTypeDef definition

class AnswerMachineDetectionConfigTypeDef(TypedDict):
    enableAnswerMachineDetection: bool,
    awaitAnswerMachinePrompt: NotRequired[bool],
```

## InstanceIdFilterTypeDef

```python
# InstanceIdFilterTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import InstanceIdFilterTypeDef


def get_value() -> InstanceIdFilterTypeDef:
    return {
        "value": ...,
    }


# InstanceIdFilterTypeDef definition

class InstanceIdFilterTypeDef(TypedDict):
    value: str,
    operator: InstanceIdFilterOperatorType,  # (1)
```

1. See [:material-code-brackets: InstanceIdFilterOperatorType](./literals.md#instanceidfilteroperatortype) 
## ScheduleOutputTypeDef

```python
# ScheduleOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ScheduleOutputTypeDef


def get_value() -> ScheduleOutputTypeDef:
    return {
        "startTime": ...,
    }


# ScheduleOutputTypeDef definition

class ScheduleOutputTypeDef(TypedDict):
    startTime: datetime,
    endTime: datetime,
    refreshFrequency: NotRequired[str],
```

## EmailChannelSubtypeParametersTypeDef

```python
# EmailChannelSubtypeParametersTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import EmailChannelSubtypeParametersTypeDef


def get_value() -> EmailChannelSubtypeParametersTypeDef:
    return {
        "destinationEmailAddress": ...,
    }


# EmailChannelSubtypeParametersTypeDef definition

class EmailChannelSubtypeParametersTypeDef(TypedDict):
    destinationEmailAddress: str,
    templateParameters: Mapping[str, str],
    connectSourceEmailAddress: NotRequired[str],
    templateArn: NotRequired[str],
```

## SmsChannelSubtypeParametersTypeDef

```python
# SmsChannelSubtypeParametersTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import SmsChannelSubtypeParametersTypeDef


def get_value() -> SmsChannelSubtypeParametersTypeDef:
    return {
        "destinationPhoneNumber": ...,
    }


# SmsChannelSubtypeParametersTypeDef definition

class SmsChannelSubtypeParametersTypeDef(TypedDict):
    destinationPhoneNumber: str,
    templateParameters: Mapping[str, str],
    connectSourcePhoneNumberArn: NotRequired[str],
    templateArn: NotRequired[str],
```

## CommunicationLimitTypeDef

```python
# CommunicationLimitTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CommunicationLimitTypeDef


def get_value() -> CommunicationLimitTypeDef:
    return {
        "maxCountPerRecipient": ...,
    }


# CommunicationLimitTypeDef definition

class CommunicationLimitTypeDef(TypedDict):
    maxCountPerRecipient: int,
    frequency: int,
    unit: CommunicationLimitTimeUnitType,  # (1)
```

1. See [:material-code-brackets: CommunicationLimitTimeUnitType](./literals.md#communicationlimittimeunittype) 
## LocalTimeZoneConfigOutputTypeDef

```python
# LocalTimeZoneConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import LocalTimeZoneConfigOutputTypeDef


def get_value() -> LocalTimeZoneConfigOutputTypeDef:
    return {
        "defaultTimeZone": ...,
    }


# LocalTimeZoneConfigOutputTypeDef definition

class LocalTimeZoneConfigOutputTypeDef(TypedDict):
    defaultTimeZone: NotRequired[str],
    localTimeZoneDetection: NotRequired[List[LocalTimeZoneDetectionTypeType]],  # (1)
```

1. See [:material-code-brackets: LocalTimeZoneDetectionTypeType](./literals.md#localtimezonedetectiontypetype) 
## LocalTimeZoneConfigTypeDef

```python
# LocalTimeZoneConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import LocalTimeZoneConfigTypeDef


def get_value() -> LocalTimeZoneConfigTypeDef:
    return {
        "defaultTimeZone": ...,
    }


# LocalTimeZoneConfigTypeDef definition

class LocalTimeZoneConfigTypeDef(TypedDict):
    defaultTimeZone: NotRequired[str],
    localTimeZoneDetection: NotRequired[Sequence[LocalTimeZoneDetectionTypeType]],  # (1)
```

1. See [:material-code-brackets: LocalTimeZoneDetectionTypeType](./literals.md#localtimezonedetectiontypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ResponseMetadataTypeDef


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

## CustomerProfilesIntegrationConfigTypeDef

```python
# CustomerProfilesIntegrationConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CustomerProfilesIntegrationConfigTypeDef


def get_value() -> CustomerProfilesIntegrationConfigTypeDef:
    return {
        "domainArn": ...,
    }


# CustomerProfilesIntegrationConfigTypeDef definition

class CustomerProfilesIntegrationConfigTypeDef(TypedDict):
    domainArn: str,
    objectTypeNames: Mapping[EventTypeType, str],  # (1)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
## CustomerProfilesIntegrationIdentifierTypeDef

```python
# CustomerProfilesIntegrationIdentifierTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CustomerProfilesIntegrationIdentifierTypeDef


def get_value() -> CustomerProfilesIntegrationIdentifierTypeDef:
    return {
        "domainArn": ...,
    }


# CustomerProfilesIntegrationIdentifierTypeDef definition

class CustomerProfilesIntegrationIdentifierTypeDef(TypedDict):
    domainArn: str,
```

## CustomerProfilesIntegrationSummaryTypeDef

```python
# CustomerProfilesIntegrationSummaryTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CustomerProfilesIntegrationSummaryTypeDef


def get_value() -> CustomerProfilesIntegrationSummaryTypeDef:
    return {
        "domainArn": ...,
    }


# CustomerProfilesIntegrationSummaryTypeDef definition

class CustomerProfilesIntegrationSummaryTypeDef(TypedDict):
    domainArn: str,
    objectTypeNames: Dict[EventTypeType, str],  # (1)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
## DeleteCampaignChannelSubtypeConfigRequestTypeDef

```python
# DeleteCampaignChannelSubtypeConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import DeleteCampaignChannelSubtypeConfigRequestTypeDef


def get_value() -> DeleteCampaignChannelSubtypeConfigRequestTypeDef:
    return {
        "id": ...,
    }


# DeleteCampaignChannelSubtypeConfigRequestTypeDef definition

class DeleteCampaignChannelSubtypeConfigRequestTypeDef(TypedDict):
    id: str,
    channelSubtype: ChannelSubtypeType,  # (1)
```

1. See [:material-code-brackets: ChannelSubtypeType](./literals.md#channelsubtypetype) 
## DeleteCampaignCommunicationLimitsRequestTypeDef

```python
# DeleteCampaignCommunicationLimitsRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import DeleteCampaignCommunicationLimitsRequestTypeDef


def get_value() -> DeleteCampaignCommunicationLimitsRequestTypeDef:
    return {
        "id": ...,
    }


# DeleteCampaignCommunicationLimitsRequestTypeDef definition

class DeleteCampaignCommunicationLimitsRequestTypeDef(TypedDict):
    id: str,
    config: CommunicationLimitsConfigTypeType,  # (1)
```

1. See [:material-code-brackets: CommunicationLimitsConfigTypeType](./literals.md#communicationlimitsconfigtypetype) 
## DeleteCampaignCommunicationTimeRequestTypeDef

```python
# DeleteCampaignCommunicationTimeRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import DeleteCampaignCommunicationTimeRequestTypeDef


def get_value() -> DeleteCampaignCommunicationTimeRequestTypeDef:
    return {
        "id": ...,
    }


# DeleteCampaignCommunicationTimeRequestTypeDef definition

class DeleteCampaignCommunicationTimeRequestTypeDef(TypedDict):
    id: str,
    config: CommunicationTimeConfigTypeType,  # (1)
```

1. See [:material-code-brackets: CommunicationTimeConfigTypeType](./literals.md#communicationtimeconfigtypetype) 
## DeleteCampaignRequestTypeDef

```python
# DeleteCampaignRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import DeleteCampaignRequestTypeDef


def get_value() -> DeleteCampaignRequestTypeDef:
    return {
        "id": ...,
    }


# DeleteCampaignRequestTypeDef definition

class DeleteCampaignRequestTypeDef(TypedDict):
    id: str,
```

## DeleteConnectInstanceConfigRequestTypeDef

```python
# DeleteConnectInstanceConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import DeleteConnectInstanceConfigRequestTypeDef


def get_value() -> DeleteConnectInstanceConfigRequestTypeDef:
    return {
        "connectInstanceId": ...,
    }


# DeleteConnectInstanceConfigRequestTypeDef definition

class DeleteConnectInstanceConfigRequestTypeDef(TypedDict):
    connectInstanceId: str,
    campaignDeletionPolicy: NotRequired[CampaignDeletionPolicyType],  # (1)
```

1. See [:material-code-brackets: CampaignDeletionPolicyType](./literals.md#campaigndeletionpolicytype) 
## DeleteInstanceOnboardingJobRequestTypeDef

```python
# DeleteInstanceOnboardingJobRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import DeleteInstanceOnboardingJobRequestTypeDef


def get_value() -> DeleteInstanceOnboardingJobRequestTypeDef:
    return {
        "connectInstanceId": ...,
    }


# DeleteInstanceOnboardingJobRequestTypeDef definition

class DeleteInstanceOnboardingJobRequestTypeDef(TypedDict):
    connectInstanceId: str,
```

## DescribeCampaignRequestTypeDef

```python
# DescribeCampaignRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import DescribeCampaignRequestTypeDef


def get_value() -> DescribeCampaignRequestTypeDef:
    return {
        "id": ...,
    }


# DescribeCampaignRequestTypeDef definition

class DescribeCampaignRequestTypeDef(TypedDict):
    id: str,
```

## EmailOutboundConfigTypeDef

```python
# EmailOutboundConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import EmailOutboundConfigTypeDef


def get_value() -> EmailOutboundConfigTypeDef:
    return {
        "connectSourceEmailAddress": ...,
    }


# EmailOutboundConfigTypeDef definition

class EmailOutboundConfigTypeDef(TypedDict):
    connectSourceEmailAddress: str,
    wisdomTemplateArn: str,
    sourceEmailAddressDisplayName: NotRequired[str],
```

## EmailOutboundModeOutputTypeDef

```python
# EmailOutboundModeOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import EmailOutboundModeOutputTypeDef


def get_value() -> EmailOutboundModeOutputTypeDef:
    return {
        "agentless": ...,
    }


# EmailOutboundModeOutputTypeDef definition

class EmailOutboundModeOutputTypeDef(TypedDict):
    agentless: NotRequired[Dict[str, Any]],
```

## EmailOutboundModeTypeDef

```python
# EmailOutboundModeTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import EmailOutboundModeTypeDef


def get_value() -> EmailOutboundModeTypeDef:
    return {
        "agentless": ...,
    }


# EmailOutboundModeTypeDef definition

class EmailOutboundModeTypeDef(TypedDict):
    agentless: NotRequired[Mapping[str, Any]],
```

## EncryptionConfigTypeDef

```python
# EncryptionConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import EncryptionConfigTypeDef


def get_value() -> EncryptionConfigTypeDef:
    return {
        "enabled": ...,
    }


# EncryptionConfigTypeDef definition

class EncryptionConfigTypeDef(TypedDict):
    enabled: bool,
    encryptionType: NotRequired[EncryptionTypeType],  # (1)
    keyArn: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## EventTriggerTypeDef

```python
# EventTriggerTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import EventTriggerTypeDef


def get_value() -> EventTriggerTypeDef:
    return {
        "customerProfilesDomainArn": ...,
    }


# EventTriggerTypeDef definition

class EventTriggerTypeDef(TypedDict):
    customerProfilesDomainArn: NotRequired[str],
```

## FailedCampaignStateResponseTypeDef

```python
# FailedCampaignStateResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import FailedCampaignStateResponseTypeDef


def get_value() -> FailedCampaignStateResponseTypeDef:
    return {
        "campaignId": ...,
    }


# FailedCampaignStateResponseTypeDef definition

class FailedCampaignStateResponseTypeDef(TypedDict):
    campaignId: NotRequired[str],
    failureCode: NotRequired[GetCampaignStateBatchFailureCodeType],  # (1)
```

1. See [:material-code-brackets: GetCampaignStateBatchFailureCodeType](./literals.md#getcampaignstatebatchfailurecodetype) 
## FailedProfileOutboundRequestTypeDef

```python
# FailedProfileOutboundRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import FailedProfileOutboundRequestTypeDef


def get_value() -> FailedProfileOutboundRequestTypeDef:
    return {
        "clientToken": ...,
    }


# FailedProfileOutboundRequestTypeDef definition

class FailedProfileOutboundRequestTypeDef(TypedDict):
    clientToken: NotRequired[str],
    id: NotRequired[str],
    failureCode: NotRequired[ProfileOutboundRequestFailureCodeType],  # (1)
```

1. See [:material-code-brackets: ProfileOutboundRequestFailureCodeType](./literals.md#profileoutboundrequestfailurecodetype) 
## FailedRequestTypeDef

```python
# FailedRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import FailedRequestTypeDef


def get_value() -> FailedRequestTypeDef:
    return {
        "clientToken": ...,
    }


# FailedRequestTypeDef definition

class FailedRequestTypeDef(TypedDict):
    clientToken: NotRequired[str],
    id: NotRequired[str],
    failureCode: NotRequired[FailureCodeType],  # (1)
```

1. See [:material-code-brackets: FailureCodeType](./literals.md#failurecodetype) 
## GetCampaignStateBatchRequestTypeDef

```python
# GetCampaignStateBatchRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import GetCampaignStateBatchRequestTypeDef


def get_value() -> GetCampaignStateBatchRequestTypeDef:
    return {
        "campaignIds": ...,
    }


# GetCampaignStateBatchRequestTypeDef definition

class GetCampaignStateBatchRequestTypeDef(TypedDict):
    campaignIds: Sequence[str],
```

## SuccessfulCampaignStateResponseTypeDef

```python
# SuccessfulCampaignStateResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import SuccessfulCampaignStateResponseTypeDef


def get_value() -> SuccessfulCampaignStateResponseTypeDef:
    return {
        "campaignId": ...,
    }


# SuccessfulCampaignStateResponseTypeDef definition

class SuccessfulCampaignStateResponseTypeDef(TypedDict):
    campaignId: NotRequired[str],
    state: NotRequired[CampaignStateType],  # (1)
```

1. See [:material-code-brackets: CampaignStateType](./literals.md#campaignstatetype) 
## GetCampaignStateRequestTypeDef

```python
# GetCampaignStateRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import GetCampaignStateRequestTypeDef


def get_value() -> GetCampaignStateRequestTypeDef:
    return {
        "id": ...,
    }


# GetCampaignStateRequestTypeDef definition

class GetCampaignStateRequestTypeDef(TypedDict):
    id: str,
```

## GetConnectInstanceConfigRequestTypeDef

```python
# GetConnectInstanceConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import GetConnectInstanceConfigRequestTypeDef


def get_value() -> GetConnectInstanceConfigRequestTypeDef:
    return {
        "connectInstanceId": ...,
    }


# GetConnectInstanceConfigRequestTypeDef definition

class GetConnectInstanceConfigRequestTypeDef(TypedDict):
    connectInstanceId: str,
```

## GetInstanceOnboardingJobStatusRequestTypeDef

```python
# GetInstanceOnboardingJobStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import GetInstanceOnboardingJobStatusRequestTypeDef


def get_value() -> GetInstanceOnboardingJobStatusRequestTypeDef:
    return {
        "connectInstanceId": ...,
    }


# GetInstanceOnboardingJobStatusRequestTypeDef definition

class GetInstanceOnboardingJobStatusRequestTypeDef(TypedDict):
    connectInstanceId: str,
```

## InstanceOnboardingJobStatusTypeDef

```python
# InstanceOnboardingJobStatusTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import InstanceOnboardingJobStatusTypeDef


def get_value() -> InstanceOnboardingJobStatusTypeDef:
    return {
        "connectInstanceId": ...,
    }


# InstanceOnboardingJobStatusTypeDef definition

class InstanceOnboardingJobStatusTypeDef(TypedDict):
    connectInstanceId: str,
    status: InstanceOnboardingJobStatusCodeType,  # (1)
    failureCode: NotRequired[InstanceOnboardingJobFailureCodeType],  # (2)
```

1. See [:material-code-brackets: InstanceOnboardingJobStatusCodeType](./literals.md#instanceonboardingjobstatuscodetype) 
2. See [:material-code-brackets: InstanceOnboardingJobFailureCodeType](./literals.md#instanceonboardingjobfailurecodetype) 
## QConnectIntegrationConfigTypeDef

```python
# QConnectIntegrationConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import QConnectIntegrationConfigTypeDef


def get_value() -> QConnectIntegrationConfigTypeDef:
    return {
        "knowledgeBaseArn": ...,
    }


# QConnectIntegrationConfigTypeDef definition

class QConnectIntegrationConfigTypeDef(TypedDict):
    knowledgeBaseArn: str,
```

## QConnectIntegrationIdentifierTypeDef

```python
# QConnectIntegrationIdentifierTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import QConnectIntegrationIdentifierTypeDef


def get_value() -> QConnectIntegrationIdentifierTypeDef:
    return {
        "knowledgeBaseArn": ...,
    }


# QConnectIntegrationIdentifierTypeDef definition

class QConnectIntegrationIdentifierTypeDef(TypedDict):
    knowledgeBaseArn: str,
```

## QConnectIntegrationSummaryTypeDef

```python
# QConnectIntegrationSummaryTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import QConnectIntegrationSummaryTypeDef


def get_value() -> QConnectIntegrationSummaryTypeDef:
    return {
        "knowledgeBaseArn": ...,
    }


# QConnectIntegrationSummaryTypeDef definition

class QConnectIntegrationSummaryTypeDef(TypedDict):
    knowledgeBaseArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import PaginatorConfigTypeDef


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

## ListConnectInstanceIntegrationsRequestTypeDef

```python
# ListConnectInstanceIntegrationsRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ListConnectInstanceIntegrationsRequestTypeDef


def get_value() -> ListConnectInstanceIntegrationsRequestTypeDef:
    return {
        "connectInstanceId": ...,
    }


# ListConnectInstanceIntegrationsRequestTypeDef definition

class ListConnectInstanceIntegrationsRequestTypeDef(TypedDict):
    connectInstanceId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "arn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    arn: str,
```

## TimeRangeTypeDef

```python
# TimeRangeTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import TimeRangeTypeDef


def get_value() -> TimeRangeTypeDef:
    return {
        "startTime": ...,
    }


# TimeRangeTypeDef definition

class TimeRangeTypeDef(TypedDict):
    startTime: str,
    endTime: str,
```

## PauseCampaignRequestTypeDef

```python
# PauseCampaignRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import PauseCampaignRequestTypeDef


def get_value() -> PauseCampaignRequestTypeDef:
    return {
        "id": ...,
    }


# PauseCampaignRequestTypeDef definition

class PauseCampaignRequestTypeDef(TypedDict):
    id: str,
```

## PredictiveConfigTypeDef

```python
# PredictiveConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import PredictiveConfigTypeDef


def get_value() -> PredictiveConfigTypeDef:
    return {
        "bandwidthAllocation": ...,
    }


# PredictiveConfigTypeDef definition

class PredictiveConfigTypeDef(TypedDict):
    bandwidthAllocation: float,
```

## ProgressiveConfigTypeDef

```python
# ProgressiveConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ProgressiveConfigTypeDef


def get_value() -> ProgressiveConfigTypeDef:
    return {
        "bandwidthAllocation": ...,
    }


# ProgressiveConfigTypeDef definition

class ProgressiveConfigTypeDef(TypedDict):
    bandwidthAllocation: float,
```

## SuccessfulRequestTypeDef

```python
# SuccessfulRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import SuccessfulRequestTypeDef


def get_value() -> SuccessfulRequestTypeDef:
    return {
        "clientToken": ...,
    }


# SuccessfulRequestTypeDef definition

class SuccessfulRequestTypeDef(TypedDict):
    clientToken: NotRequired[str],
    id: NotRequired[str],
```

## SuccessfulProfileOutboundRequestTypeDef

```python
# SuccessfulProfileOutboundRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import SuccessfulProfileOutboundRequestTypeDef


def get_value() -> SuccessfulProfileOutboundRequestTypeDef:
    return {
        "clientToken": ...,
    }


# SuccessfulProfileOutboundRequestTypeDef definition

class SuccessfulProfileOutboundRequestTypeDef(TypedDict):
    clientToken: NotRequired[str],
    id: NotRequired[str],
```

## RestrictedPeriodTypeDef

```python
# RestrictedPeriodTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import RestrictedPeriodTypeDef


def get_value() -> RestrictedPeriodTypeDef:
    return {
        "name": ...,
    }


# RestrictedPeriodTypeDef definition

class RestrictedPeriodTypeDef(TypedDict):
    startDate: str,
    endDate: str,
    name: NotRequired[str],
```

## ResumeCampaignRequestTypeDef

```python
# ResumeCampaignRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ResumeCampaignRequestTypeDef


def get_value() -> ResumeCampaignRequestTypeDef:
    return {
        "id": ...,
    }


# ResumeCampaignRequestTypeDef definition

class ResumeCampaignRequestTypeDef(TypedDict):
    id: str,
```

## SmsOutboundConfigTypeDef

```python
# SmsOutboundConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import SmsOutboundConfigTypeDef


def get_value() -> SmsOutboundConfigTypeDef:
    return {
        "connectSourcePhoneNumberArn": ...,
    }


# SmsOutboundConfigTypeDef definition

class SmsOutboundConfigTypeDef(TypedDict):
    connectSourcePhoneNumberArn: str,
    wisdomTemplateArn: str,
```

## SmsOutboundModeOutputTypeDef

```python
# SmsOutboundModeOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import SmsOutboundModeOutputTypeDef


def get_value() -> SmsOutboundModeOutputTypeDef:
    return {
        "agentless": ...,
    }


# SmsOutboundModeOutputTypeDef definition

class SmsOutboundModeOutputTypeDef(TypedDict):
    agentless: NotRequired[Dict[str, Any]],
```

## SmsOutboundModeTypeDef

```python
# SmsOutboundModeTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import SmsOutboundModeTypeDef


def get_value() -> SmsOutboundModeTypeDef:
    return {
        "agentless": ...,
    }


# SmsOutboundModeTypeDef definition

class SmsOutboundModeTypeDef(TypedDict):
    agentless: NotRequired[Mapping[str, Any]],
```

## StartCampaignRequestTypeDef

```python
# StartCampaignRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import StartCampaignRequestTypeDef


def get_value() -> StartCampaignRequestTypeDef:
    return {
        "id": ...,
    }


# StartCampaignRequestTypeDef definition

class StartCampaignRequestTypeDef(TypedDict):
    id: str,
```

## StopCampaignRequestTypeDef

```python
# StopCampaignRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import StopCampaignRequestTypeDef


def get_value() -> StopCampaignRequestTypeDef:
    return {
        "id": ...,
    }


# StopCampaignRequestTypeDef definition

class StopCampaignRequestTypeDef(TypedDict):
    id: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "arn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    arn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "arn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    arn: str,
    tagKeys: Sequence[str],
```

## UpdateCampaignFlowAssociationRequestTypeDef

```python
# UpdateCampaignFlowAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import UpdateCampaignFlowAssociationRequestTypeDef


def get_value() -> UpdateCampaignFlowAssociationRequestTypeDef:
    return {
        "id": ...,
    }


# UpdateCampaignFlowAssociationRequestTypeDef definition

class UpdateCampaignFlowAssociationRequestTypeDef(TypedDict):
    id: str,
    connectCampaignFlowArn: str,
```

## UpdateCampaignNameRequestTypeDef

```python
# UpdateCampaignNameRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import UpdateCampaignNameRequestTypeDef


def get_value() -> UpdateCampaignNameRequestTypeDef:
    return {
        "id": ...,
    }


# UpdateCampaignNameRequestTypeDef definition

class UpdateCampaignNameRequestTypeDef(TypedDict):
    id: str,
    name: str,
```

## TelephonyChannelSubtypeParametersTypeDef

```python
# TelephonyChannelSubtypeParametersTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import TelephonyChannelSubtypeParametersTypeDef


def get_value() -> TelephonyChannelSubtypeParametersTypeDef:
    return {
        "destinationPhoneNumber": ...,
    }


# TelephonyChannelSubtypeParametersTypeDef definition

class TelephonyChannelSubtypeParametersTypeDef(TypedDict):
    destinationPhoneNumber: str,
    attributes: Mapping[str, str],
    connectSourcePhoneNumber: NotRequired[str],
    answerMachineDetectionConfig: NotRequired[AnswerMachineDetectionConfigTypeDef],  # (1)
```

1. See [:material-code-braces: AnswerMachineDetectionConfigTypeDef](./type_defs.md#answermachinedetectionconfigtypedef) 
## TelephonyOutboundConfigTypeDef

```python
# TelephonyOutboundConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import TelephonyOutboundConfigTypeDef


def get_value() -> TelephonyOutboundConfigTypeDef:
    return {
        "connectContactFlowId": ...,
    }


# TelephonyOutboundConfigTypeDef definition

class TelephonyOutboundConfigTypeDef(TypedDict):
    connectContactFlowId: str,
    connectSourcePhoneNumber: NotRequired[str],
    answerMachineDetectionConfig: NotRequired[AnswerMachineDetectionConfigTypeDef],  # (1)
```

1. See [:material-code-braces: AnswerMachineDetectionConfigTypeDef](./type_defs.md#answermachinedetectionconfigtypedef) 
## CampaignFiltersTypeDef

```python
# CampaignFiltersTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CampaignFiltersTypeDef


def get_value() -> CampaignFiltersTypeDef:
    return {
        "instanceIdFilter": ...,
    }


# CampaignFiltersTypeDef definition

class CampaignFiltersTypeDef(TypedDict):
    instanceIdFilter: NotRequired[InstanceIdFilterTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceIdFilterTypeDef](./type_defs.md#instanceidfiltertypedef) 
## CampaignSummaryTypeDef

```python
# CampaignSummaryTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CampaignSummaryTypeDef


def get_value() -> CampaignSummaryTypeDef:
    return {
        "id": ...,
    }


# CampaignSummaryTypeDef definition

class CampaignSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    connectInstanceId: str,
    channelSubtypes: List[ChannelSubtypeType],  # (1)
    schedule: NotRequired[ScheduleOutputTypeDef],  # (2)
    connectCampaignFlowArn: NotRequired[str],
```

1. See [:material-code-brackets: ChannelSubtypeType](./literals.md#channelsubtypetype) 
2. See [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
## CommunicationLimitsOutputTypeDef

```python
# CommunicationLimitsOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CommunicationLimitsOutputTypeDef


def get_value() -> CommunicationLimitsOutputTypeDef:
    return {
        "communicationLimitsList": ...,
    }


# CommunicationLimitsOutputTypeDef definition

class CommunicationLimitsOutputTypeDef(TypedDict):
    communicationLimitsList: NotRequired[List[CommunicationLimitTypeDef]],  # (1)
```

1. See [:material-code-braces: CommunicationLimitTypeDef](./type_defs.md#communicationlimittypedef) 
## CommunicationLimitsTypeDef

```python
# CommunicationLimitsTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CommunicationLimitsTypeDef


def get_value() -> CommunicationLimitsTypeDef:
    return {
        "communicationLimitsList": ...,
    }


# CommunicationLimitsTypeDef definition

class CommunicationLimitsTypeDef(TypedDict):
    communicationLimitsList: NotRequired[Sequence[CommunicationLimitTypeDef]],  # (1)
```

1. See [:material-code-braces: CommunicationLimitTypeDef](./type_defs.md#communicationlimittypedef) 
## CreateCampaignResponseTypeDef

```python
# CreateCampaignResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CreateCampaignResponseTypeDef


def get_value() -> CreateCampaignResponseTypeDef:
    return {
        "id": ...,
    }


# CreateCampaignResponseTypeDef definition

class CreateCampaignResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCampaignStateResponseTypeDef

```python
# GetCampaignStateResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import GetCampaignStateResponseTypeDef


def get_value() -> GetCampaignStateResponseTypeDef:
    return {
        "state": ...,
    }


# GetCampaignStateResponseTypeDef definition

class GetCampaignStateResponseTypeDef(TypedDict):
    state: CampaignStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CampaignStateType](./literals.md#campaignstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmailChannelSubtypeConfigOutputTypeDef

```python
# EmailChannelSubtypeConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import EmailChannelSubtypeConfigOutputTypeDef


def get_value() -> EmailChannelSubtypeConfigOutputTypeDef:
    return {
        "capacity": ...,
    }


# EmailChannelSubtypeConfigOutputTypeDef definition

class EmailChannelSubtypeConfigOutputTypeDef(TypedDict):
    outboundMode: EmailOutboundModeOutputTypeDef,  # (1)
    defaultOutboundConfig: EmailOutboundConfigTypeDef,  # (2)
    capacity: NotRequired[float],
```

1. See [:material-code-braces: EmailOutboundModeOutputTypeDef](./type_defs.md#emailoutboundmodeoutputtypedef) 
2. See [:material-code-braces: EmailOutboundConfigTypeDef](./type_defs.md#emailoutboundconfigtypedef) 
## EmailChannelSubtypeConfigTypeDef

```python
# EmailChannelSubtypeConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import EmailChannelSubtypeConfigTypeDef


def get_value() -> EmailChannelSubtypeConfigTypeDef:
    return {
        "capacity": ...,
    }


# EmailChannelSubtypeConfigTypeDef definition

class EmailChannelSubtypeConfigTypeDef(TypedDict):
    outboundMode: EmailOutboundModeTypeDef,  # (1)
    defaultOutboundConfig: EmailOutboundConfigTypeDef,  # (2)
    capacity: NotRequired[float],
```

1. See [:material-code-braces: EmailOutboundModeTypeDef](./type_defs.md#emailoutboundmodetypedef) 
2. See [:material-code-braces: EmailOutboundConfigTypeDef](./type_defs.md#emailoutboundconfigtypedef) 
## InstanceConfigTypeDef

```python
# InstanceConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import InstanceConfigTypeDef


def get_value() -> InstanceConfigTypeDef:
    return {
        "connectInstanceId": ...,
    }


# InstanceConfigTypeDef definition

class InstanceConfigTypeDef(TypedDict):
    connectInstanceId: str,
    serviceLinkedRoleArn: str,
    encryptionConfig: EncryptionConfigTypeDef,  # (1)
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
## StartInstanceOnboardingJobRequestTypeDef

```python
# StartInstanceOnboardingJobRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import StartInstanceOnboardingJobRequestTypeDef


def get_value() -> StartInstanceOnboardingJobRequestTypeDef:
    return {
        "connectInstanceId": ...,
    }


# StartInstanceOnboardingJobRequestTypeDef definition

class StartInstanceOnboardingJobRequestTypeDef(TypedDict):
    connectInstanceId: str,
    encryptionConfig: EncryptionConfigTypeDef,  # (1)
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
## SourceTypeDef

```python
# SourceTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import SourceTypeDef


def get_value() -> SourceTypeDef:
    return {
        "customerProfilesSegmentArn": ...,
    }


# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    customerProfilesSegmentArn: NotRequired[str],
    eventTrigger: NotRequired[EventTriggerTypeDef],  # (1)
```

1. See [:material-code-braces: EventTriggerTypeDef](./type_defs.md#eventtriggertypedef) 
## GetCampaignStateBatchResponseTypeDef

```python
# GetCampaignStateBatchResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import GetCampaignStateBatchResponseTypeDef


def get_value() -> GetCampaignStateBatchResponseTypeDef:
    return {
        "successfulRequests": ...,
    }


# GetCampaignStateBatchResponseTypeDef definition

class GetCampaignStateBatchResponseTypeDef(TypedDict):
    successfulRequests: List[SuccessfulCampaignStateResponseTypeDef],  # (1)
    failedRequests: List[FailedCampaignStateResponseTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SuccessfulCampaignStateResponseTypeDef](./type_defs.md#successfulcampaignstateresponsetypedef) 
2. See [:material-code-braces: FailedCampaignStateResponseTypeDef](./type_defs.md#failedcampaignstateresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstanceOnboardingJobStatusResponseTypeDef

```python
# GetInstanceOnboardingJobStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import GetInstanceOnboardingJobStatusResponseTypeDef


def get_value() -> GetInstanceOnboardingJobStatusResponseTypeDef:
    return {
        "connectInstanceOnboardingJobStatus": ...,
    }


# GetInstanceOnboardingJobStatusResponseTypeDef definition

class GetInstanceOnboardingJobStatusResponseTypeDef(TypedDict):
    connectInstanceOnboardingJobStatus: InstanceOnboardingJobStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceOnboardingJobStatusTypeDef](./type_defs.md#instanceonboardingjobstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartInstanceOnboardingJobResponseTypeDef

```python
# StartInstanceOnboardingJobResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import StartInstanceOnboardingJobResponseTypeDef


def get_value() -> StartInstanceOnboardingJobResponseTypeDef:
    return {
        "connectInstanceOnboardingJobStatus": ...,
    }


# StartInstanceOnboardingJobResponseTypeDef definition

class StartInstanceOnboardingJobResponseTypeDef(TypedDict):
    connectInstanceOnboardingJobStatus: InstanceOnboardingJobStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceOnboardingJobStatusTypeDef](./type_defs.md#instanceonboardingjobstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntegrationConfigTypeDef

```python
# IntegrationConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import IntegrationConfigTypeDef


def get_value() -> IntegrationConfigTypeDef:
    return {
        "customerProfiles": ...,
    }


# IntegrationConfigTypeDef definition

class IntegrationConfigTypeDef(TypedDict):
    customerProfiles: NotRequired[CustomerProfilesIntegrationConfigTypeDef],  # (1)
    qConnect: NotRequired[QConnectIntegrationConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CustomerProfilesIntegrationConfigTypeDef](./type_defs.md#customerprofilesintegrationconfigtypedef) 
2. See [:material-code-braces: QConnectIntegrationConfigTypeDef](./type_defs.md#qconnectintegrationconfigtypedef) 
## IntegrationIdentifierTypeDef

```python
# IntegrationIdentifierTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import IntegrationIdentifierTypeDef


def get_value() -> IntegrationIdentifierTypeDef:
    return {
        "customerProfiles": ...,
    }


# IntegrationIdentifierTypeDef definition

class IntegrationIdentifierTypeDef(TypedDict):
    customerProfiles: NotRequired[CustomerProfilesIntegrationIdentifierTypeDef],  # (1)
    qConnect: NotRequired[QConnectIntegrationIdentifierTypeDef],  # (2)
```

1. See [:material-code-braces: CustomerProfilesIntegrationIdentifierTypeDef](./type_defs.md#customerprofilesintegrationidentifiertypedef) 
2. See [:material-code-braces: QConnectIntegrationIdentifierTypeDef](./type_defs.md#qconnectintegrationidentifiertypedef) 
## IntegrationSummaryTypeDef

```python
# IntegrationSummaryTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import IntegrationSummaryTypeDef


def get_value() -> IntegrationSummaryTypeDef:
    return {
        "customerProfiles": ...,
    }


# IntegrationSummaryTypeDef definition

class IntegrationSummaryTypeDef(TypedDict):
    customerProfiles: NotRequired[CustomerProfilesIntegrationSummaryTypeDef],  # (1)
    qConnect: NotRequired[QConnectIntegrationSummaryTypeDef],  # (2)
```

1. See [:material-code-braces: CustomerProfilesIntegrationSummaryTypeDef](./type_defs.md#customerprofilesintegrationsummarytypedef) 
2. See [:material-code-braces: QConnectIntegrationSummaryTypeDef](./type_defs.md#qconnectintegrationsummarytypedef) 
## ListConnectInstanceIntegrationsRequestPaginateTypeDef

```python
# ListConnectInstanceIntegrationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ListConnectInstanceIntegrationsRequestPaginateTypeDef


def get_value() -> ListConnectInstanceIntegrationsRequestPaginateTypeDef:
    return {
        "connectInstanceId": ...,
    }


# ListConnectInstanceIntegrationsRequestPaginateTypeDef definition

class ListConnectInstanceIntegrationsRequestPaginateTypeDef(TypedDict):
    connectInstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## OpenHoursOutputTypeDef

```python
# OpenHoursOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import OpenHoursOutputTypeDef


def get_value() -> OpenHoursOutputTypeDef:
    return {
        "dailyHours": ...,
    }


# OpenHoursOutputTypeDef definition

class OpenHoursOutputTypeDef(TypedDict):
    dailyHours: NotRequired[Dict[DayOfWeekType, List[TimeRangeTypeDef]]],  # (1)
```

1. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
## OpenHoursTypeDef

```python
# OpenHoursTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import OpenHoursTypeDef


def get_value() -> OpenHoursTypeDef:
    return {
        "dailyHours": ...,
    }


# OpenHoursTypeDef definition

class OpenHoursTypeDef(TypedDict):
    dailyHours: NotRequired[Mapping[DayOfWeekType, Sequence[TimeRangeTypeDef]]],  # (1)
```

1. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
## ProfileOutboundRequestTypeDef

```python
# ProfileOutboundRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ProfileOutboundRequestTypeDef


def get_value() -> ProfileOutboundRequestTypeDef:
    return {
        "clientToken": ...,
    }


# ProfileOutboundRequestTypeDef definition

class ProfileOutboundRequestTypeDef(TypedDict):
    clientToken: str,
    profileId: str,
    expirationTime: NotRequired[TimestampTypeDef],
```

## ScheduleTypeDef

```python
# ScheduleTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ScheduleTypeDef


def get_value() -> ScheduleTypeDef:
    return {
        "startTime": ...,
    }


# ScheduleTypeDef definition

class ScheduleTypeDef(TypedDict):
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    refreshFrequency: NotRequired[str],
```

## TelephonyOutboundModeOutputTypeDef

```python
# TelephonyOutboundModeOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import TelephonyOutboundModeOutputTypeDef


def get_value() -> TelephonyOutboundModeOutputTypeDef:
    return {
        "progressive": ...,
    }


# TelephonyOutboundModeOutputTypeDef definition

class TelephonyOutboundModeOutputTypeDef(TypedDict):
    progressive: NotRequired[ProgressiveConfigTypeDef],  # (1)
    predictive: NotRequired[PredictiveConfigTypeDef],  # (2)
    agentless: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: ProgressiveConfigTypeDef](./type_defs.md#progressiveconfigtypedef) 
2. See [:material-code-braces: PredictiveConfigTypeDef](./type_defs.md#predictiveconfigtypedef) 
## TelephonyOutboundModeTypeDef

```python
# TelephonyOutboundModeTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import TelephonyOutboundModeTypeDef


def get_value() -> TelephonyOutboundModeTypeDef:
    return {
        "progressive": ...,
    }


# TelephonyOutboundModeTypeDef definition

class TelephonyOutboundModeTypeDef(TypedDict):
    progressive: NotRequired[ProgressiveConfigTypeDef],  # (1)
    predictive: NotRequired[PredictiveConfigTypeDef],  # (2)
    agentless: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: ProgressiveConfigTypeDef](./type_defs.md#progressiveconfigtypedef) 
2. See [:material-code-braces: PredictiveConfigTypeDef](./type_defs.md#predictiveconfigtypedef) 
## PutOutboundRequestBatchResponseTypeDef

```python
# PutOutboundRequestBatchResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import PutOutboundRequestBatchResponseTypeDef


def get_value() -> PutOutboundRequestBatchResponseTypeDef:
    return {
        "successfulRequests": ...,
    }


# PutOutboundRequestBatchResponseTypeDef definition

class PutOutboundRequestBatchResponseTypeDef(TypedDict):
    successfulRequests: List[SuccessfulRequestTypeDef],  # (1)
    failedRequests: List[FailedRequestTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SuccessfulRequestTypeDef](./type_defs.md#successfulrequesttypedef) 
2. See [:material-code-braces: FailedRequestTypeDef](./type_defs.md#failedrequesttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutProfileOutboundRequestBatchResponseTypeDef

```python
# PutProfileOutboundRequestBatchResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import PutProfileOutboundRequestBatchResponseTypeDef


def get_value() -> PutProfileOutboundRequestBatchResponseTypeDef:
    return {
        "successfulRequests": ...,
    }


# PutProfileOutboundRequestBatchResponseTypeDef definition

class PutProfileOutboundRequestBatchResponseTypeDef(TypedDict):
    successfulRequests: List[SuccessfulProfileOutboundRequestTypeDef],  # (1)
    failedRequests: List[FailedProfileOutboundRequestTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SuccessfulProfileOutboundRequestTypeDef](./type_defs.md#successfulprofileoutboundrequesttypedef) 
2. See [:material-code-braces: FailedProfileOutboundRequestTypeDef](./type_defs.md#failedprofileoutboundrequesttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestrictedPeriodsOutputTypeDef

```python
# RestrictedPeriodsOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import RestrictedPeriodsOutputTypeDef


def get_value() -> RestrictedPeriodsOutputTypeDef:
    return {
        "restrictedPeriodList": ...,
    }


# RestrictedPeriodsOutputTypeDef definition

class RestrictedPeriodsOutputTypeDef(TypedDict):
    restrictedPeriodList: NotRequired[List[RestrictedPeriodTypeDef]],  # (1)
```

1. See [:material-code-braces: RestrictedPeriodTypeDef](./type_defs.md#restrictedperiodtypedef) 
## RestrictedPeriodsTypeDef

```python
# RestrictedPeriodsTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import RestrictedPeriodsTypeDef


def get_value() -> RestrictedPeriodsTypeDef:
    return {
        "restrictedPeriodList": ...,
    }


# RestrictedPeriodsTypeDef definition

class RestrictedPeriodsTypeDef(TypedDict):
    restrictedPeriodList: NotRequired[Sequence[RestrictedPeriodTypeDef]],  # (1)
```

1. See [:material-code-braces: RestrictedPeriodTypeDef](./type_defs.md#restrictedperiodtypedef) 
## SmsChannelSubtypeConfigOutputTypeDef

```python
# SmsChannelSubtypeConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import SmsChannelSubtypeConfigOutputTypeDef


def get_value() -> SmsChannelSubtypeConfigOutputTypeDef:
    return {
        "capacity": ...,
    }


# SmsChannelSubtypeConfigOutputTypeDef definition

class SmsChannelSubtypeConfigOutputTypeDef(TypedDict):
    outboundMode: SmsOutboundModeOutputTypeDef,  # (1)
    defaultOutboundConfig: SmsOutboundConfigTypeDef,  # (2)
    capacity: NotRequired[float],
```

1. See [:material-code-braces: SmsOutboundModeOutputTypeDef](./type_defs.md#smsoutboundmodeoutputtypedef) 
2. See [:material-code-braces: SmsOutboundConfigTypeDef](./type_defs.md#smsoutboundconfigtypedef) 
## SmsChannelSubtypeConfigTypeDef

```python
# SmsChannelSubtypeConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import SmsChannelSubtypeConfigTypeDef


def get_value() -> SmsChannelSubtypeConfigTypeDef:
    return {
        "capacity": ...,
    }


# SmsChannelSubtypeConfigTypeDef definition

class SmsChannelSubtypeConfigTypeDef(TypedDict):
    outboundMode: SmsOutboundModeTypeDef,  # (1)
    defaultOutboundConfig: SmsOutboundConfigTypeDef,  # (2)
    capacity: NotRequired[float],
```

1. See [:material-code-braces: SmsOutboundModeTypeDef](./type_defs.md#smsoutboundmodetypedef) 
2. See [:material-code-braces: SmsOutboundConfigTypeDef](./type_defs.md#smsoutboundconfigtypedef) 
## ChannelSubtypeParametersTypeDef

```python
# ChannelSubtypeParametersTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ChannelSubtypeParametersTypeDef


def get_value() -> ChannelSubtypeParametersTypeDef:
    return {
        "telephony": ...,
    }


# ChannelSubtypeParametersTypeDef definition

class ChannelSubtypeParametersTypeDef(TypedDict):
    telephony: NotRequired[TelephonyChannelSubtypeParametersTypeDef],  # (1)
    sms: NotRequired[SmsChannelSubtypeParametersTypeDef],  # (2)
    email: NotRequired[EmailChannelSubtypeParametersTypeDef],  # (3)
```

1. See [:material-code-braces: TelephonyChannelSubtypeParametersTypeDef](./type_defs.md#telephonychannelsubtypeparameterstypedef) 
2. See [:material-code-braces: SmsChannelSubtypeParametersTypeDef](./type_defs.md#smschannelsubtypeparameterstypedef) 
3. See [:material-code-braces: EmailChannelSubtypeParametersTypeDef](./type_defs.md#emailchannelsubtypeparameterstypedef) 
## ListCampaignsRequestPaginateTypeDef

```python
# ListCampaignsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ListCampaignsRequestPaginateTypeDef


def get_value() -> ListCampaignsRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# ListCampaignsRequestPaginateTypeDef definition

class ListCampaignsRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[CampaignFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CampaignFiltersTypeDef](./type_defs.md#campaignfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCampaignsRequestTypeDef

```python
# ListCampaignsRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ListCampaignsRequestTypeDef


def get_value() -> ListCampaignsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListCampaignsRequestTypeDef definition

class ListCampaignsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filters: NotRequired[CampaignFiltersTypeDef],  # (1)
```

1. See [:material-code-braces: CampaignFiltersTypeDef](./type_defs.md#campaignfilterstypedef) 
## ListCampaignsResponseTypeDef

```python
# ListCampaignsResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ListCampaignsResponseTypeDef


def get_value() -> ListCampaignsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListCampaignsResponseTypeDef definition

class ListCampaignsResponseTypeDef(TypedDict):
    campaignSummaryList: List[CampaignSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CampaignSummaryTypeDef](./type_defs.md#campaignsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CommunicationLimitsConfigOutputTypeDef

```python
# CommunicationLimitsConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CommunicationLimitsConfigOutputTypeDef


def get_value() -> CommunicationLimitsConfigOutputTypeDef:
    return {
        "allChannelSubtypes": ...,
    }


# CommunicationLimitsConfigOutputTypeDef definition

class CommunicationLimitsConfigOutputTypeDef(TypedDict):
    allChannelSubtypes: NotRequired[CommunicationLimitsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CommunicationLimitsOutputTypeDef](./type_defs.md#communicationlimitsoutputtypedef) 
## CommunicationLimitsConfigTypeDef

```python
# CommunicationLimitsConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CommunicationLimitsConfigTypeDef


def get_value() -> CommunicationLimitsConfigTypeDef:
    return {
        "allChannelSubtypes": ...,
    }


# CommunicationLimitsConfigTypeDef definition

class CommunicationLimitsConfigTypeDef(TypedDict):
    allChannelSubtypes: NotRequired[CommunicationLimitsTypeDef],  # (1)
```

1. See [:material-code-braces: CommunicationLimitsTypeDef](./type_defs.md#communicationlimitstypedef) 
## GetConnectInstanceConfigResponseTypeDef

```python
# GetConnectInstanceConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import GetConnectInstanceConfigResponseTypeDef


def get_value() -> GetConnectInstanceConfigResponseTypeDef:
    return {
        "connectInstanceConfig": ...,
    }


# GetConnectInstanceConfigResponseTypeDef definition

class GetConnectInstanceConfigResponseTypeDef(TypedDict):
    connectInstanceConfig: InstanceConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCampaignSourceRequestTypeDef

```python
# UpdateCampaignSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import UpdateCampaignSourceRequestTypeDef


def get_value() -> UpdateCampaignSourceRequestTypeDef:
    return {
        "id": ...,
    }


# UpdateCampaignSourceRequestTypeDef definition

class UpdateCampaignSourceRequestTypeDef(TypedDict):
    id: str,
    source: SourceTypeDef,  # (1)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
## PutConnectInstanceIntegrationRequestTypeDef

```python
# PutConnectInstanceIntegrationRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import PutConnectInstanceIntegrationRequestTypeDef


def get_value() -> PutConnectInstanceIntegrationRequestTypeDef:
    return {
        "connectInstanceId": ...,
    }


# PutConnectInstanceIntegrationRequestTypeDef definition

class PutConnectInstanceIntegrationRequestTypeDef(TypedDict):
    connectInstanceId: str,
    integrationConfig: IntegrationConfigTypeDef,  # (1)
```

1. See [:material-code-braces: IntegrationConfigTypeDef](./type_defs.md#integrationconfigtypedef) 
## DeleteConnectInstanceIntegrationRequestTypeDef

```python
# DeleteConnectInstanceIntegrationRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import DeleteConnectInstanceIntegrationRequestTypeDef


def get_value() -> DeleteConnectInstanceIntegrationRequestTypeDef:
    return {
        "connectInstanceId": ...,
    }


# DeleteConnectInstanceIntegrationRequestTypeDef definition

class DeleteConnectInstanceIntegrationRequestTypeDef(TypedDict):
    connectInstanceId: str,
    integrationIdentifier: IntegrationIdentifierTypeDef,  # (1)
```

1. See [:material-code-braces: IntegrationIdentifierTypeDef](./type_defs.md#integrationidentifiertypedef) 
## ListConnectInstanceIntegrationsResponseTypeDef

```python
# ListConnectInstanceIntegrationsResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ListConnectInstanceIntegrationsResponseTypeDef


def get_value() -> ListConnectInstanceIntegrationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListConnectInstanceIntegrationsResponseTypeDef definition

class ListConnectInstanceIntegrationsResponseTypeDef(TypedDict):
    integrationSummaryList: List[IntegrationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IntegrationSummaryTypeDef](./type_defs.md#integrationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutProfileOutboundRequestBatchRequestTypeDef

```python
# PutProfileOutboundRequestBatchRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import PutProfileOutboundRequestBatchRequestTypeDef


def get_value() -> PutProfileOutboundRequestBatchRequestTypeDef:
    return {
        "id": ...,
    }


# PutProfileOutboundRequestBatchRequestTypeDef definition

class PutProfileOutboundRequestBatchRequestTypeDef(TypedDict):
    id: str,
    profileOutboundRequests: Sequence[ProfileOutboundRequestTypeDef],  # (1)
```

1. See [:material-code-braces: ProfileOutboundRequestTypeDef](./type_defs.md#profileoutboundrequesttypedef) 
## TelephonyChannelSubtypeConfigOutputTypeDef

```python
# TelephonyChannelSubtypeConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import TelephonyChannelSubtypeConfigOutputTypeDef


def get_value() -> TelephonyChannelSubtypeConfigOutputTypeDef:
    return {
        "capacity": ...,
    }


# TelephonyChannelSubtypeConfigOutputTypeDef definition

class TelephonyChannelSubtypeConfigOutputTypeDef(TypedDict):
    outboundMode: TelephonyOutboundModeOutputTypeDef,  # (1)
    defaultOutboundConfig: TelephonyOutboundConfigTypeDef,  # (2)
    capacity: NotRequired[float],
    connectQueueId: NotRequired[str],
```

1. See [:material-code-braces: TelephonyOutboundModeOutputTypeDef](./type_defs.md#telephonyoutboundmodeoutputtypedef) 
2. See [:material-code-braces: TelephonyOutboundConfigTypeDef](./type_defs.md#telephonyoutboundconfigtypedef) 
## TelephonyChannelSubtypeConfigTypeDef

```python
# TelephonyChannelSubtypeConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import TelephonyChannelSubtypeConfigTypeDef


def get_value() -> TelephonyChannelSubtypeConfigTypeDef:
    return {
        "capacity": ...,
    }


# TelephonyChannelSubtypeConfigTypeDef definition

class TelephonyChannelSubtypeConfigTypeDef(TypedDict):
    outboundMode: TelephonyOutboundModeTypeDef,  # (1)
    defaultOutboundConfig: TelephonyOutboundConfigTypeDef,  # (2)
    capacity: NotRequired[float],
    connectQueueId: NotRequired[str],
```

1. See [:material-code-braces: TelephonyOutboundModeTypeDef](./type_defs.md#telephonyoutboundmodetypedef) 
2. See [:material-code-braces: TelephonyOutboundConfigTypeDef](./type_defs.md#telephonyoutboundconfigtypedef) 
## TimeWindowOutputTypeDef

```python
# TimeWindowOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import TimeWindowOutputTypeDef


def get_value() -> TimeWindowOutputTypeDef:
    return {
        "openHours": ...,
    }


# TimeWindowOutputTypeDef definition

class TimeWindowOutputTypeDef(TypedDict):
    openHours: OpenHoursOutputTypeDef,  # (1)
    restrictedPeriods: NotRequired[RestrictedPeriodsOutputTypeDef],  # (2)
```

1. See [:material-code-braces: OpenHoursOutputTypeDef](./type_defs.md#openhoursoutputtypedef) 
2. See [:material-code-braces: RestrictedPeriodsOutputTypeDef](./type_defs.md#restrictedperiodsoutputtypedef) 
## TimeWindowTypeDef

```python
# TimeWindowTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import TimeWindowTypeDef


def get_value() -> TimeWindowTypeDef:
    return {
        "openHours": ...,
    }


# TimeWindowTypeDef definition

class TimeWindowTypeDef(TypedDict):
    openHours: OpenHoursTypeDef,  # (1)
    restrictedPeriods: NotRequired[RestrictedPeriodsTypeDef],  # (2)
```

1. See [:material-code-braces: OpenHoursTypeDef](./type_defs.md#openhourstypedef) 
2. See [:material-code-braces: RestrictedPeriodsTypeDef](./type_defs.md#restrictedperiodstypedef) 
## OutboundRequestTypeDef

```python
# OutboundRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import OutboundRequestTypeDef


def get_value() -> OutboundRequestTypeDef:
    return {
        "clientToken": ...,
    }


# OutboundRequestTypeDef definition

class OutboundRequestTypeDef(TypedDict):
    clientToken: str,
    expirationTime: TimestampTypeDef,
    channelSubtypeParameters: ChannelSubtypeParametersTypeDef,  # (1)
```

1. See [:material-code-braces: ChannelSubtypeParametersTypeDef](./type_defs.md#channelsubtypeparameterstypedef) 
## UpdateCampaignScheduleRequestTypeDef

```python
# UpdateCampaignScheduleRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import UpdateCampaignScheduleRequestTypeDef


def get_value() -> UpdateCampaignScheduleRequestTypeDef:
    return {
        "id": ...,
    }


# UpdateCampaignScheduleRequestTypeDef definition

class UpdateCampaignScheduleRequestTypeDef(TypedDict):
    id: str,
    schedule: ScheduleUnionTypeDef,  # (1)
```

1. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
## ChannelSubtypeConfigOutputTypeDef

```python
# ChannelSubtypeConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ChannelSubtypeConfigOutputTypeDef


def get_value() -> ChannelSubtypeConfigOutputTypeDef:
    return {
        "telephony": ...,
    }


# ChannelSubtypeConfigOutputTypeDef definition

class ChannelSubtypeConfigOutputTypeDef(TypedDict):
    telephony: NotRequired[TelephonyChannelSubtypeConfigOutputTypeDef],  # (1)
    sms: NotRequired[SmsChannelSubtypeConfigOutputTypeDef],  # (2)
    email: NotRequired[EmailChannelSubtypeConfigOutputTypeDef],  # (3)
```

1. See [:material-code-braces: TelephonyChannelSubtypeConfigOutputTypeDef](./type_defs.md#telephonychannelsubtypeconfigoutputtypedef) 
2. See [:material-code-braces: SmsChannelSubtypeConfigOutputTypeDef](./type_defs.md#smschannelsubtypeconfigoutputtypedef) 
3. See [:material-code-braces: EmailChannelSubtypeConfigOutputTypeDef](./type_defs.md#emailchannelsubtypeconfigoutputtypedef) 
## ChannelSubtypeConfigTypeDef

```python
# ChannelSubtypeConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import ChannelSubtypeConfigTypeDef


def get_value() -> ChannelSubtypeConfigTypeDef:
    return {
        "telephony": ...,
    }


# ChannelSubtypeConfigTypeDef definition

class ChannelSubtypeConfigTypeDef(TypedDict):
    telephony: NotRequired[TelephonyChannelSubtypeConfigTypeDef],  # (1)
    sms: NotRequired[SmsChannelSubtypeConfigTypeDef],  # (2)
    email: NotRequired[EmailChannelSubtypeConfigTypeDef],  # (3)
```

1. See [:material-code-braces: TelephonyChannelSubtypeConfigTypeDef](./type_defs.md#telephonychannelsubtypeconfigtypedef) 
2. See [:material-code-braces: SmsChannelSubtypeConfigTypeDef](./type_defs.md#smschannelsubtypeconfigtypedef) 
3. See [:material-code-braces: EmailChannelSubtypeConfigTypeDef](./type_defs.md#emailchannelsubtypeconfigtypedef) 
## CommunicationTimeConfigOutputTypeDef

```python
# CommunicationTimeConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CommunicationTimeConfigOutputTypeDef


def get_value() -> CommunicationTimeConfigOutputTypeDef:
    return {
        "localTimeZoneConfig": ...,
    }


# CommunicationTimeConfigOutputTypeDef definition

class CommunicationTimeConfigOutputTypeDef(TypedDict):
    localTimeZoneConfig: LocalTimeZoneConfigOutputTypeDef,  # (1)
    telephony: NotRequired[TimeWindowOutputTypeDef],  # (2)
    sms: NotRequired[TimeWindowOutputTypeDef],  # (2)
    email: NotRequired[TimeWindowOutputTypeDef],  # (2)
```

1. See [:material-code-braces: LocalTimeZoneConfigOutputTypeDef](./type_defs.md#localtimezoneconfigoutputtypedef) 
2. See [:material-code-braces: TimeWindowOutputTypeDef](./type_defs.md#timewindowoutputtypedef) 
3. See [:material-code-braces: TimeWindowOutputTypeDef](./type_defs.md#timewindowoutputtypedef) 
4. See [:material-code-braces: TimeWindowOutputTypeDef](./type_defs.md#timewindowoutputtypedef) 
## CommunicationTimeConfigTypeDef

```python
# CommunicationTimeConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CommunicationTimeConfigTypeDef


def get_value() -> CommunicationTimeConfigTypeDef:
    return {
        "localTimeZoneConfig": ...,
    }


# CommunicationTimeConfigTypeDef definition

class CommunicationTimeConfigTypeDef(TypedDict):
    localTimeZoneConfig: LocalTimeZoneConfigTypeDef,  # (1)
    telephony: NotRequired[TimeWindowTypeDef],  # (2)
    sms: NotRequired[TimeWindowTypeDef],  # (2)
    email: NotRequired[TimeWindowTypeDef],  # (2)
```

1. See [:material-code-braces: LocalTimeZoneConfigTypeDef](./type_defs.md#localtimezoneconfigtypedef) 
2. See [:material-code-braces: TimeWindowTypeDef](./type_defs.md#timewindowtypedef) 
3. See [:material-code-braces: TimeWindowTypeDef](./type_defs.md#timewindowtypedef) 
4. See [:material-code-braces: TimeWindowTypeDef](./type_defs.md#timewindowtypedef) 
## PutOutboundRequestBatchRequestTypeDef

```python
# PutOutboundRequestBatchRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import PutOutboundRequestBatchRequestTypeDef


def get_value() -> PutOutboundRequestBatchRequestTypeDef:
    return {
        "id": ...,
    }


# PutOutboundRequestBatchRequestTypeDef definition

class PutOutboundRequestBatchRequestTypeDef(TypedDict):
    id: str,
    outboundRequests: Sequence[OutboundRequestTypeDef],  # (1)
```

1. See [:material-code-braces: OutboundRequestTypeDef](./type_defs.md#outboundrequesttypedef) 
## UpdateCampaignCommunicationLimitsRequestTypeDef

```python
# UpdateCampaignCommunicationLimitsRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import UpdateCampaignCommunicationLimitsRequestTypeDef


def get_value() -> UpdateCampaignCommunicationLimitsRequestTypeDef:
    return {
        "id": ...,
    }


# UpdateCampaignCommunicationLimitsRequestTypeDef definition

class UpdateCampaignCommunicationLimitsRequestTypeDef(TypedDict):
    id: str,
    communicationLimitsOverride: CommunicationLimitsConfigUnionTypeDef,  # (1)
```

1. See [:material-code-braces: CommunicationLimitsConfigTypeDef](./type_defs.md#communicationlimitsconfigtypedef) [:material-code-braces: CommunicationLimitsConfigOutputTypeDef](./type_defs.md#communicationlimitsconfigoutputtypedef) 
## CampaignTypeDef

```python
# CampaignTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CampaignTypeDef


def get_value() -> CampaignTypeDef:
    return {
        "id": ...,
    }


# CampaignTypeDef definition

class CampaignTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    connectInstanceId: str,
    channelSubtypeConfig: ChannelSubtypeConfigOutputTypeDef,  # (1)
    source: NotRequired[SourceTypeDef],  # (2)
    connectCampaignFlowArn: NotRequired[str],
    schedule: NotRequired[ScheduleOutputTypeDef],  # (3)
    communicationTimeConfig: NotRequired[CommunicationTimeConfigOutputTypeDef],  # (4)
    communicationLimitsOverride: NotRequired[CommunicationLimitsConfigOutputTypeDef],  # (5)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ChannelSubtypeConfigOutputTypeDef](./type_defs.md#channelsubtypeconfigoutputtypedef) 
2. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
3. See [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
4. See [:material-code-braces: CommunicationTimeConfigOutputTypeDef](./type_defs.md#communicationtimeconfigoutputtypedef) 
5. See [:material-code-braces: CommunicationLimitsConfigOutputTypeDef](./type_defs.md#communicationlimitsconfigoutputtypedef) 
## UpdateCampaignChannelSubtypeConfigRequestTypeDef

```python
# UpdateCampaignChannelSubtypeConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import UpdateCampaignChannelSubtypeConfigRequestTypeDef


def get_value() -> UpdateCampaignChannelSubtypeConfigRequestTypeDef:
    return {
        "id": ...,
    }


# UpdateCampaignChannelSubtypeConfigRequestTypeDef definition

class UpdateCampaignChannelSubtypeConfigRequestTypeDef(TypedDict):
    id: str,
    channelSubtypeConfig: ChannelSubtypeConfigUnionTypeDef,  # (1)
```

1. See [:material-code-braces: ChannelSubtypeConfigTypeDef](./type_defs.md#channelsubtypeconfigtypedef) [:material-code-braces: ChannelSubtypeConfigOutputTypeDef](./type_defs.md#channelsubtypeconfigoutputtypedef) 
## DescribeCampaignResponseTypeDef

```python
# DescribeCampaignResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import DescribeCampaignResponseTypeDef


def get_value() -> DescribeCampaignResponseTypeDef:
    return {
        "campaign": ...,
    }


# DescribeCampaignResponseTypeDef definition

class DescribeCampaignResponseTypeDef(TypedDict):
    campaign: CampaignTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CampaignTypeDef](./type_defs.md#campaigntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCampaignRequestTypeDef

```python
# CreateCampaignRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import CreateCampaignRequestTypeDef


def get_value() -> CreateCampaignRequestTypeDef:
    return {
        "name": ...,
    }


# CreateCampaignRequestTypeDef definition

class CreateCampaignRequestTypeDef(TypedDict):
    name: str,
    connectInstanceId: str,
    channelSubtypeConfig: ChannelSubtypeConfigUnionTypeDef,  # (1)
    source: NotRequired[SourceTypeDef],  # (2)
    connectCampaignFlowArn: NotRequired[str],
    schedule: NotRequired[ScheduleUnionTypeDef],  # (3)
    communicationTimeConfig: NotRequired[CommunicationTimeConfigUnionTypeDef],  # (4)
    communicationLimitsOverride: NotRequired[CommunicationLimitsConfigUnionTypeDef],  # (5)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ChannelSubtypeConfigTypeDef](./type_defs.md#channelsubtypeconfigtypedef) [:material-code-braces: ChannelSubtypeConfigOutputTypeDef](./type_defs.md#channelsubtypeconfigoutputtypedef) 
2. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
3. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
4. See [:material-code-braces: CommunicationTimeConfigTypeDef](./type_defs.md#communicationtimeconfigtypedef) [:material-code-braces: CommunicationTimeConfigOutputTypeDef](./type_defs.md#communicationtimeconfigoutputtypedef) 
5. See [:material-code-braces: CommunicationLimitsConfigTypeDef](./type_defs.md#communicationlimitsconfigtypedef) [:material-code-braces: CommunicationLimitsConfigOutputTypeDef](./type_defs.md#communicationlimitsconfigoutputtypedef) 
## UpdateCampaignCommunicationTimeRequestTypeDef

```python
# UpdateCampaignCommunicationTimeRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcampaignsv2.type_defs import UpdateCampaignCommunicationTimeRequestTypeDef


def get_value() -> UpdateCampaignCommunicationTimeRequestTypeDef:
    return {
        "id": ...,
    }


# UpdateCampaignCommunicationTimeRequestTypeDef definition

class UpdateCampaignCommunicationTimeRequestTypeDef(TypedDict):
    id: str,
    communicationTimeConfig: CommunicationTimeConfigUnionTypeDef,  # (1)
```

1. See [:material-code-braces: CommunicationTimeConfigTypeDef](./type_defs.md#communicationtimeconfigtypedef) [:material-code-braces: CommunicationTimeConfigOutputTypeDef](./type_defs.md#communicationtimeconfigoutputtypedef) 
