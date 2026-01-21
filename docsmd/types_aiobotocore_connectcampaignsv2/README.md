# ConnectCampaignServiceV2 module

> [Index](../README.md) > ConnectCampaignServiceV2


!!! note ""

    Auto-generated documentation for [ConnectCampaignServiceV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaignsv2.html#connectcampaignservicev2)
    type annotations stubs module [types-aiobotocore-connectcampaignsv2](https://pypi.org/project/types-aiobotocore-connectcampaignsv2/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ConnectCampaignServiceV2` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ConnectCampaignServiceV2` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[connectcampaignsv2]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[connectcampaignsv2]'

# standalone installation
python -m pip install types-aiobotocore-connectcampaignsv2
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-connectcampaignsv2
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ConnectCampaignServiceV2Client

Type annotations and code completion for  `#!python session.create_client("connectcampaignsv2")` as [ConnectCampaignServiceV2Client](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaignsv2.html#ConnectCampaignServiceV2.Client)

```python
# ConnectCampaignServiceV2Client usage example

from aiobotocore.session import get_session

from types_aiobotocore_connectcampaignsv2.client import ConnectCampaignServiceV2Client


session = get_session()
async with session.create_client("connectcampaignsv2") as client:
    client: ConnectCampaignServiceV2Client
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("connectcampaignsv2").get_paginator("...")`.

```python
# ListCampaignsPaginator usage example

from types_aiobotocore_connectcampaignsv2.paginator import ListCampaignsPaginator

def get_list_campaigns_paginator() -> ListCampaignsPaginator:
    return client.get_paginator("list_campaigns"))
```

- [ListCampaignsPaginator](./paginators.md#listcampaignspaginator)
- [ListConnectInstanceIntegrationsPaginator](./paginators.md#listconnectinstanceintegrationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AgentActionType usage example

from types_aiobotocore_connectcampaignsv2.literals import AgentActionType

def get_value() -> AgentActionType:
    return "DISCARD"
```

- [AgentActionType](./literals.md#agentactiontype)
- [CampaignDeletionPolicyType](./literals.md#campaigndeletionpolicytype)
- [CampaignStateType](./literals.md#campaignstatetype)
- [ChannelSubtypeType](./literals.md#channelsubtypetype)
- [CommunicationLimitTimeUnitType](./literals.md#communicationlimittimeunittype)
- [CommunicationLimitsConfigTypeType](./literals.md#communicationlimitsconfigtypetype)
- [CommunicationTimeConfigTypeType](./literals.md#communicationtimeconfigtypetype)
- [DayOfWeekType](./literals.md#dayofweektype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [EventTypeType](./literals.md#eventtypetype)
- [ExternalCampaignTypeType](./literals.md#externalcampaigntypetype)
- [FailureCodeType](./literals.md#failurecodetype)
- [GetCampaignStateBatchFailureCodeType](./literals.md#getcampaignstatebatchfailurecodetype)
- [InstanceIdFilterOperatorType](./literals.md#instanceidfilteroperatortype)
- [InstanceLimitsHandlingType](./literals.md#instancelimitshandlingtype)
- [InstanceOnboardingJobFailureCodeType](./literals.md#instanceonboardingjobfailurecodetype)
- [InstanceOnboardingJobStatusCodeType](./literals.md#instanceonboardingjobstatuscodetype)
- [ListCampaignsPaginatorName](./literals.md#listcampaignspaginatorname)
- [ListConnectInstanceIntegrationsPaginatorName](./literals.md#listconnectinstanceintegrationspaginatorname)
- [LocalTimeZoneDetectionTypeType](./literals.md#localtimezonedetectiontypetype)
- [ProfileOutboundRequestFailureCodeType](./literals.md#profileoutboundrequestfailurecodetype)
- [ConnectCampaignServiceV2ServiceName](./literals.md#connectcampaignservicev2servicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AnswerMachineDetectionConfigTypeDef](./type_defs.md#answermachinedetectionconfigtypedef)
- [InstanceIdFilterTypeDef](./type_defs.md#instanceidfiltertypedef)
- [ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef)
- [EmailChannelSubtypeParametersTypeDef](./type_defs.md#emailchannelsubtypeparameterstypedef)
- [SmsChannelSubtypeParametersTypeDef](./type_defs.md#smschannelsubtypeparameterstypedef)
- [WhatsAppChannelSubtypeParametersTypeDef](./type_defs.md#whatsappchannelsubtypeparameterstypedef)
- [CommunicationLimitTypeDef](./type_defs.md#communicationlimittypedef)
- [LocalTimeZoneConfigOutputTypeDef](./type_defs.md#localtimezoneconfigoutputtypedef)
- [LocalTimeZoneConfigTypeDef](./type_defs.md#localtimezoneconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CustomerProfilesIntegrationConfigTypeDef](./type_defs.md#customerprofilesintegrationconfigtypedef)
- [CustomerProfilesIntegrationIdentifierTypeDef](./type_defs.md#customerprofilesintegrationidentifiertypedef)
- [CustomerProfilesIntegrationSummaryTypeDef](./type_defs.md#customerprofilesintegrationsummarytypedef)
- [DeleteCampaignChannelSubtypeConfigRequestTypeDef](./type_defs.md#deletecampaignchannelsubtypeconfigrequesttypedef)
- [DeleteCampaignCommunicationLimitsRequestTypeDef](./type_defs.md#deletecampaigncommunicationlimitsrequesttypedef)
- [DeleteCampaignCommunicationTimeRequestTypeDef](./type_defs.md#deletecampaigncommunicationtimerequesttypedef)
- [DeleteCampaignRequestTypeDef](./type_defs.md#deletecampaignrequesttypedef)
- [DeleteConnectInstanceConfigRequestTypeDef](./type_defs.md#deleteconnectinstanceconfigrequesttypedef)
- [DeleteInstanceOnboardingJobRequestTypeDef](./type_defs.md#deleteinstanceonboardingjobrequesttypedef)
- [DescribeCampaignRequestTypeDef](./type_defs.md#describecampaignrequesttypedef)
- [EmailOutboundConfigTypeDef](./type_defs.md#emailoutboundconfigtypedef)
- [EmailOutboundModeOutputTypeDef](./type_defs.md#emailoutboundmodeoutputtypedef)
- [EmailOutboundModeTypeDef](./type_defs.md#emailoutboundmodetypedef)
- [EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef)
- [EventTriggerTypeDef](./type_defs.md#eventtriggertypedef)
- [FailedCampaignStateResponseTypeDef](./type_defs.md#failedcampaignstateresponsetypedef)
- [FailedProfileOutboundRequestTypeDef](./type_defs.md#failedprofileoutboundrequesttypedef)
- [FailedRequestTypeDef](./type_defs.md#failedrequesttypedef)
- [GetCampaignStateBatchRequestTypeDef](./type_defs.md#getcampaignstatebatchrequesttypedef)
- [SuccessfulCampaignStateResponseTypeDef](./type_defs.md#successfulcampaignstateresponsetypedef)
- [GetCampaignStateRequestTypeDef](./type_defs.md#getcampaignstaterequesttypedef)
- [GetConnectInstanceConfigRequestTypeDef](./type_defs.md#getconnectinstanceconfigrequesttypedef)
- [GetInstanceCommunicationLimitsRequestTypeDef](./type_defs.md#getinstancecommunicationlimitsrequesttypedef)
- [GetInstanceOnboardingJobStatusRequestTypeDef](./type_defs.md#getinstanceonboardingjobstatusrequesttypedef)
- [InstanceOnboardingJobStatusTypeDef](./type_defs.md#instanceonboardingjobstatustypedef)
- [LambdaIntegrationConfigTypeDef](./type_defs.md#lambdaintegrationconfigtypedef)
- [QConnectIntegrationConfigTypeDef](./type_defs.md#qconnectintegrationconfigtypedef)
- [LambdaIntegrationIdentifierTypeDef](./type_defs.md#lambdaintegrationidentifiertypedef)
- [QConnectIntegrationIdentifierTypeDef](./type_defs.md#qconnectintegrationidentifiertypedef)
- [LambdaIntegrationSummaryTypeDef](./type_defs.md#lambdaintegrationsummarytypedef)
- [QConnectIntegrationSummaryTypeDef](./type_defs.md#qconnectintegrationsummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListConnectInstanceIntegrationsRequestTypeDef](./type_defs.md#listconnectinstanceintegrationsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [TimeRangeTypeDef](./type_defs.md#timerangetypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [PauseCampaignRequestTypeDef](./type_defs.md#pausecampaignrequesttypedef)
- [PredictiveConfigTypeDef](./type_defs.md#predictiveconfigtypedef)
- [TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef)
- [ProgressiveConfigTypeDef](./type_defs.md#progressiveconfigtypedef)
- [SuccessfulRequestTypeDef](./type_defs.md#successfulrequesttypedef)
- [SuccessfulProfileOutboundRequestTypeDef](./type_defs.md#successfulprofileoutboundrequesttypedef)
- [RestrictedPeriodTypeDef](./type_defs.md#restrictedperiodtypedef)
- [ResumeCampaignRequestTypeDef](./type_defs.md#resumecampaignrequesttypedef)
- [SmsOutboundConfigTypeDef](./type_defs.md#smsoutboundconfigtypedef)
- [SmsOutboundModeOutputTypeDef](./type_defs.md#smsoutboundmodeoutputtypedef)
- [SmsOutboundModeTypeDef](./type_defs.md#smsoutboundmodetypedef)
- [StartCampaignRequestTypeDef](./type_defs.md#startcampaignrequesttypedef)
- [StopCampaignRequestTypeDef](./type_defs.md#stopcampaignrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateCampaignFlowAssociationRequestTypeDef](./type_defs.md#updatecampaignflowassociationrequesttypedef)
- [UpdateCampaignNameRequestTypeDef](./type_defs.md#updatecampaignnamerequesttypedef)
- [WhatsAppOutboundConfigTypeDef](./type_defs.md#whatsappoutboundconfigtypedef)
- [WhatsAppOutboundModeOutputTypeDef](./type_defs.md#whatsappoutboundmodeoutputtypedef)
- [WhatsAppOutboundModeTypeDef](./type_defs.md#whatsappoutboundmodetypedef)
- [TelephonyChannelSubtypeParametersTypeDef](./type_defs.md#telephonychannelsubtypeparameterstypedef)
- [TelephonyOutboundConfigTypeDef](./type_defs.md#telephonyoutboundconfigtypedef)
- [CampaignFiltersTypeDef](./type_defs.md#campaignfilterstypedef)
- [CampaignSummaryTypeDef](./type_defs.md#campaignsummarytypedef)
- [CommunicationLimitsOutputTypeDef](./type_defs.md#communicationlimitsoutputtypedef)
- [CommunicationLimitsTypeDef](./type_defs.md#communicationlimitstypedef)
- [CreateCampaignResponseTypeDef](./type_defs.md#createcampaignresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetCampaignStateResponseTypeDef](./type_defs.md#getcampaignstateresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [EmailChannelSubtypeConfigOutputTypeDef](./type_defs.md#emailchannelsubtypeconfigoutputtypedef)
- [EmailChannelSubtypeConfigTypeDef](./type_defs.md#emailchannelsubtypeconfigtypedef)
- [InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef)
- [StartInstanceOnboardingJobRequestTypeDef](./type_defs.md#startinstanceonboardingjobrequesttypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [GetCampaignStateBatchResponseTypeDef](./type_defs.md#getcampaignstatebatchresponsetypedef)
- [GetInstanceOnboardingJobStatusResponseTypeDef](./type_defs.md#getinstanceonboardingjobstatusresponsetypedef)
- [StartInstanceOnboardingJobResponseTypeDef](./type_defs.md#startinstanceonboardingjobresponsetypedef)
- [IntegrationConfigTypeDef](./type_defs.md#integrationconfigtypedef)
- [IntegrationIdentifierTypeDef](./type_defs.md#integrationidentifiertypedef)
- [IntegrationSummaryTypeDef](./type_defs.md#integrationsummarytypedef)
- [ListConnectInstanceIntegrationsRequestPaginateTypeDef](./type_defs.md#listconnectinstanceintegrationsrequestpaginatetypedef)
- [OpenHoursOutputTypeDef](./type_defs.md#openhoursoutputtypedef)
- [OpenHoursTypeDef](./type_defs.md#openhourstypedef)
- [ProfileOutboundRequestTypeDef](./type_defs.md#profileoutboundrequesttypedef)
- [ScheduleTypeDef](./type_defs.md#scheduletypedef)
- [PreviewConfigOutputTypeDef](./type_defs.md#previewconfigoutputtypedef)
- [PreviewConfigTypeDef](./type_defs.md#previewconfigtypedef)
- [PutOutboundRequestBatchResponseTypeDef](./type_defs.md#putoutboundrequestbatchresponsetypedef)
- [PutProfileOutboundRequestBatchResponseTypeDef](./type_defs.md#putprofileoutboundrequestbatchresponsetypedef)
- [RestrictedPeriodsOutputTypeDef](./type_defs.md#restrictedperiodsoutputtypedef)
- [RestrictedPeriodsTypeDef](./type_defs.md#restrictedperiodstypedef)
- [SmsChannelSubtypeConfigOutputTypeDef](./type_defs.md#smschannelsubtypeconfigoutputtypedef)
- [SmsChannelSubtypeConfigTypeDef](./type_defs.md#smschannelsubtypeconfigtypedef)
- [WhatsAppChannelSubtypeConfigOutputTypeDef](./type_defs.md#whatsappchannelsubtypeconfigoutputtypedef)
- [WhatsAppChannelSubtypeConfigTypeDef](./type_defs.md#whatsappchannelsubtypeconfigtypedef)
- [ChannelSubtypeParametersTypeDef](./type_defs.md#channelsubtypeparameterstypedef)
- [ListCampaignsRequestPaginateTypeDef](./type_defs.md#listcampaignsrequestpaginatetypedef)
- [ListCampaignsRequestTypeDef](./type_defs.md#listcampaignsrequesttypedef)
- [ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef)
- [CommunicationLimitsConfigOutputTypeDef](./type_defs.md#communicationlimitsconfigoutputtypedef)
- [InstanceCommunicationLimitsConfigOutputTypeDef](./type_defs.md#instancecommunicationlimitsconfigoutputtypedef)
- [CommunicationLimitsConfigTypeDef](./type_defs.md#communicationlimitsconfigtypedef)
- [InstanceCommunicationLimitsConfigTypeDef](./type_defs.md#instancecommunicationlimitsconfigtypedef)
- [GetConnectInstanceConfigResponseTypeDef](./type_defs.md#getconnectinstanceconfigresponsetypedef)
- [UpdateCampaignSourceRequestTypeDef](./type_defs.md#updatecampaignsourcerequesttypedef)
- [PutConnectInstanceIntegrationRequestTypeDef](./type_defs.md#putconnectinstanceintegrationrequesttypedef)
- [DeleteConnectInstanceIntegrationRequestTypeDef](./type_defs.md#deleteconnectinstanceintegrationrequesttypedef)
- [ListConnectInstanceIntegrationsResponseTypeDef](./type_defs.md#listconnectinstanceintegrationsresponsetypedef)
- [PutProfileOutboundRequestBatchRequestTypeDef](./type_defs.md#putprofileoutboundrequestbatchrequesttypedef)
- [ScheduleUnionTypeDef](./type_defs.md#scheduleuniontypedef)
- [TelephonyOutboundModeOutputTypeDef](./type_defs.md#telephonyoutboundmodeoutputtypedef)
- [TelephonyOutboundModeTypeDef](./type_defs.md#telephonyoutboundmodetypedef)
- [TimeWindowOutputTypeDef](./type_defs.md#timewindowoutputtypedef)
- [TimeWindowTypeDef](./type_defs.md#timewindowtypedef)
- [OutboundRequestTypeDef](./type_defs.md#outboundrequesttypedef)
- [GetInstanceCommunicationLimitsResponseTypeDef](./type_defs.md#getinstancecommunicationlimitsresponsetypedef)
- [CommunicationLimitsConfigUnionTypeDef](./type_defs.md#communicationlimitsconfiguniontypedef)
- [InstanceCommunicationLimitsConfigUnionTypeDef](./type_defs.md#instancecommunicationlimitsconfiguniontypedef)
- [UpdateCampaignScheduleRequestTypeDef](./type_defs.md#updatecampaignschedulerequesttypedef)
- [TelephonyChannelSubtypeConfigOutputTypeDef](./type_defs.md#telephonychannelsubtypeconfigoutputtypedef)
- [TelephonyChannelSubtypeConfigTypeDef](./type_defs.md#telephonychannelsubtypeconfigtypedef)
- [CommunicationTimeConfigOutputTypeDef](./type_defs.md#communicationtimeconfigoutputtypedef)
- [CommunicationTimeConfigTypeDef](./type_defs.md#communicationtimeconfigtypedef)
- [PutOutboundRequestBatchRequestTypeDef](./type_defs.md#putoutboundrequestbatchrequesttypedef)
- [UpdateCampaignCommunicationLimitsRequestTypeDef](./type_defs.md#updatecampaigncommunicationlimitsrequesttypedef)
- [PutInstanceCommunicationLimitsRequestTypeDef](./type_defs.md#putinstancecommunicationlimitsrequesttypedef)
- [ChannelSubtypeConfigOutputTypeDef](./type_defs.md#channelsubtypeconfigoutputtypedef)
- [ChannelSubtypeConfigTypeDef](./type_defs.md#channelsubtypeconfigtypedef)
- [CommunicationTimeConfigUnionTypeDef](./type_defs.md#communicationtimeconfiguniontypedef)
- [CampaignTypeDef](./type_defs.md#campaigntypedef)
- [ChannelSubtypeConfigUnionTypeDef](./type_defs.md#channelsubtypeconfiguniontypedef)
- [UpdateCampaignCommunicationTimeRequestTypeDef](./type_defs.md#updatecampaigncommunicationtimerequesttypedef)
- [DescribeCampaignResponseTypeDef](./type_defs.md#describecampaignresponsetypedef)
- [CreateCampaignRequestTypeDef](./type_defs.md#createcampaignrequesttypedef)
- [UpdateCampaignChannelSubtypeConfigRequestTypeDef](./type_defs.md#updatecampaignchannelsubtypeconfigrequesttypedef)

