# ConnectCampaignServiceV2 module

> [Index](../README.md) > ConnectCampaignServiceV2


!!! note ""

    Auto-generated documentation for [ConnectCampaignServiceV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaignsv2.html#connectcampaignservicev2)
    type annotations stubs module [types-aiobotocore-connectcampaignsv2](https://pypi.org/project/types-aiobotocore-connectcampaignsv2/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
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
# CampaignDeletionPolicyType usage example

from types_aiobotocore_connectcampaignsv2.literals import CampaignDeletionPolicyType

def get_value() -> CampaignDeletionPolicyType:
    return "DELETE_ALL"
```

- [CampaignDeletionPolicyType](./literals.md#campaigndeletionpolicytype)
- [CampaignStateType](./literals.md#campaignstatetype)
- [ChannelSubtypeType](./literals.md#channelsubtypetype)
- [CommunicationLimitTimeUnitType](./literals.md#communicationlimittimeunittype)
- [CommunicationLimitsConfigTypeType](./literals.md#communicationlimitsconfigtypetype)
- [CommunicationTimeConfigTypeType](./literals.md#communicationtimeconfigtypetype)
- [DayOfWeekType](./literals.md#dayofweektype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [EventTypeType](./literals.md#eventtypetype)
- [FailureCodeType](./literals.md#failurecodetype)
- [GetCampaignStateBatchFailureCodeType](./literals.md#getcampaignstatebatchfailurecodetype)
- [InstanceIdFilterOperatorType](./literals.md#instanceidfilteroperatortype)
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
- [CommunicationLimitTypeDef](./type_defs.md#communicationlimittypedef)
- [LocalTimeZoneConfigOutputTypeDef](./type_defs.md#localtimezoneconfigoutputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CustomerProfilesIntegrationConfigTypeDef](./type_defs.md#customerprofilesintegrationconfigtypedef)
- [CustomerProfilesIntegrationIdentifierTypeDef](./type_defs.md#customerprofilesintegrationidentifiertypedef)
- [CustomerProfilesIntegrationSummaryTypeDef](./type_defs.md#customerprofilesintegrationsummarytypedef)
- [DeleteCampaignChannelSubtypeConfigRequestRequestTypeDef](./type_defs.md#deletecampaignchannelsubtypeconfigrequestrequesttypedef)
- [DeleteCampaignCommunicationLimitsRequestRequestTypeDef](./type_defs.md#deletecampaigncommunicationlimitsrequestrequesttypedef)
- [DeleteCampaignCommunicationTimeRequestRequestTypeDef](./type_defs.md#deletecampaigncommunicationtimerequestrequesttypedef)
- [DeleteCampaignRequestRequestTypeDef](./type_defs.md#deletecampaignrequestrequesttypedef)
- [DeleteConnectInstanceConfigRequestRequestTypeDef](./type_defs.md#deleteconnectinstanceconfigrequestrequesttypedef)
- [DeleteInstanceOnboardingJobRequestRequestTypeDef](./type_defs.md#deleteinstanceonboardingjobrequestrequesttypedef)
- [DescribeCampaignRequestRequestTypeDef](./type_defs.md#describecampaignrequestrequesttypedef)
- [EmailOutboundConfigTypeDef](./type_defs.md#emailoutboundconfigtypedef)
- [EmailOutboundModeOutputTypeDef](./type_defs.md#emailoutboundmodeoutputtypedef)
- [EmailOutboundModeTypeDef](./type_defs.md#emailoutboundmodetypedef)
- [EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef)
- [EventTriggerTypeDef](./type_defs.md#eventtriggertypedef)
- [FailedCampaignStateResponseTypeDef](./type_defs.md#failedcampaignstateresponsetypedef)
- [FailedProfileOutboundRequestTypeDef](./type_defs.md#failedprofileoutboundrequesttypedef)
- [FailedRequestTypeDef](./type_defs.md#failedrequesttypedef)
- [GetCampaignStateBatchRequestRequestTypeDef](./type_defs.md#getcampaignstatebatchrequestrequesttypedef)
- [SuccessfulCampaignStateResponseTypeDef](./type_defs.md#successfulcampaignstateresponsetypedef)
- [GetCampaignStateRequestRequestTypeDef](./type_defs.md#getcampaignstaterequestrequesttypedef)
- [GetConnectInstanceConfigRequestRequestTypeDef](./type_defs.md#getconnectinstanceconfigrequestrequesttypedef)
- [GetInstanceOnboardingJobStatusRequestRequestTypeDef](./type_defs.md#getinstanceonboardingjobstatusrequestrequesttypedef)
- [InstanceOnboardingJobStatusTypeDef](./type_defs.md#instanceonboardingjobstatustypedef)
- [QConnectIntegrationConfigTypeDef](./type_defs.md#qconnectintegrationconfigtypedef)
- [QConnectIntegrationIdentifierTypeDef](./type_defs.md#qconnectintegrationidentifiertypedef)
- [QConnectIntegrationSummaryTypeDef](./type_defs.md#qconnectintegrationsummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListConnectInstanceIntegrationsRequestRequestTypeDef](./type_defs.md#listconnectinstanceintegrationsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [LocalTimeZoneConfigTypeDef](./type_defs.md#localtimezoneconfigtypedef)
- [TimeRangeTypeDef](./type_defs.md#timerangetypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [PauseCampaignRequestRequestTypeDef](./type_defs.md#pausecampaignrequestrequesttypedef)
- [PredictiveConfigTypeDef](./type_defs.md#predictiveconfigtypedef)
- [ProgressiveConfigTypeDef](./type_defs.md#progressiveconfigtypedef)
- [SuccessfulRequestTypeDef](./type_defs.md#successfulrequesttypedef)
- [SuccessfulProfileOutboundRequestTypeDef](./type_defs.md#successfulprofileoutboundrequesttypedef)
- [RestrictedPeriodTypeDef](./type_defs.md#restrictedperiodtypedef)
- [ResumeCampaignRequestRequestTypeDef](./type_defs.md#resumecampaignrequestrequesttypedef)
- [SmsOutboundConfigTypeDef](./type_defs.md#smsoutboundconfigtypedef)
- [SmsOutboundModeOutputTypeDef](./type_defs.md#smsoutboundmodeoutputtypedef)
- [SmsOutboundModeTypeDef](./type_defs.md#smsoutboundmodetypedef)
- [StartCampaignRequestRequestTypeDef](./type_defs.md#startcampaignrequestrequesttypedef)
- [StopCampaignRequestRequestTypeDef](./type_defs.md#stopcampaignrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateCampaignFlowAssociationRequestRequestTypeDef](./type_defs.md#updatecampaignflowassociationrequestrequesttypedef)
- [UpdateCampaignNameRequestRequestTypeDef](./type_defs.md#updatecampaignnamerequestrequesttypedef)
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
- [EmailOutboundModeUnionTypeDef](./type_defs.md#emailoutboundmodeuniontypedef)
- [InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef)
- [StartInstanceOnboardingJobRequestRequestTypeDef](./type_defs.md#startinstanceonboardingjobrequestrequesttypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [GetCampaignStateBatchResponseTypeDef](./type_defs.md#getcampaignstatebatchresponsetypedef)
- [GetInstanceOnboardingJobStatusResponseTypeDef](./type_defs.md#getinstanceonboardingjobstatusresponsetypedef)
- [StartInstanceOnboardingJobResponseTypeDef](./type_defs.md#startinstanceonboardingjobresponsetypedef)
- [IntegrationConfigTypeDef](./type_defs.md#integrationconfigtypedef)
- [IntegrationIdentifierTypeDef](./type_defs.md#integrationidentifiertypedef)
- [IntegrationSummaryTypeDef](./type_defs.md#integrationsummarytypedef)
- [ListConnectInstanceIntegrationsRequestPaginateTypeDef](./type_defs.md#listconnectinstanceintegrationsrequestpaginatetypedef)
- [LocalTimeZoneConfigUnionTypeDef](./type_defs.md#localtimezoneconfiguniontypedef)
- [OpenHoursOutputTypeDef](./type_defs.md#openhoursoutputtypedef)
- [OpenHoursTypeDef](./type_defs.md#openhourstypedef)
- [ProfileOutboundRequestTypeDef](./type_defs.md#profileoutboundrequesttypedef)
- [ScheduleTypeDef](./type_defs.md#scheduletypedef)
- [TelephonyOutboundModeOutputTypeDef](./type_defs.md#telephonyoutboundmodeoutputtypedef)
- [TelephonyOutboundModeTypeDef](./type_defs.md#telephonyoutboundmodetypedef)
- [PutOutboundRequestBatchResponseTypeDef](./type_defs.md#putoutboundrequestbatchresponsetypedef)
- [PutProfileOutboundRequestBatchResponseTypeDef](./type_defs.md#putprofileoutboundrequestbatchresponsetypedef)
- [RestrictedPeriodsOutputTypeDef](./type_defs.md#restrictedperiodsoutputtypedef)
- [RestrictedPeriodsTypeDef](./type_defs.md#restrictedperiodstypedef)
- [SmsChannelSubtypeConfigOutputTypeDef](./type_defs.md#smschannelsubtypeconfigoutputtypedef)
- [SmsOutboundModeUnionTypeDef](./type_defs.md#smsoutboundmodeuniontypedef)
- [ChannelSubtypeParametersTypeDef](./type_defs.md#channelsubtypeparameterstypedef)
- [ListCampaignsRequestPaginateTypeDef](./type_defs.md#listcampaignsrequestpaginatetypedef)
- [ListCampaignsRequestRequestTypeDef](./type_defs.md#listcampaignsrequestrequesttypedef)
- [ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef)
- [CommunicationLimitsConfigOutputTypeDef](./type_defs.md#communicationlimitsconfigoutputtypedef)
- [CommunicationLimitsUnionTypeDef](./type_defs.md#communicationlimitsuniontypedef)
- [EmailChannelSubtypeConfigTypeDef](./type_defs.md#emailchannelsubtypeconfigtypedef)
- [GetConnectInstanceConfigResponseTypeDef](./type_defs.md#getconnectinstanceconfigresponsetypedef)
- [UpdateCampaignSourceRequestRequestTypeDef](./type_defs.md#updatecampaignsourcerequestrequesttypedef)
- [PutConnectInstanceIntegrationRequestRequestTypeDef](./type_defs.md#putconnectinstanceintegrationrequestrequesttypedef)
- [DeleteConnectInstanceIntegrationRequestRequestTypeDef](./type_defs.md#deleteconnectinstanceintegrationrequestrequesttypedef)
- [ListConnectInstanceIntegrationsResponseTypeDef](./type_defs.md#listconnectinstanceintegrationsresponsetypedef)
- [OpenHoursUnionTypeDef](./type_defs.md#openhoursuniontypedef)
- [PutProfileOutboundRequestBatchRequestRequestTypeDef](./type_defs.md#putprofileoutboundrequestbatchrequestrequesttypedef)
- [UpdateCampaignScheduleRequestRequestTypeDef](./type_defs.md#updatecampaignschedulerequestrequesttypedef)
- [TelephonyChannelSubtypeConfigOutputTypeDef](./type_defs.md#telephonychannelsubtypeconfigoutputtypedef)
- [TelephonyOutboundModeUnionTypeDef](./type_defs.md#telephonyoutboundmodeuniontypedef)
- [TimeWindowOutputTypeDef](./type_defs.md#timewindowoutputtypedef)
- [RestrictedPeriodsUnionTypeDef](./type_defs.md#restrictedperiodsuniontypedef)
- [SmsChannelSubtypeConfigTypeDef](./type_defs.md#smschannelsubtypeconfigtypedef)
- [OutboundRequestTypeDef](./type_defs.md#outboundrequesttypedef)
- [CommunicationLimitsConfigTypeDef](./type_defs.md#communicationlimitsconfigtypedef)
- [EmailChannelSubtypeConfigUnionTypeDef](./type_defs.md#emailchannelsubtypeconfiguniontypedef)
- [ChannelSubtypeConfigOutputTypeDef](./type_defs.md#channelsubtypeconfigoutputtypedef)
- [TelephonyChannelSubtypeConfigTypeDef](./type_defs.md#telephonychannelsubtypeconfigtypedef)
- [CommunicationTimeConfigOutputTypeDef](./type_defs.md#communicationtimeconfigoutputtypedef)
- [TimeWindowTypeDef](./type_defs.md#timewindowtypedef)
- [SmsChannelSubtypeConfigUnionTypeDef](./type_defs.md#smschannelsubtypeconfiguniontypedef)
- [PutOutboundRequestBatchRequestRequestTypeDef](./type_defs.md#putoutboundrequestbatchrequestrequesttypedef)
- [UpdateCampaignCommunicationLimitsRequestRequestTypeDef](./type_defs.md#updatecampaigncommunicationlimitsrequestrequesttypedef)
- [TelephonyChannelSubtypeConfigUnionTypeDef](./type_defs.md#telephonychannelsubtypeconfiguniontypedef)
- [CampaignTypeDef](./type_defs.md#campaigntypedef)
- [TimeWindowUnionTypeDef](./type_defs.md#timewindowuniontypedef)
- [ChannelSubtypeConfigTypeDef](./type_defs.md#channelsubtypeconfigtypedef)
- [DescribeCampaignResponseTypeDef](./type_defs.md#describecampaignresponsetypedef)
- [CommunicationTimeConfigTypeDef](./type_defs.md#communicationtimeconfigtypedef)
- [UpdateCampaignChannelSubtypeConfigRequestRequestTypeDef](./type_defs.md#updatecampaignchannelsubtypeconfigrequestrequesttypedef)
- [CreateCampaignRequestRequestTypeDef](./type_defs.md#createcampaignrequestrequesttypedef)
- [UpdateCampaignCommunicationTimeRequestRequestTypeDef](./type_defs.md#updatecampaigncommunicationtimerequestrequesttypedef)

