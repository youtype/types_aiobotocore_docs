<a id="pinpointclient-for-aiobotocore-pinpoint-module"></a>

# PinpointClient for aiobotocore Pinpoint module

> [Index](..) > [Pinpoint](.) > PinpointClient

Auto-generated documentation for
[Pinpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
type annotations stubs module
[types-aiobotocore-pinpoint](https://pypi.org/project/types-aiobotocore-pinpoint/).

- [PinpointClient for aiobotocore Pinpoint module](#pinpointclient-for-aiobotocore-pinpoint-module)
  - [PinpointClient](#pinpointclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_app](#create_app)
    - [create_campaign](#create_campaign)
    - [create_email_template](#create_email_template)
    - [create_export_job](#create_export_job)
    - [create_import_job](#create_import_job)
    - [create_in_app_template](#create_in_app_template)
    - [create_journey](#create_journey)
    - [create_push_template](#create_push_template)
    - [create_recommender_configuration](#create_recommender_configuration)
    - [create_segment](#create_segment)
    - [create_sms_template](#create_sms_template)
    - [create_voice_template](#create_voice_template)
    - [delete_adm_channel](#delete_adm_channel)
    - [delete_apns_channel](#delete_apns_channel)
    - [delete_apns_sandbox_channel](#delete_apns_sandbox_channel)
    - [delete_apns_voip_channel](#delete_apns_voip_channel)
    - [delete_apns_voip_sandbox_channel](#delete_apns_voip_sandbox_channel)
    - [delete_app](#delete_app)
    - [delete_baidu_channel](#delete_baidu_channel)
    - [delete_campaign](#delete_campaign)
    - [delete_email_channel](#delete_email_channel)
    - [delete_email_template](#delete_email_template)
    - [delete_endpoint](#delete_endpoint)
    - [delete_event_stream](#delete_event_stream)
    - [delete_gcm_channel](#delete_gcm_channel)
    - [delete_in_app_template](#delete_in_app_template)
    - [delete_journey](#delete_journey)
    - [delete_push_template](#delete_push_template)
    - [delete_recommender_configuration](#delete_recommender_configuration)
    - [delete_segment](#delete_segment)
    - [delete_sms_channel](#delete_sms_channel)
    - [delete_sms_template](#delete_sms_template)
    - [delete_user_endpoints](#delete_user_endpoints)
    - [delete_voice_channel](#delete_voice_channel)
    - [delete_voice_template](#delete_voice_template)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_adm_channel](#get_adm_channel)
    - [get_apns_channel](#get_apns_channel)
    - [get_apns_sandbox_channel](#get_apns_sandbox_channel)
    - [get_apns_voip_channel](#get_apns_voip_channel)
    - [get_apns_voip_sandbox_channel](#get_apns_voip_sandbox_channel)
    - [get_app](#get_app)
    - [get_application_date_range_kpi](#get_application_date_range_kpi)
    - [get_application_settings](#get_application_settings)
    - [get_apps](#get_apps)
    - [get_baidu_channel](#get_baidu_channel)
    - [get_campaign](#get_campaign)
    - [get_campaign_activities](#get_campaign_activities)
    - [get_campaign_date_range_kpi](#get_campaign_date_range_kpi)
    - [get_campaign_version](#get_campaign_version)
    - [get_campaign_versions](#get_campaign_versions)
    - [get_campaigns](#get_campaigns)
    - [get_channels](#get_channels)
    - [get_email_channel](#get_email_channel)
    - [get_email_template](#get_email_template)
    - [get_endpoint](#get_endpoint)
    - [get_event_stream](#get_event_stream)
    - [get_export_job](#get_export_job)
    - [get_export_jobs](#get_export_jobs)
    - [get_gcm_channel](#get_gcm_channel)
    - [get_import_job](#get_import_job)
    - [get_import_jobs](#get_import_jobs)
    - [get_in_app_messages](#get_in_app_messages)
    - [get_in_app_template](#get_in_app_template)
    - [get_journey](#get_journey)
    - [get_journey_date_range_kpi](#get_journey_date_range_kpi)
    - [get_journey_execution_activity_metrics](#get_journey_execution_activity_metrics)
    - [get_journey_execution_metrics](#get_journey_execution_metrics)
    - [get_push_template](#get_push_template)
    - [get_recommender_configuration](#get_recommender_configuration)
    - [get_recommender_configurations](#get_recommender_configurations)
    - [get_segment](#get_segment)
    - [get_segment_export_jobs](#get_segment_export_jobs)
    - [get_segment_import_jobs](#get_segment_import_jobs)
    - [get_segment_version](#get_segment_version)
    - [get_segment_versions](#get_segment_versions)
    - [get_segments](#get_segments)
    - [get_sms_channel](#get_sms_channel)
    - [get_sms_template](#get_sms_template)
    - [get_user_endpoints](#get_user_endpoints)
    - [get_voice_channel](#get_voice_channel)
    - [get_voice_template](#get_voice_template)
    - [list_journeys](#list_journeys)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_template_versions](#list_template_versions)
    - [list_templates](#list_templates)
    - [phone_number_validate](#phone_number_validate)
    - [put_event_stream](#put_event_stream)
    - [put_events](#put_events)
    - [remove_attributes](#remove_attributes)
    - [send_messages](#send_messages)
    - [send_otp_message](#send_otp_message)
    - [send_users_messages](#send_users_messages)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_adm_channel](#update_adm_channel)
    - [update_apns_channel](#update_apns_channel)
    - [update_apns_sandbox_channel](#update_apns_sandbox_channel)
    - [update_apns_voip_channel](#update_apns_voip_channel)
    - [update_apns_voip_sandbox_channel](#update_apns_voip_sandbox_channel)
    - [update_application_settings](#update_application_settings)
    - [update_baidu_channel](#update_baidu_channel)
    - [update_campaign](#update_campaign)
    - [update_email_channel](#update_email_channel)
    - [update_email_template](#update_email_template)
    - [update_endpoint](#update_endpoint)
    - [update_endpoints_batch](#update_endpoints_batch)
    - [update_gcm_channel](#update_gcm_channel)
    - [update_in_app_template](#update_in_app_template)
    - [update_journey](#update_journey)
    - [update_journey_state](#update_journey_state)
    - [update_push_template](#update_push_template)
    - [update_recommender_configuration](#update_recommender_configuration)
    - [update_segment](#update_segment)
    - [update_sms_channel](#update_sms_channel)
    - [update_sms_template](#update_sms_template)
    - [update_template_active_version](#update_template_active_version)
    - [update_voice_channel](#update_voice_channel)
    - [update_voice_template](#update_voice_template)
    - [verify_otp_message](#verify_otp_message)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)

<a id="pinpointclient"></a>

## PinpointClient

Type annotations for `session.create_client("pinpoint")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_pinpoint.client import PinpointClient

session = get_session()
async with session.create_client("pinpoint") as client:
    client: PinpointClient
```

Boto3 documentation:
[Pinpoint.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_pinpoint.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.ForbiddenException`
- `Exceptions.InternalServerErrorException`
- `Exceptions.MethodNotAllowedException`
- `Exceptions.NotFoundException`
- `Exceptions.PayloadTooLargeException`
- `Exceptions.TooManyRequestsException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

PinpointClient exceptions.

Type annotations for `session.create_client("pinpoint").exceptions` method.

Boto3 documentation:
[Pinpoint.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("pinpoint").can_paginate` method.

Boto3 documentation:
[Pinpoint.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_app"></a>

### create_app

Creates an application.

Type annotations for `session.create_client("pinpoint").create_app` method.

Boto3 documentation:
[Pinpoint.Client.create_app](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_app)

Asynchronous method. Use `await create_app(...)` for a synchronous call.

Arguments mapping described in
[CreateAppRequestRequestTypeDef](./type_defs.md#createapprequestrequesttypedef).

Keyword-only arguments:

- `CreateApplicationRequest`:
  [CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[CreateAppResponseTypeDef](./type_defs.md#createappresponsetypedef).

<a id="create_campaign"></a>

### create_campaign

Creates a new campaign for an application or updates the settings of an
existing campaign for an application.

Type annotations for `session.create_client("pinpoint").create_campaign`
method.

Boto3 documentation:
[Pinpoint.Client.create_campaign](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_campaign)

Asynchronous method. Use `await create_campaign(...)` for a synchronous call.

Arguments mapping described in
[CreateCampaignRequestRequestTypeDef](./type_defs.md#createcampaignrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `WriteCampaignRequest`:
  [WriteCampaignRequestTypeDef](./type_defs.md#writecampaignrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[CreateCampaignResponseTypeDef](./type_defs.md#createcampaignresponsetypedef).

<a id="create_email_template"></a>

### create_email_template

Creates a message template for messages that are sent through the email
channel.

Type annotations for `session.create_client("pinpoint").create_email_template`
method.

Boto3 documentation:
[Pinpoint.Client.create_email_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_email_template)

Asynchronous method. Use `await create_email_template(...)` for a synchronous
call.

Arguments mapping described in
[CreateEmailTemplateRequestRequestTypeDef](./type_defs.md#createemailtemplaterequestrequesttypedef).

Keyword-only arguments:

- `EmailTemplateRequest`:
  [EmailTemplateRequestTypeDef](./type_defs.md#emailtemplaterequesttypedef)
  *(required)*
- `TemplateName`: `str` *(required)*

Returns a `Coroutine` for
[CreateEmailTemplateResponseTypeDef](./type_defs.md#createemailtemplateresponsetypedef).

<a id="create_export_job"></a>

### create_export_job

Creates an export job for an application.

Type annotations for `session.create_client("pinpoint").create_export_job`
method.

Boto3 documentation:
[Pinpoint.Client.create_export_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_export_job)

Asynchronous method. Use `await create_export_job(...)` for a synchronous call.

Arguments mapping described in
[CreateExportJobRequestRequestTypeDef](./type_defs.md#createexportjobrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `ExportJobRequest`:
  [ExportJobRequestTypeDef](./type_defs.md#exportjobrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[CreateExportJobResponseTypeDef](./type_defs.md#createexportjobresponsetypedef).

<a id="create_import_job"></a>

### create_import_job

Creates an import job for an application.

Type annotations for `session.create_client("pinpoint").create_import_job`
method.

Boto3 documentation:
[Pinpoint.Client.create_import_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_import_job)

Asynchronous method. Use `await create_import_job(...)` for a synchronous call.

Arguments mapping described in
[CreateImportJobRequestRequestTypeDef](./type_defs.md#createimportjobrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `ImportJobRequest`:
  [ImportJobRequestTypeDef](./type_defs.md#importjobrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[CreateImportJobResponseTypeDef](./type_defs.md#createimportjobresponsetypedef).

<a id="create_in_app_template"></a>

### create_in_app_template

Creates a new message template for messages using the in-app message channel.

Type annotations for `session.create_client("pinpoint").create_in_app_template`
method.

Boto3 documentation:
[Pinpoint.Client.create_in_app_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_in_app_template)

Asynchronous method. Use `await create_in_app_template(...)` for a synchronous
call.

Arguments mapping described in
[CreateInAppTemplateRequestRequestTypeDef](./type_defs.md#createinapptemplaterequestrequesttypedef).

Keyword-only arguments:

- `InAppTemplateRequest`:
  [InAppTemplateRequestTypeDef](./type_defs.md#inapptemplaterequesttypedef)
  *(required)*
- `TemplateName`: `str` *(required)*

Returns a `Coroutine` for
[CreateInAppTemplateResponseTypeDef](./type_defs.md#createinapptemplateresponsetypedef).

<a id="create_journey"></a>

### create_journey

Creates a journey for an application.

Type annotations for `session.create_client("pinpoint").create_journey` method.

Boto3 documentation:
[Pinpoint.Client.create_journey](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_journey)

Asynchronous method. Use `await create_journey(...)` for a synchronous call.

Arguments mapping described in
[CreateJourneyRequestRequestTypeDef](./type_defs.md#createjourneyrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `WriteJourneyRequest`:
  [WriteJourneyRequestTypeDef](./type_defs.md#writejourneyrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[CreateJourneyResponseTypeDef](./type_defs.md#createjourneyresponsetypedef).

<a id="create_push_template"></a>

### create_push_template

Creates a message template for messages that are sent through a push
notification channel.

Type annotations for `session.create_client("pinpoint").create_push_template`
method.

Boto3 documentation:
[Pinpoint.Client.create_push_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_push_template)

Asynchronous method. Use `await create_push_template(...)` for a synchronous
call.

Arguments mapping described in
[CreatePushTemplateRequestRequestTypeDef](./type_defs.md#createpushtemplaterequestrequesttypedef).

Keyword-only arguments:

- `PushNotificationTemplateRequest`:
  [PushNotificationTemplateRequestTypeDef](./type_defs.md#pushnotificationtemplaterequesttypedef)
  *(required)*
- `TemplateName`: `str` *(required)*

Returns a `Coroutine` for
[CreatePushTemplateResponseTypeDef](./type_defs.md#createpushtemplateresponsetypedef).

<a id="create_recommender_configuration"></a>

### create_recommender_configuration

Creates an Amazon Pinpoint configuration for a recommender model.

Type annotations for
`session.create_client("pinpoint").create_recommender_configuration` method.

Boto3 documentation:
[Pinpoint.Client.create_recommender_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_recommender_configuration)

Asynchronous method. Use `await create_recommender_configuration(...)` for a
synchronous call.

Arguments mapping described in
[CreateRecommenderConfigurationRequestRequestTypeDef](./type_defs.md#createrecommenderconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `CreateRecommenderConfiguration`:
  [CreateRecommenderConfigurationTypeDef](./type_defs.md#createrecommenderconfigurationtypedef)
  *(required)*

Returns a `Coroutine` for
[CreateRecommenderConfigurationResponseTypeDef](./type_defs.md#createrecommenderconfigurationresponsetypedef).

<a id="create_segment"></a>

### create_segment

Creates a new segment for an application or updates the configuration,
dimension, and other settings for an existing segment that's associated with an
application.

Type annotations for `session.create_client("pinpoint").create_segment` method.

Boto3 documentation:
[Pinpoint.Client.create_segment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_segment)

Asynchronous method. Use `await create_segment(...)` for a synchronous call.

Arguments mapping described in
[CreateSegmentRequestRequestTypeDef](./type_defs.md#createsegmentrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `WriteSegmentRequest`:
  [WriteSegmentRequestTypeDef](./type_defs.md#writesegmentrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[CreateSegmentResponseTypeDef](./type_defs.md#createsegmentresponsetypedef).

<a id="create_sms_template"></a>

### create_sms_template

Creates a message template for messages that are sent through the SMS channel.

Type annotations for `session.create_client("pinpoint").create_sms_template`
method.

Boto3 documentation:
[Pinpoint.Client.create_sms_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_sms_template)

Asynchronous method. Use `await create_sms_template(...)` for a synchronous
call.

Arguments mapping described in
[CreateSmsTemplateRequestRequestTypeDef](./type_defs.md#createsmstemplaterequestrequesttypedef).

Keyword-only arguments:

- `SMSTemplateRequest`:
  [SMSTemplateRequestTypeDef](./type_defs.md#smstemplaterequesttypedef)
  *(required)*
- `TemplateName`: `str` *(required)*

Returns a `Coroutine` for
[CreateSmsTemplateResponseTypeDef](./type_defs.md#createsmstemplateresponsetypedef).

<a id="create_voice_template"></a>

### create_voice_template

Creates a message template for messages that are sent through the voice
channel.

Type annotations for `session.create_client("pinpoint").create_voice_template`
method.

Boto3 documentation:
[Pinpoint.Client.create_voice_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_voice_template)

Asynchronous method. Use `await create_voice_template(...)` for a synchronous
call.

Arguments mapping described in
[CreateVoiceTemplateRequestRequestTypeDef](./type_defs.md#createvoicetemplaterequestrequesttypedef).

Keyword-only arguments:

- `TemplateName`: `str` *(required)*
- `VoiceTemplateRequest`:
  [VoiceTemplateRequestTypeDef](./type_defs.md#voicetemplaterequesttypedef)
  *(required)*

Returns a `Coroutine` for
[CreateVoiceTemplateResponseTypeDef](./type_defs.md#createvoicetemplateresponsetypedef).

<a id="delete_adm_channel"></a>

### delete_adm_channel

Disables the ADM channel for an application and deletes any existing settings
for the channel.

Type annotations for `session.create_client("pinpoint").delete_adm_channel`
method.

Boto3 documentation:
[Pinpoint.Client.delete_adm_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_adm_channel)

Asynchronous method. Use `await delete_adm_channel(...)` for a synchronous
call.

Arguments mapping described in
[DeleteAdmChannelRequestRequestTypeDef](./type_defs.md#deleteadmchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteAdmChannelResponseTypeDef](./type_defs.md#deleteadmchannelresponsetypedef).

<a id="delete_apns_channel"></a>

### delete_apns_channel

Disables the APNs channel for an application and deletes any existing settings
for the channel.

Type annotations for `session.create_client("pinpoint").delete_apns_channel`
method.

Boto3 documentation:
[Pinpoint.Client.delete_apns_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_apns_channel)

Asynchronous method. Use `await delete_apns_channel(...)` for a synchronous
call.

Arguments mapping described in
[DeleteApnsChannelRequestRequestTypeDef](./type_defs.md#deleteapnschannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteApnsChannelResponseTypeDef](./type_defs.md#deleteapnschannelresponsetypedef).

<a id="delete_apns_sandbox_channel"></a>

### delete_apns_sandbox_channel

Disables the APNs sandbox channel for an application and deletes any existing
settings for the channel.

Type annotations for
`session.create_client("pinpoint").delete_apns_sandbox_channel` method.

Boto3 documentation:
[Pinpoint.Client.delete_apns_sandbox_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_apns_sandbox_channel)

Asynchronous method. Use `await delete_apns_sandbox_channel(...)` for a
synchronous call.

Arguments mapping described in
[DeleteApnsSandboxChannelRequestRequestTypeDef](./type_defs.md#deleteapnssandboxchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteApnsSandboxChannelResponseTypeDef](./type_defs.md#deleteapnssandboxchannelresponsetypedef).

<a id="delete_apns_voip_channel"></a>

### delete_apns_voip_channel

Disables the APNs VoIP channel for an application and deletes any existing
settings for the channel.

Type annotations for
`session.create_client("pinpoint").delete_apns_voip_channel` method.

Boto3 documentation:
[Pinpoint.Client.delete_apns_voip_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_apns_voip_channel)

Asynchronous method. Use `await delete_apns_voip_channel(...)` for a
synchronous call.

Arguments mapping described in
[DeleteApnsVoipChannelRequestRequestTypeDef](./type_defs.md#deleteapnsvoipchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteApnsVoipChannelResponseTypeDef](./type_defs.md#deleteapnsvoipchannelresponsetypedef).

<a id="delete_apns_voip_sandbox_channel"></a>

### delete_apns_voip_sandbox_channel

Disables the APNs VoIP sandbox channel for an application and deletes any
existing settings for the channel.

Type annotations for
`session.create_client("pinpoint").delete_apns_voip_sandbox_channel` method.

Boto3 documentation:
[Pinpoint.Client.delete_apns_voip_sandbox_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_apns_voip_sandbox_channel)

Asynchronous method. Use `await delete_apns_voip_sandbox_channel(...)` for a
synchronous call.

Arguments mapping described in
[DeleteApnsVoipSandboxChannelRequestRequestTypeDef](./type_defs.md#deleteapnsvoipsandboxchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteApnsVoipSandboxChannelResponseTypeDef](./type_defs.md#deleteapnsvoipsandboxchannelresponsetypedef).

<a id="delete_app"></a>

### delete_app

Deletes an application.

Type annotations for `session.create_client("pinpoint").delete_app` method.

Boto3 documentation:
[Pinpoint.Client.delete_app](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_app)

Asynchronous method. Use `await delete_app(...)` for a synchronous call.

Arguments mapping described in
[DeleteAppRequestRequestTypeDef](./type_defs.md#deleteapprequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteAppResponseTypeDef](./type_defs.md#deleteappresponsetypedef).

<a id="delete_baidu_channel"></a>

### delete_baidu_channel

Disables the Baidu channel for an application and deletes any existing settings
for the channel.

Type annotations for `session.create_client("pinpoint").delete_baidu_channel`
method.

Boto3 documentation:
[Pinpoint.Client.delete_baidu_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_baidu_channel)

Asynchronous method. Use `await delete_baidu_channel(...)` for a synchronous
call.

Arguments mapping described in
[DeleteBaiduChannelRequestRequestTypeDef](./type_defs.md#deletebaiduchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteBaiduChannelResponseTypeDef](./type_defs.md#deletebaiduchannelresponsetypedef).

<a id="delete_campaign"></a>

### delete_campaign

Deletes a campaign from an application.

Type annotations for `session.create_client("pinpoint").delete_campaign`
method.

Boto3 documentation:
[Pinpoint.Client.delete_campaign](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_campaign)

Asynchronous method. Use `await delete_campaign(...)` for a synchronous call.

Arguments mapping described in
[DeleteCampaignRequestRequestTypeDef](./type_defs.md#deletecampaignrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `CampaignId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteCampaignResponseTypeDef](./type_defs.md#deletecampaignresponsetypedef).

<a id="delete_email_channel"></a>

### delete_email_channel

Disables the email channel for an application and deletes any existing settings
for the channel.

Type annotations for `session.create_client("pinpoint").delete_email_channel`
method.

Boto3 documentation:
[Pinpoint.Client.delete_email_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_email_channel)

Asynchronous method. Use `await delete_email_channel(...)` for a synchronous
call.

Arguments mapping described in
[DeleteEmailChannelRequestRequestTypeDef](./type_defs.md#deleteemailchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteEmailChannelResponseTypeDef](./type_defs.md#deleteemailchannelresponsetypedef).

<a id="delete_email_template"></a>

### delete_email_template

Deletes a message template for messages that were sent through the email
channel.

Type annotations for `session.create_client("pinpoint").delete_email_template`
method.

Boto3 documentation:
[Pinpoint.Client.delete_email_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_email_template)

Asynchronous method. Use `await delete_email_template(...)` for a synchronous
call.

Arguments mapping described in
[DeleteEmailTemplateRequestRequestTypeDef](./type_defs.md#deleteemailtemplaterequestrequesttypedef).

Keyword-only arguments:

- `TemplateName`: `str` *(required)*
- `Version`: `str`

Returns a `Coroutine` for
[DeleteEmailTemplateResponseTypeDef](./type_defs.md#deleteemailtemplateresponsetypedef).

<a id="delete_endpoint"></a>

### delete_endpoint

Deletes an endpoint from an application.

Type annotations for `session.create_client("pinpoint").delete_endpoint`
method.

Boto3 documentation:
[Pinpoint.Client.delete_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_endpoint)

Asynchronous method. Use `await delete_endpoint(...)` for a synchronous call.

Arguments mapping described in
[DeleteEndpointRequestRequestTypeDef](./type_defs.md#deleteendpointrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EndpointId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteEndpointResponseTypeDef](./type_defs.md#deleteendpointresponsetypedef).

<a id="delete_event_stream"></a>

### delete_event_stream

Deletes the event stream for an application.

Type annotations for `session.create_client("pinpoint").delete_event_stream`
method.

Boto3 documentation:
[Pinpoint.Client.delete_event_stream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_event_stream)

Asynchronous method. Use `await delete_event_stream(...)` for a synchronous
call.

Arguments mapping described in
[DeleteEventStreamRequestRequestTypeDef](./type_defs.md#deleteeventstreamrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteEventStreamResponseTypeDef](./type_defs.md#deleteeventstreamresponsetypedef).

<a id="delete_gcm_channel"></a>

### delete_gcm_channel

Disables the GCM channel for an application and deletes any existing settings
for the channel.

Type annotations for `session.create_client("pinpoint").delete_gcm_channel`
method.

Boto3 documentation:
[Pinpoint.Client.delete_gcm_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_gcm_channel)

Asynchronous method. Use `await delete_gcm_channel(...)` for a synchronous
call.

Arguments mapping described in
[DeleteGcmChannelRequestRequestTypeDef](./type_defs.md#deletegcmchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteGcmChannelResponseTypeDef](./type_defs.md#deletegcmchannelresponsetypedef).

<a id="delete_in_app_template"></a>

### delete_in_app_template

Deletes a message template for messages sent using the in-app message channel.

Type annotations for `session.create_client("pinpoint").delete_in_app_template`
method.

Boto3 documentation:
[Pinpoint.Client.delete_in_app_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_in_app_template)

Asynchronous method. Use `await delete_in_app_template(...)` for a synchronous
call.

Arguments mapping described in
[DeleteInAppTemplateRequestRequestTypeDef](./type_defs.md#deleteinapptemplaterequestrequesttypedef).

Keyword-only arguments:

- `TemplateName`: `str` *(required)*
- `Version`: `str`

Returns a `Coroutine` for
[DeleteInAppTemplateResponseTypeDef](./type_defs.md#deleteinapptemplateresponsetypedef).

<a id="delete_journey"></a>

### delete_journey

Deletes a journey from an application.

Type annotations for `session.create_client("pinpoint").delete_journey` method.

Boto3 documentation:
[Pinpoint.Client.delete_journey](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_journey)

Asynchronous method. Use `await delete_journey(...)` for a synchronous call.

Arguments mapping described in
[DeleteJourneyRequestRequestTypeDef](./type_defs.md#deletejourneyrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `JourneyId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteJourneyResponseTypeDef](./type_defs.md#deletejourneyresponsetypedef).

<a id="delete_push_template"></a>

### delete_push_template

Deletes a message template for messages that were sent through a push
notification channel.

Type annotations for `session.create_client("pinpoint").delete_push_template`
method.

Boto3 documentation:
[Pinpoint.Client.delete_push_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_push_template)

Asynchronous method. Use `await delete_push_template(...)` for a synchronous
call.

Arguments mapping described in
[DeletePushTemplateRequestRequestTypeDef](./type_defs.md#deletepushtemplaterequestrequesttypedef).

Keyword-only arguments:

- `TemplateName`: `str` *(required)*
- `Version`: `str`

Returns a `Coroutine` for
[DeletePushTemplateResponseTypeDef](./type_defs.md#deletepushtemplateresponsetypedef).

<a id="delete_recommender_configuration"></a>

### delete_recommender_configuration

Deletes an Amazon Pinpoint configuration for a recommender model.

Type annotations for
`session.create_client("pinpoint").delete_recommender_configuration` method.

Boto3 documentation:
[Pinpoint.Client.delete_recommender_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_recommender_configuration)

Asynchronous method. Use `await delete_recommender_configuration(...)` for a
synchronous call.

Arguments mapping described in
[DeleteRecommenderConfigurationRequestRequestTypeDef](./type_defs.md#deleterecommenderconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `RecommenderId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteRecommenderConfigurationResponseTypeDef](./type_defs.md#deleterecommenderconfigurationresponsetypedef).

<a id="delete_segment"></a>

### delete_segment

Deletes a segment from an application.

Type annotations for `session.create_client("pinpoint").delete_segment` method.

Boto3 documentation:
[Pinpoint.Client.delete_segment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_segment)

Asynchronous method. Use `await delete_segment(...)` for a synchronous call.

Arguments mapping described in
[DeleteSegmentRequestRequestTypeDef](./type_defs.md#deletesegmentrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `SegmentId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteSegmentResponseTypeDef](./type_defs.md#deletesegmentresponsetypedef).

<a id="delete_sms_channel"></a>

### delete_sms_channel

Disables the SMS channel for an application and deletes any existing settings
for the channel.

Type annotations for `session.create_client("pinpoint").delete_sms_channel`
method.

Boto3 documentation:
[Pinpoint.Client.delete_sms_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_sms_channel)

Asynchronous method. Use `await delete_sms_channel(...)` for a synchronous
call.

Arguments mapping described in
[DeleteSmsChannelRequestRequestTypeDef](./type_defs.md#deletesmschannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteSmsChannelResponseTypeDef](./type_defs.md#deletesmschannelresponsetypedef).

<a id="delete_sms_template"></a>

### delete_sms_template

Deletes a message template for messages that were sent through the SMS channel.

Type annotations for `session.create_client("pinpoint").delete_sms_template`
method.

Boto3 documentation:
[Pinpoint.Client.delete_sms_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_sms_template)

Asynchronous method. Use `await delete_sms_template(...)` for a synchronous
call.

Arguments mapping described in
[DeleteSmsTemplateRequestRequestTypeDef](./type_defs.md#deletesmstemplaterequestrequesttypedef).

Keyword-only arguments:

- `TemplateName`: `str` *(required)*
- `Version`: `str`

Returns a `Coroutine` for
[DeleteSmsTemplateResponseTypeDef](./type_defs.md#deletesmstemplateresponsetypedef).

<a id="delete_user_endpoints"></a>

### delete_user_endpoints

Deletes all the endpoints that are associated with a specific user ID.

Type annotations for `session.create_client("pinpoint").delete_user_endpoints`
method.

Boto3 documentation:
[Pinpoint.Client.delete_user_endpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_user_endpoints)

Asynchronous method. Use `await delete_user_endpoints(...)` for a synchronous
call.

Arguments mapping described in
[DeleteUserEndpointsRequestRequestTypeDef](./type_defs.md#deleteuserendpointsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `UserId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteUserEndpointsResponseTypeDef](./type_defs.md#deleteuserendpointsresponsetypedef).

<a id="delete_voice_channel"></a>

### delete_voice_channel

Disables the voice channel for an application and deletes any existing settings
for the channel.

Type annotations for `session.create_client("pinpoint").delete_voice_channel`
method.

Boto3 documentation:
[Pinpoint.Client.delete_voice_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_voice_channel)

Asynchronous method. Use `await delete_voice_channel(...)` for a synchronous
call.

Arguments mapping described in
[DeleteVoiceChannelRequestRequestTypeDef](./type_defs.md#deletevoicechannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteVoiceChannelResponseTypeDef](./type_defs.md#deletevoicechannelresponsetypedef).

<a id="delete_voice_template"></a>

### delete_voice_template

Deletes a message template for messages that were sent through the voice
channel.

Type annotations for `session.create_client("pinpoint").delete_voice_template`
method.

Boto3 documentation:
[Pinpoint.Client.delete_voice_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.delete_voice_template)

Asynchronous method. Use `await delete_voice_template(...)` for a synchronous
call.

Arguments mapping described in
[DeleteVoiceTemplateRequestRequestTypeDef](./type_defs.md#deletevoicetemplaterequestrequesttypedef).

Keyword-only arguments:

- `TemplateName`: `str` *(required)*
- `Version`: `str`

Returns a `Coroutine` for
[DeleteVoiceTemplateResponseTypeDef](./type_defs.md#deletevoicetemplateresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("pinpoint").generate_presigned_url`
method.

Boto3 documentation:
[Pinpoint.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_adm_channel"></a>

### get_adm_channel

Retrieves information about the status and settings of the ADM channel for an
application.

Type annotations for `session.create_client("pinpoint").get_adm_channel`
method.

Boto3 documentation:
[Pinpoint.Client.get_adm_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_adm_channel)

Asynchronous method. Use `await get_adm_channel(...)` for a synchronous call.

Arguments mapping described in
[GetAdmChannelRequestRequestTypeDef](./type_defs.md#getadmchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetAdmChannelResponseTypeDef](./type_defs.md#getadmchannelresponsetypedef).

<a id="get_apns_channel"></a>

### get_apns_channel

Retrieves information about the status and settings of the APNs channel for an
application.

Type annotations for `session.create_client("pinpoint").get_apns_channel`
method.

Boto3 documentation:
[Pinpoint.Client.get_apns_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_apns_channel)

Asynchronous method. Use `await get_apns_channel(...)` for a synchronous call.

Arguments mapping described in
[GetApnsChannelRequestRequestTypeDef](./type_defs.md#getapnschannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetApnsChannelResponseTypeDef](./type_defs.md#getapnschannelresponsetypedef).

<a id="get_apns_sandbox_channel"></a>

### get_apns_sandbox_channel

Retrieves information about the status and settings of the APNs sandbox channel
for an application.

Type annotations for
`session.create_client("pinpoint").get_apns_sandbox_channel` method.

Boto3 documentation:
[Pinpoint.Client.get_apns_sandbox_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_apns_sandbox_channel)

Asynchronous method. Use `await get_apns_sandbox_channel(...)` for a
synchronous call.

Arguments mapping described in
[GetApnsSandboxChannelRequestRequestTypeDef](./type_defs.md#getapnssandboxchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetApnsSandboxChannelResponseTypeDef](./type_defs.md#getapnssandboxchannelresponsetypedef).

<a id="get_apns_voip_channel"></a>

### get_apns_voip_channel

Retrieves information about the status and settings of the APNs VoIP channel
for an application.

Type annotations for `session.create_client("pinpoint").get_apns_voip_channel`
method.

Boto3 documentation:
[Pinpoint.Client.get_apns_voip_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_apns_voip_channel)

Asynchronous method. Use `await get_apns_voip_channel(...)` for a synchronous
call.

Arguments mapping described in
[GetApnsVoipChannelRequestRequestTypeDef](./type_defs.md#getapnsvoipchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetApnsVoipChannelResponseTypeDef](./type_defs.md#getapnsvoipchannelresponsetypedef).

<a id="get_apns_voip_sandbox_channel"></a>

### get_apns_voip_sandbox_channel

Retrieves information about the status and settings of the APNs VoIP sandbox
channel for an application.

Type annotations for
`session.create_client("pinpoint").get_apns_voip_sandbox_channel` method.

Boto3 documentation:
[Pinpoint.Client.get_apns_voip_sandbox_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_apns_voip_sandbox_channel)

Asynchronous method. Use `await get_apns_voip_sandbox_channel(...)` for a
synchronous call.

Arguments mapping described in
[GetApnsVoipSandboxChannelRequestRequestTypeDef](./type_defs.md#getapnsvoipsandboxchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetApnsVoipSandboxChannelResponseTypeDef](./type_defs.md#getapnsvoipsandboxchannelresponsetypedef).

<a id="get_app"></a>

### get_app

Retrieves information about an application.

Type annotations for `session.create_client("pinpoint").get_app` method.

Boto3 documentation:
[Pinpoint.Client.get_app](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_app)

Asynchronous method. Use `await get_app(...)` for a synchronous call.

Arguments mapping described in
[GetAppRequestRequestTypeDef](./type_defs.md#getapprequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetAppResponseTypeDef](./type_defs.md#getappresponsetypedef).

<a id="get_application_date_range_kpi"></a>

### get_application_date_range_kpi

Retrieves (queries) pre-aggregated data for a standard metric that applies to
an application.

Type annotations for
`session.create_client("pinpoint").get_application_date_range_kpi` method.

Boto3 documentation:
[Pinpoint.Client.get_application_date_range_kpi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_application_date_range_kpi)

Asynchronous method. Use `await get_application_date_range_kpi(...)` for a
synchronous call.

Arguments mapping described in
[GetApplicationDateRangeKpiRequestRequestTypeDef](./type_defs.md#getapplicationdaterangekpirequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `KpiName`: `str` *(required)*
- `EndTime`: `Union`\[`datetime`, `str`\]
- `NextToken`: `str`
- `PageSize`: `str`
- `StartTime`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for
[GetApplicationDateRangeKpiResponseTypeDef](./type_defs.md#getapplicationdaterangekpiresponsetypedef).

<a id="get_application_settings"></a>

### get_application_settings

Retrieves information about the settings for an application.

Type annotations for
`session.create_client("pinpoint").get_application_settings` method.

Boto3 documentation:
[Pinpoint.Client.get_application_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_application_settings)

Asynchronous method. Use `await get_application_settings(...)` for a
synchronous call.

Arguments mapping described in
[GetApplicationSettingsRequestRequestTypeDef](./type_defs.md#getapplicationsettingsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetApplicationSettingsResponseTypeDef](./type_defs.md#getapplicationsettingsresponsetypedef).

<a id="get_apps"></a>

### get_apps

Retrieves information about all the applications that are associated with your
Amazon Pinpoint account.

Type annotations for `session.create_client("pinpoint").get_apps` method.

Boto3 documentation:
[Pinpoint.Client.get_apps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_apps)

Asynchronous method. Use `await get_apps(...)` for a synchronous call.

Arguments mapping described in
[GetAppsRequestRequestTypeDef](./type_defs.md#getappsrequestrequesttypedef).

Keyword-only arguments:

- `PageSize`: `str`
- `Token`: `str`

Returns a `Coroutine` for
[GetAppsResponseTypeDef](./type_defs.md#getappsresponsetypedef).

<a id="get_baidu_channel"></a>

### get_baidu_channel

Retrieves information about the status and settings of the Baidu channel for an
application.

Type annotations for `session.create_client("pinpoint").get_baidu_channel`
method.

Boto3 documentation:
[Pinpoint.Client.get_baidu_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_baidu_channel)

Asynchronous method. Use `await get_baidu_channel(...)` for a synchronous call.

Arguments mapping described in
[GetBaiduChannelRequestRequestTypeDef](./type_defs.md#getbaiduchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetBaiduChannelResponseTypeDef](./type_defs.md#getbaiduchannelresponsetypedef).

<a id="get_campaign"></a>

### get_campaign

Retrieves information about the status, configuration, and other settings for a
campaign.

Type annotations for `session.create_client("pinpoint").get_campaign` method.

Boto3 documentation:
[Pinpoint.Client.get_campaign](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_campaign)

Asynchronous method. Use `await get_campaign(...)` for a synchronous call.

Arguments mapping described in
[GetCampaignRequestRequestTypeDef](./type_defs.md#getcampaignrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `CampaignId`: `str` *(required)*

Returns a `Coroutine` for
[GetCampaignResponseTypeDef](./type_defs.md#getcampaignresponsetypedef).

<a id="get_campaign_activities"></a>

### get_campaign_activities

Retrieves information about all the activities for a campaign.

Type annotations for
`session.create_client("pinpoint").get_campaign_activities` method.

Boto3 documentation:
[Pinpoint.Client.get_campaign_activities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_campaign_activities)

Asynchronous method. Use `await get_campaign_activities(...)` for a synchronous
call.

Arguments mapping described in
[GetCampaignActivitiesRequestRequestTypeDef](./type_defs.md#getcampaignactivitiesrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `CampaignId`: `str` *(required)*
- `PageSize`: `str`
- `Token`: `str`

Returns a `Coroutine` for
[GetCampaignActivitiesResponseTypeDef](./type_defs.md#getcampaignactivitiesresponsetypedef).

<a id="get_campaign_date_range_kpi"></a>

### get_campaign_date_range_kpi

Retrieves (queries) pre-aggregated data for a standard metric that applies to a
campaign.

Type annotations for
`session.create_client("pinpoint").get_campaign_date_range_kpi` method.

Boto3 documentation:
[Pinpoint.Client.get_campaign_date_range_kpi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_campaign_date_range_kpi)

Asynchronous method. Use `await get_campaign_date_range_kpi(...)` for a
synchronous call.

Arguments mapping described in
[GetCampaignDateRangeKpiRequestRequestTypeDef](./type_defs.md#getcampaigndaterangekpirequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `CampaignId`: `str` *(required)*
- `KpiName`: `str` *(required)*
- `EndTime`: `Union`\[`datetime`, `str`\]
- `NextToken`: `str`
- `PageSize`: `str`
- `StartTime`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for
[GetCampaignDateRangeKpiResponseTypeDef](./type_defs.md#getcampaigndaterangekpiresponsetypedef).

<a id="get_campaign_version"></a>

### get_campaign_version

Retrieves information about the status, configuration, and other settings for a
specific version of a campaign.

Type annotations for `session.create_client("pinpoint").get_campaign_version`
method.

Boto3 documentation:
[Pinpoint.Client.get_campaign_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_campaign_version)

Asynchronous method. Use `await get_campaign_version(...)` for a synchronous
call.

Arguments mapping described in
[GetCampaignVersionRequestRequestTypeDef](./type_defs.md#getcampaignversionrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `CampaignId`: `str` *(required)*
- `Version`: `str` *(required)*

Returns a `Coroutine` for
[GetCampaignVersionResponseTypeDef](./type_defs.md#getcampaignversionresponsetypedef).

<a id="get_campaign_versions"></a>

### get_campaign_versions

Retrieves information about the status, configuration, and other settings for
all versions of a campaign.

Type annotations for `session.create_client("pinpoint").get_campaign_versions`
method.

Boto3 documentation:
[Pinpoint.Client.get_campaign_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_campaign_versions)

Asynchronous method. Use `await get_campaign_versions(...)` for a synchronous
call.

Arguments mapping described in
[GetCampaignVersionsRequestRequestTypeDef](./type_defs.md#getcampaignversionsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `CampaignId`: `str` *(required)*
- `PageSize`: `str`
- `Token`: `str`

Returns a `Coroutine` for
[GetCampaignVersionsResponseTypeDef](./type_defs.md#getcampaignversionsresponsetypedef).

<a id="get_campaigns"></a>

### get_campaigns

Retrieves information about the status, configuration, and other settings for
all the campaigns that are associated with an application.

Type annotations for `session.create_client("pinpoint").get_campaigns` method.

Boto3 documentation:
[Pinpoint.Client.get_campaigns](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_campaigns)

Asynchronous method. Use `await get_campaigns(...)` for a synchronous call.

Arguments mapping described in
[GetCampaignsRequestRequestTypeDef](./type_defs.md#getcampaignsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `PageSize`: `str`
- `Token`: `str`

Returns a `Coroutine` for
[GetCampaignsResponseTypeDef](./type_defs.md#getcampaignsresponsetypedef).

<a id="get_channels"></a>

### get_channels

Retrieves information about the history and status of each channel for an
application.

Type annotations for `session.create_client("pinpoint").get_channels` method.

Boto3 documentation:
[Pinpoint.Client.get_channels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_channels)

Asynchronous method. Use `await get_channels(...)` for a synchronous call.

Arguments mapping described in
[GetChannelsRequestRequestTypeDef](./type_defs.md#getchannelsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetChannelsResponseTypeDef](./type_defs.md#getchannelsresponsetypedef).

<a id="get_email_channel"></a>

### get_email_channel

Retrieves information about the status and settings of the email channel for an
application.

Type annotations for `session.create_client("pinpoint").get_email_channel`
method.

Boto3 documentation:
[Pinpoint.Client.get_email_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_email_channel)

Asynchronous method. Use `await get_email_channel(...)` for a synchronous call.

Arguments mapping described in
[GetEmailChannelRequestRequestTypeDef](./type_defs.md#getemailchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetEmailChannelResponseTypeDef](./type_defs.md#getemailchannelresponsetypedef).

<a id="get_email_template"></a>

### get_email_template

Retrieves the content and settings of a message template for messages that are
sent through the email channel.

Type annotations for `session.create_client("pinpoint").get_email_template`
method.

Boto3 documentation:
[Pinpoint.Client.get_email_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_email_template)

Asynchronous method. Use `await get_email_template(...)` for a synchronous
call.

Arguments mapping described in
[GetEmailTemplateRequestRequestTypeDef](./type_defs.md#getemailtemplaterequestrequesttypedef).

Keyword-only arguments:

- `TemplateName`: `str` *(required)*
- `Version`: `str`

Returns a `Coroutine` for
[GetEmailTemplateResponseTypeDef](./type_defs.md#getemailtemplateresponsetypedef).

<a id="get_endpoint"></a>

### get_endpoint

Retrieves information about the settings and attributes of a specific endpoint
for an application.

Type annotations for `session.create_client("pinpoint").get_endpoint` method.

Boto3 documentation:
[Pinpoint.Client.get_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_endpoint)

Asynchronous method. Use `await get_endpoint(...)` for a synchronous call.

Arguments mapping described in
[GetEndpointRequestRequestTypeDef](./type_defs.md#getendpointrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EndpointId`: `str` *(required)*

Returns a `Coroutine` for
[GetEndpointResponseTypeDef](./type_defs.md#getendpointresponsetypedef).

<a id="get_event_stream"></a>

### get_event_stream

Retrieves information about the event stream settings for an application.

Type annotations for `session.create_client("pinpoint").get_event_stream`
method.

Boto3 documentation:
[Pinpoint.Client.get_event_stream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_event_stream)

Asynchronous method. Use `await get_event_stream(...)` for a synchronous call.

Arguments mapping described in
[GetEventStreamRequestRequestTypeDef](./type_defs.md#geteventstreamrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetEventStreamResponseTypeDef](./type_defs.md#geteventstreamresponsetypedef).

<a id="get_export_job"></a>

### get_export_job

Retrieves information about the status and settings of a specific export job
for an application.

Type annotations for `session.create_client("pinpoint").get_export_job` method.

Boto3 documentation:
[Pinpoint.Client.get_export_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_export_job)

Asynchronous method. Use `await get_export_job(...)` for a synchronous call.

Arguments mapping described in
[GetExportJobRequestRequestTypeDef](./type_defs.md#getexportjobrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `JobId`: `str` *(required)*

Returns a `Coroutine` for
[GetExportJobResponseTypeDef](./type_defs.md#getexportjobresponsetypedef).

<a id="get_export_jobs"></a>

### get_export_jobs

Retrieves information about the status and settings of all the export jobs for
an application.

Type annotations for `session.create_client("pinpoint").get_export_jobs`
method.

Boto3 documentation:
[Pinpoint.Client.get_export_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_export_jobs)

Asynchronous method. Use `await get_export_jobs(...)` for a synchronous call.

Arguments mapping described in
[GetExportJobsRequestRequestTypeDef](./type_defs.md#getexportjobsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `PageSize`: `str`
- `Token`: `str`

Returns a `Coroutine` for
[GetExportJobsResponseTypeDef](./type_defs.md#getexportjobsresponsetypedef).

<a id="get_gcm_channel"></a>

### get_gcm_channel

Retrieves information about the status and settings of the GCM channel for an
application.

Type annotations for `session.create_client("pinpoint").get_gcm_channel`
method.

Boto3 documentation:
[Pinpoint.Client.get_gcm_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_gcm_channel)

Asynchronous method. Use `await get_gcm_channel(...)` for a synchronous call.

Arguments mapping described in
[GetGcmChannelRequestRequestTypeDef](./type_defs.md#getgcmchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetGcmChannelResponseTypeDef](./type_defs.md#getgcmchannelresponsetypedef).

<a id="get_import_job"></a>

### get_import_job

Retrieves information about the status and settings of a specific import job
for an application.

Type annotations for `session.create_client("pinpoint").get_import_job` method.

Boto3 documentation:
[Pinpoint.Client.get_import_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_import_job)

Asynchronous method. Use `await get_import_job(...)` for a synchronous call.

Arguments mapping described in
[GetImportJobRequestRequestTypeDef](./type_defs.md#getimportjobrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `JobId`: `str` *(required)*

Returns a `Coroutine` for
[GetImportJobResponseTypeDef](./type_defs.md#getimportjobresponsetypedef).

<a id="get_import_jobs"></a>

### get_import_jobs

Retrieves information about the status and settings of all the import jobs for
an application.

Type annotations for `session.create_client("pinpoint").get_import_jobs`
method.

Boto3 documentation:
[Pinpoint.Client.get_import_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_import_jobs)

Asynchronous method. Use `await get_import_jobs(...)` for a synchronous call.

Arguments mapping described in
[GetImportJobsRequestRequestTypeDef](./type_defs.md#getimportjobsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `PageSize`: `str`
- `Token`: `str`

Returns a `Coroutine` for
[GetImportJobsResponseTypeDef](./type_defs.md#getimportjobsresponsetypedef).

<a id="get_in_app_messages"></a>

### get_in_app_messages

Retrieves the in-app messages targeted for the provided endpoint ID.

Type annotations for `session.create_client("pinpoint").get_in_app_messages`
method.

Boto3 documentation:
[Pinpoint.Client.get_in_app_messages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_in_app_messages)

Asynchronous method. Use `await get_in_app_messages(...)` for a synchronous
call.

Arguments mapping described in
[GetInAppMessagesRequestRequestTypeDef](./type_defs.md#getinappmessagesrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EndpointId`: `str` *(required)*

Returns a `Coroutine` for
[GetInAppMessagesResponseTypeDef](./type_defs.md#getinappmessagesresponsetypedef).

<a id="get_in_app_template"></a>

### get_in_app_template

Retrieves the content and settings of a message template for messages sent
through the in-app channel.

Type annotations for `session.create_client("pinpoint").get_in_app_template`
method.

Boto3 documentation:
[Pinpoint.Client.get_in_app_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_in_app_template)

Asynchronous method. Use `await get_in_app_template(...)` for a synchronous
call.

Arguments mapping described in
[GetInAppTemplateRequestRequestTypeDef](./type_defs.md#getinapptemplaterequestrequesttypedef).

Keyword-only arguments:

- `TemplateName`: `str` *(required)*
- `Version`: `str`

Returns a `Coroutine` for
[GetInAppTemplateResponseTypeDef](./type_defs.md#getinapptemplateresponsetypedef).

<a id="get_journey"></a>

### get_journey

Retrieves information about the status, configuration, and other settings for a
journey.

Type annotations for `session.create_client("pinpoint").get_journey` method.

Boto3 documentation:
[Pinpoint.Client.get_journey](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey)

Asynchronous method. Use `await get_journey(...)` for a synchronous call.

Arguments mapping described in
[GetJourneyRequestRequestTypeDef](./type_defs.md#getjourneyrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `JourneyId`: `str` *(required)*

Returns a `Coroutine` for
[GetJourneyResponseTypeDef](./type_defs.md#getjourneyresponsetypedef).

<a id="get_journey_date_range_kpi"></a>

### get_journey_date_range_kpi

Retrieves (queries) pre-aggregated data for a standard engagement metric that
applies to a journey.

Type annotations for
`session.create_client("pinpoint").get_journey_date_range_kpi` method.

Boto3 documentation:
[Pinpoint.Client.get_journey_date_range_kpi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_date_range_kpi)

Asynchronous method. Use `await get_journey_date_range_kpi(...)` for a
synchronous call.

Arguments mapping described in
[GetJourneyDateRangeKpiRequestRequestTypeDef](./type_defs.md#getjourneydaterangekpirequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `JourneyId`: `str` *(required)*
- `KpiName`: `str` *(required)*
- `EndTime`: `Union`\[`datetime`, `str`\]
- `NextToken`: `str`
- `PageSize`: `str`
- `StartTime`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for
[GetJourneyDateRangeKpiResponseTypeDef](./type_defs.md#getjourneydaterangekpiresponsetypedef).

<a id="get_journey_execution_activity_metrics"></a>

### get_journey_execution_activity_metrics

Retrieves (queries) pre-aggregated data for a standard execution metric that
applies to a journey activity.

Type annotations for
`session.create_client("pinpoint").get_journey_execution_activity_metrics`
method.

Boto3 documentation:
[Pinpoint.Client.get_journey_execution_activity_metrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_execution_activity_metrics)

Asynchronous method. Use `await get_journey_execution_activity_metrics(...)`
for a synchronous call.

Arguments mapping described in
[GetJourneyExecutionActivityMetricsRequestRequestTypeDef](./type_defs.md#getjourneyexecutionactivitymetricsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `JourneyActivityId`: `str` *(required)*
- `JourneyId`: `str` *(required)*
- `NextToken`: `str`
- `PageSize`: `str`

Returns a `Coroutine` for
[GetJourneyExecutionActivityMetricsResponseTypeDef](./type_defs.md#getjourneyexecutionactivitymetricsresponsetypedef).

<a id="get_journey_execution_metrics"></a>

### get_journey_execution_metrics

Retrieves (queries) pre-aggregated data for a standard execution metric that
applies to a journey.

Type annotations for
`session.create_client("pinpoint").get_journey_execution_metrics` method.

Boto3 documentation:
[Pinpoint.Client.get_journey_execution_metrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_execution_metrics)

Asynchronous method. Use `await get_journey_execution_metrics(...)` for a
synchronous call.

Arguments mapping described in
[GetJourneyExecutionMetricsRequestRequestTypeDef](./type_defs.md#getjourneyexecutionmetricsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `JourneyId`: `str` *(required)*
- `NextToken`: `str`
- `PageSize`: `str`

Returns a `Coroutine` for
[GetJourneyExecutionMetricsResponseTypeDef](./type_defs.md#getjourneyexecutionmetricsresponsetypedef).

<a id="get_push_template"></a>

### get_push_template

Retrieves the content and settings of a message template for messages that are
sent through a push notification channel.

Type annotations for `session.create_client("pinpoint").get_push_template`
method.

Boto3 documentation:
[Pinpoint.Client.get_push_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_push_template)

Asynchronous method. Use `await get_push_template(...)` for a synchronous call.

Arguments mapping described in
[GetPushTemplateRequestRequestTypeDef](./type_defs.md#getpushtemplaterequestrequesttypedef).

Keyword-only arguments:

- `TemplateName`: `str` *(required)*
- `Version`: `str`

Returns a `Coroutine` for
[GetPushTemplateResponseTypeDef](./type_defs.md#getpushtemplateresponsetypedef).

<a id="get_recommender_configuration"></a>

### get_recommender_configuration

Retrieves information about an Amazon Pinpoint configuration for a recommender
model.

Type annotations for
`session.create_client("pinpoint").get_recommender_configuration` method.

Boto3 documentation:
[Pinpoint.Client.get_recommender_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_recommender_configuration)

Asynchronous method. Use `await get_recommender_configuration(...)` for a
synchronous call.

Arguments mapping described in
[GetRecommenderConfigurationRequestRequestTypeDef](./type_defs.md#getrecommenderconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `RecommenderId`: `str` *(required)*

Returns a `Coroutine` for
[GetRecommenderConfigurationResponseTypeDef](./type_defs.md#getrecommenderconfigurationresponsetypedef).

<a id="get_recommender_configurations"></a>

### get_recommender_configurations

Retrieves information about all the recommender model configurations that are
associated with your Amazon Pinpoint account.

Type annotations for
`session.create_client("pinpoint").get_recommender_configurations` method.

Boto3 documentation:
[Pinpoint.Client.get_recommender_configurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_recommender_configurations)

Asynchronous method. Use `await get_recommender_configurations(...)` for a
synchronous call.

Arguments mapping described in
[GetRecommenderConfigurationsRequestRequestTypeDef](./type_defs.md#getrecommenderconfigurationsrequestrequesttypedef).

Keyword-only arguments:

- `PageSize`: `str`
- `Token`: `str`

Returns a `Coroutine` for
[GetRecommenderConfigurationsResponseTypeDef](./type_defs.md#getrecommenderconfigurationsresponsetypedef).

<a id="get_segment"></a>

### get_segment

Retrieves information about the configuration, dimension, and other settings
for a specific segment that's associated with an application.

Type annotations for `session.create_client("pinpoint").get_segment` method.

Boto3 documentation:
[Pinpoint.Client.get_segment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_segment)

Asynchronous method. Use `await get_segment(...)` for a synchronous call.

Arguments mapping described in
[GetSegmentRequestRequestTypeDef](./type_defs.md#getsegmentrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `SegmentId`: `str` *(required)*

Returns a `Coroutine` for
[GetSegmentResponseTypeDef](./type_defs.md#getsegmentresponsetypedef).

<a id="get_segment_export_jobs"></a>

### get_segment_export_jobs

Retrieves information about the status and settings of the export jobs for a
segment.

Type annotations for
`session.create_client("pinpoint").get_segment_export_jobs` method.

Boto3 documentation:
[Pinpoint.Client.get_segment_export_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_segment_export_jobs)

Asynchronous method. Use `await get_segment_export_jobs(...)` for a synchronous
call.

Arguments mapping described in
[GetSegmentExportJobsRequestRequestTypeDef](./type_defs.md#getsegmentexportjobsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `SegmentId`: `str` *(required)*
- `PageSize`: `str`
- `Token`: `str`

Returns a `Coroutine` for
[GetSegmentExportJobsResponseTypeDef](./type_defs.md#getsegmentexportjobsresponsetypedef).

<a id="get_segment_import_jobs"></a>

### get_segment_import_jobs

Retrieves information about the status and settings of the import jobs for a
segment.

Type annotations for
`session.create_client("pinpoint").get_segment_import_jobs` method.

Boto3 documentation:
[Pinpoint.Client.get_segment_import_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_segment_import_jobs)

Asynchronous method. Use `await get_segment_import_jobs(...)` for a synchronous
call.

Arguments mapping described in
[GetSegmentImportJobsRequestRequestTypeDef](./type_defs.md#getsegmentimportjobsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `SegmentId`: `str` *(required)*
- `PageSize`: `str`
- `Token`: `str`

Returns a `Coroutine` for
[GetSegmentImportJobsResponseTypeDef](./type_defs.md#getsegmentimportjobsresponsetypedef).

<a id="get_segment_version"></a>

### get_segment_version

Retrieves information about the configuration, dimension, and other settings
for a specific version of a segment that's associated with an application.

Type annotations for `session.create_client("pinpoint").get_segment_version`
method.

Boto3 documentation:
[Pinpoint.Client.get_segment_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_segment_version)

Asynchronous method. Use `await get_segment_version(...)` for a synchronous
call.

Arguments mapping described in
[GetSegmentVersionRequestRequestTypeDef](./type_defs.md#getsegmentversionrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `SegmentId`: `str` *(required)*
- `Version`: `str` *(required)*

Returns a `Coroutine` for
[GetSegmentVersionResponseTypeDef](./type_defs.md#getsegmentversionresponsetypedef).

<a id="get_segment_versions"></a>

### get_segment_versions

Retrieves information about the configuration, dimension, and other settings
for all the versions of a specific segment that's associated with an
application.

Type annotations for `session.create_client("pinpoint").get_segment_versions`
method.

Boto3 documentation:
[Pinpoint.Client.get_segment_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_segment_versions)

Asynchronous method. Use `await get_segment_versions(...)` for a synchronous
call.

Arguments mapping described in
[GetSegmentVersionsRequestRequestTypeDef](./type_defs.md#getsegmentversionsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `SegmentId`: `str` *(required)*
- `PageSize`: `str`
- `Token`: `str`

Returns a `Coroutine` for
[GetSegmentVersionsResponseTypeDef](./type_defs.md#getsegmentversionsresponsetypedef).

<a id="get_segments"></a>

### get_segments

Retrieves information about the configuration, dimension, and other settings
for all the segments that are associated with an application.

Type annotations for `session.create_client("pinpoint").get_segments` method.

Boto3 documentation:
[Pinpoint.Client.get_segments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_segments)

Asynchronous method. Use `await get_segments(...)` for a synchronous call.

Arguments mapping described in
[GetSegmentsRequestRequestTypeDef](./type_defs.md#getsegmentsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `PageSize`: `str`
- `Token`: `str`

Returns a `Coroutine` for
[GetSegmentsResponseTypeDef](./type_defs.md#getsegmentsresponsetypedef).

<a id="get_sms_channel"></a>

### get_sms_channel

Retrieves information about the status and settings of the SMS channel for an
application.

Type annotations for `session.create_client("pinpoint").get_sms_channel`
method.

Boto3 documentation:
[Pinpoint.Client.get_sms_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_sms_channel)

Asynchronous method. Use `await get_sms_channel(...)` for a synchronous call.

Arguments mapping described in
[GetSmsChannelRequestRequestTypeDef](./type_defs.md#getsmschannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetSmsChannelResponseTypeDef](./type_defs.md#getsmschannelresponsetypedef).

<a id="get_sms_template"></a>

### get_sms_template

Retrieves the content and settings of a message template for messages that are
sent through the SMS channel.

Type annotations for `session.create_client("pinpoint").get_sms_template`
method.

Boto3 documentation:
[Pinpoint.Client.get_sms_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_sms_template)

Asynchronous method. Use `await get_sms_template(...)` for a synchronous call.

Arguments mapping described in
[GetSmsTemplateRequestRequestTypeDef](./type_defs.md#getsmstemplaterequestrequesttypedef).

Keyword-only arguments:

- `TemplateName`: `str` *(required)*
- `Version`: `str`

Returns a `Coroutine` for
[GetSmsTemplateResponseTypeDef](./type_defs.md#getsmstemplateresponsetypedef).

<a id="get_user_endpoints"></a>

### get_user_endpoints

Retrieves information about all the endpoints that are associated with a
specific user ID.

Type annotations for `session.create_client("pinpoint").get_user_endpoints`
method.

Boto3 documentation:
[Pinpoint.Client.get_user_endpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_user_endpoints)

Asynchronous method. Use `await get_user_endpoints(...)` for a synchronous
call.

Arguments mapping described in
[GetUserEndpointsRequestRequestTypeDef](./type_defs.md#getuserendpointsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `UserId`: `str` *(required)*

Returns a `Coroutine` for
[GetUserEndpointsResponseTypeDef](./type_defs.md#getuserendpointsresponsetypedef).

<a id="get_voice_channel"></a>

### get_voice_channel

Retrieves information about the status and settings of the voice channel for an
application.

Type annotations for `session.create_client("pinpoint").get_voice_channel`
method.

Boto3 documentation:
[Pinpoint.Client.get_voice_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_voice_channel)

Asynchronous method. Use `await get_voice_channel(...)` for a synchronous call.

Arguments mapping described in
[GetVoiceChannelRequestRequestTypeDef](./type_defs.md#getvoicechannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetVoiceChannelResponseTypeDef](./type_defs.md#getvoicechannelresponsetypedef).

<a id="get_voice_template"></a>

### get_voice_template

Retrieves the content and settings of a message template for messages that are
sent through the voice channel.

Type annotations for `session.create_client("pinpoint").get_voice_template`
method.

Boto3 documentation:
[Pinpoint.Client.get_voice_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_voice_template)

Asynchronous method. Use `await get_voice_template(...)` for a synchronous
call.

Arguments mapping described in
[GetVoiceTemplateRequestRequestTypeDef](./type_defs.md#getvoicetemplaterequestrequesttypedef).

Keyword-only arguments:

- `TemplateName`: `str` *(required)*
- `Version`: `str`

Returns a `Coroutine` for
[GetVoiceTemplateResponseTypeDef](./type_defs.md#getvoicetemplateresponsetypedef).

<a id="list_journeys"></a>

### list_journeys

Retrieves information about the status, configuration, and other settings for
all the journeys that are associated with an application.

Type annotations for `session.create_client("pinpoint").list_journeys` method.

Boto3 documentation:
[Pinpoint.Client.list_journeys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.list_journeys)

Asynchronous method. Use `await list_journeys(...)` for a synchronous call.

Arguments mapping described in
[ListJourneysRequestRequestTypeDef](./type_defs.md#listjourneysrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `PageSize`: `str`
- `Token`: `str`

Returns a `Coroutine` for
[ListJourneysResponseTypeDef](./type_defs.md#listjourneysresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Retrieves all the tags (keys and values) that are associated with an
application, campaign, message template, or segment.

Type annotations for `session.create_client("pinpoint").list_tags_for_resource`
method.

Boto3 documentation:
[Pinpoint.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="list_template_versions"></a>

### list_template_versions

Retrieves information about all the versions of a specific message template.

Type annotations for `session.create_client("pinpoint").list_template_versions`
method.

Boto3 documentation:
[Pinpoint.Client.list_template_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.list_template_versions)

Asynchronous method. Use `await list_template_versions(...)` for a synchronous
call.

Arguments mapping described in
[ListTemplateVersionsRequestRequestTypeDef](./type_defs.md#listtemplateversionsrequestrequesttypedef).

Keyword-only arguments:

- `TemplateName`: `str` *(required)*
- `TemplateType`: `str` *(required)*
- `NextToken`: `str`
- `PageSize`: `str`

Returns a `Coroutine` for
[ListTemplateVersionsResponseTypeDef](./type_defs.md#listtemplateversionsresponsetypedef).

<a id="list_templates"></a>

### list_templates

Retrieves information about all the message templates that are associated with
your Amazon Pinpoint account.

Type annotations for `session.create_client("pinpoint").list_templates` method.

Boto3 documentation:
[Pinpoint.Client.list_templates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.list_templates)

Asynchronous method. Use `await list_templates(...)` for a synchronous call.

Arguments mapping described in
[ListTemplatesRequestRequestTypeDef](./type_defs.md#listtemplatesrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `PageSize`: `str`
- `Prefix`: `str`
- `TemplateType`: `str`

Returns a `Coroutine` for
[ListTemplatesResponseTypeDef](./type_defs.md#listtemplatesresponsetypedef).

<a id="phone_number_validate"></a>

### phone_number_validate

Retrieves information about a phone number.

Type annotations for `session.create_client("pinpoint").phone_number_validate`
method.

Boto3 documentation:
[Pinpoint.Client.phone_number_validate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.phone_number_validate)

Asynchronous method. Use `await phone_number_validate(...)` for a synchronous
call.

Arguments mapping described in
[PhoneNumberValidateRequestRequestTypeDef](./type_defs.md#phonenumbervalidaterequestrequesttypedef).

Keyword-only arguments:

- `NumberValidateRequest`:
  [NumberValidateRequestTypeDef](./type_defs.md#numbervalidaterequesttypedef)
  *(required)*

Returns a `Coroutine` for
[PhoneNumberValidateResponseTypeDef](./type_defs.md#phonenumbervalidateresponsetypedef).

<a id="put_event_stream"></a>

### put_event_stream

Creates a new event stream for an application or updates the settings of an
existing event stream for an application.

Type annotations for `session.create_client("pinpoint").put_event_stream`
method.

Boto3 documentation:
[Pinpoint.Client.put_event_stream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.put_event_stream)

Asynchronous method. Use `await put_event_stream(...)` for a synchronous call.

Arguments mapping described in
[PutEventStreamRequestRequestTypeDef](./type_defs.md#puteventstreamrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `WriteEventStream`:
  [WriteEventStreamTypeDef](./type_defs.md#writeeventstreamtypedef)
  *(required)*

Returns a `Coroutine` for
[PutEventStreamResponseTypeDef](./type_defs.md#puteventstreamresponsetypedef).

<a id="put_events"></a>

### put_events

Creates a new event to record for endpoints, or creates or updates endpoint
data that existing events are associated with.

Type annotations for `session.create_client("pinpoint").put_events` method.

Boto3 documentation:
[Pinpoint.Client.put_events](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.put_events)

Asynchronous method. Use `await put_events(...)` for a synchronous call.

Arguments mapping described in
[PutEventsRequestRequestTypeDef](./type_defs.md#puteventsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EventsRequest`: [EventsRequestTypeDef](./type_defs.md#eventsrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[PutEventsResponseTypeDef](./type_defs.md#puteventsresponsetypedef).

<a id="remove_attributes"></a>

### remove_attributes

Removes one or more attributes, of the same attribute type, from all the
endpoints that are associated with an application.

Type annotations for `session.create_client("pinpoint").remove_attributes`
method.

Boto3 documentation:
[Pinpoint.Client.remove_attributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.remove_attributes)

Asynchronous method. Use `await remove_attributes(...)` for a synchronous call.

Arguments mapping described in
[RemoveAttributesRequestRequestTypeDef](./type_defs.md#removeattributesrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `AttributeType`: `str` *(required)*
- `UpdateAttributesRequest`:
  [UpdateAttributesRequestTypeDef](./type_defs.md#updateattributesrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[RemoveAttributesResponseTypeDef](./type_defs.md#removeattributesresponsetypedef).

<a id="send_messages"></a>

### send_messages

Creates and sends a direct message.

Type annotations for `session.create_client("pinpoint").send_messages` method.

Boto3 documentation:
[Pinpoint.Client.send_messages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_messages)

Asynchronous method. Use `await send_messages(...)` for a synchronous call.

Arguments mapping described in
[SendMessagesRequestRequestTypeDef](./type_defs.md#sendmessagesrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `MessageRequest`:
  [MessageRequestTypeDef](./type_defs.md#messagerequesttypedef) *(required)*

Returns a `Coroutine` for
[SendMessagesResponseTypeDef](./type_defs.md#sendmessagesresponsetypedef).

<a id="send_otp_message"></a>

### send_otp_message

Send an OTP message See also:
[AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/pinpoint-2016-12-01/SendOTPMessage).

Type annotations for `session.create_client("pinpoint").send_otp_message`
method.

Boto3 documentation:
[Pinpoint.Client.send_otp_message](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_otp_message)

Asynchronous method. Use `await send_otp_message(...)` for a synchronous call.

Arguments mapping described in
[SendOTPMessageRequestRequestTypeDef](./type_defs.md#sendotpmessagerequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `SendOTPMessageRequestParameters`:
  [SendOTPMessageRequestParametersTypeDef](./type_defs.md#sendotpmessagerequestparameterstypedef)
  *(required)*

Returns a `Coroutine` for
[SendOTPMessageResponseTypeDef](./type_defs.md#sendotpmessageresponsetypedef).

<a id="send_users_messages"></a>

### send_users_messages

Creates and sends a message to a list of users.

Type annotations for `session.create_client("pinpoint").send_users_messages`
method.

Boto3 documentation:
[Pinpoint.Client.send_users_messages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_users_messages)

Asynchronous method. Use `await send_users_messages(...)` for a synchronous
call.

Arguments mapping described in
[SendUsersMessagesRequestRequestTypeDef](./type_defs.md#sendusersmessagesrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `SendUsersMessageRequest`:
  [SendUsersMessageRequestTypeDef](./type_defs.md#sendusersmessagerequesttypedef)
  *(required)*

Returns a `Coroutine` for
[SendUsersMessagesResponseTypeDef](./type_defs.md#sendusersmessagesresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Adds one or more tags (keys and values) to an application, campaign, message
template, or segment.

Type annotations for `session.create_client("pinpoint").tag_resource` method.

Boto3 documentation:
[Pinpoint.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagsModel`: [TagsModelTypeDef](./type_defs.md#tagsmodeltypedef) *(required)*

<a id="untag_resource"></a>

### untag_resource

Removes one or more tags (keys and values) from an application, campaign,
message template, or segment.

Type annotations for `session.create_client("pinpoint").untag_resource` method.

Boto3 documentation:
[Pinpoint.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

<a id="update_adm_channel"></a>

### update_adm_channel

Enables the ADM channel for an application or updates the status and settings
of the ADM channel for an application.

Type annotations for `session.create_client("pinpoint").update_adm_channel`
method.

Boto3 documentation:
[Pinpoint.Client.update_adm_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_adm_channel)

Asynchronous method. Use `await update_adm_channel(...)` for a synchronous
call.

Arguments mapping described in
[UpdateAdmChannelRequestRequestTypeDef](./type_defs.md#updateadmchannelrequestrequesttypedef).

Keyword-only arguments:

- `ADMChannelRequest`:
  [ADMChannelRequestTypeDef](./type_defs.md#admchannelrequesttypedef)
  *(required)*
- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[UpdateAdmChannelResponseTypeDef](./type_defs.md#updateadmchannelresponsetypedef).

<a id="update_apns_channel"></a>

### update_apns_channel

Enables the APNs channel for an application or updates the status and settings
of the APNs channel for an application.

Type annotations for `session.create_client("pinpoint").update_apns_channel`
method.

Boto3 documentation:
[Pinpoint.Client.update_apns_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_apns_channel)

Asynchronous method. Use `await update_apns_channel(...)` for a synchronous
call.

Arguments mapping described in
[UpdateApnsChannelRequestRequestTypeDef](./type_defs.md#updateapnschannelrequestrequesttypedef).

Keyword-only arguments:

- `APNSChannelRequest`:
  [APNSChannelRequestTypeDef](./type_defs.md#apnschannelrequesttypedef)
  *(required)*
- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[UpdateApnsChannelResponseTypeDef](./type_defs.md#updateapnschannelresponsetypedef).

<a id="update_apns_sandbox_channel"></a>

### update_apns_sandbox_channel

Enables the APNs sandbox channel for an application or updates the status and
settings of the APNs sandbox channel for an application.

Type annotations for
`session.create_client("pinpoint").update_apns_sandbox_channel` method.

Boto3 documentation:
[Pinpoint.Client.update_apns_sandbox_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_apns_sandbox_channel)

Asynchronous method. Use `await update_apns_sandbox_channel(...)` for a
synchronous call.

Arguments mapping described in
[UpdateApnsSandboxChannelRequestRequestTypeDef](./type_defs.md#updateapnssandboxchannelrequestrequesttypedef).

Keyword-only arguments:

- `APNSSandboxChannelRequest`:
  [APNSSandboxChannelRequestTypeDef](./type_defs.md#apnssandboxchannelrequesttypedef)
  *(required)*
- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[UpdateApnsSandboxChannelResponseTypeDef](./type_defs.md#updateapnssandboxchannelresponsetypedef).

<a id="update_apns_voip_channel"></a>

### update_apns_voip_channel

Enables the APNs VoIP channel for an application or updates the status and
settings of the APNs VoIP channel for an application.

Type annotations for
`session.create_client("pinpoint").update_apns_voip_channel` method.

Boto3 documentation:
[Pinpoint.Client.update_apns_voip_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_apns_voip_channel)

Asynchronous method. Use `await update_apns_voip_channel(...)` for a
synchronous call.

Arguments mapping described in
[UpdateApnsVoipChannelRequestRequestTypeDef](./type_defs.md#updateapnsvoipchannelrequestrequesttypedef).

Keyword-only arguments:

- `APNSVoipChannelRequest`:
  [APNSVoipChannelRequestTypeDef](./type_defs.md#apnsvoipchannelrequesttypedef)
  *(required)*
- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[UpdateApnsVoipChannelResponseTypeDef](./type_defs.md#updateapnsvoipchannelresponsetypedef).

<a id="update_apns_voip_sandbox_channel"></a>

### update_apns_voip_sandbox_channel

Enables the APNs VoIP sandbox channel for an application or updates the status
and settings of the APNs VoIP sandbox channel for an application.

Type annotations for
`session.create_client("pinpoint").update_apns_voip_sandbox_channel` method.

Boto3 documentation:
[Pinpoint.Client.update_apns_voip_sandbox_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_apns_voip_sandbox_channel)

Asynchronous method. Use `await update_apns_voip_sandbox_channel(...)` for a
synchronous call.

Arguments mapping described in
[UpdateApnsVoipSandboxChannelRequestRequestTypeDef](./type_defs.md#updateapnsvoipsandboxchannelrequestrequesttypedef).

Keyword-only arguments:

- `APNSVoipSandboxChannelRequest`:
  [APNSVoipSandboxChannelRequestTypeDef](./type_defs.md#apnsvoipsandboxchannelrequesttypedef)
  *(required)*
- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[UpdateApnsVoipSandboxChannelResponseTypeDef](./type_defs.md#updateapnsvoipsandboxchannelresponsetypedef).

<a id="update_application_settings"></a>

### update_application_settings

Updates the settings for an application.

Type annotations for
`session.create_client("pinpoint").update_application_settings` method.

Boto3 documentation:
[Pinpoint.Client.update_application_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_application_settings)

Asynchronous method. Use `await update_application_settings(...)` for a
synchronous call.

Arguments mapping described in
[UpdateApplicationSettingsRequestRequestTypeDef](./type_defs.md#updateapplicationsettingsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `WriteApplicationSettingsRequest`:
  [WriteApplicationSettingsRequestTypeDef](./type_defs.md#writeapplicationsettingsrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateApplicationSettingsResponseTypeDef](./type_defs.md#updateapplicationsettingsresponsetypedef).

<a id="update_baidu_channel"></a>

### update_baidu_channel

Enables the Baidu channel for an application or updates the status and settings
of the Baidu channel for an application.

Type annotations for `session.create_client("pinpoint").update_baidu_channel`
method.

Boto3 documentation:
[Pinpoint.Client.update_baidu_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_baidu_channel)

Asynchronous method. Use `await update_baidu_channel(...)` for a synchronous
call.

Arguments mapping described in
[UpdateBaiduChannelRequestRequestTypeDef](./type_defs.md#updatebaiduchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `BaiduChannelRequest`:
  [BaiduChannelRequestTypeDef](./type_defs.md#baiduchannelrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateBaiduChannelResponseTypeDef](./type_defs.md#updatebaiduchannelresponsetypedef).

<a id="update_campaign"></a>

### update_campaign

Updates the configuration and other settings for a campaign.

Type annotations for `session.create_client("pinpoint").update_campaign`
method.

Boto3 documentation:
[Pinpoint.Client.update_campaign](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_campaign)

Asynchronous method. Use `await update_campaign(...)` for a synchronous call.

Arguments mapping described in
[UpdateCampaignRequestRequestTypeDef](./type_defs.md#updatecampaignrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `CampaignId`: `str` *(required)*
- `WriteCampaignRequest`:
  [WriteCampaignRequestTypeDef](./type_defs.md#writecampaignrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateCampaignResponseTypeDef](./type_defs.md#updatecampaignresponsetypedef).

<a id="update_email_channel"></a>

### update_email_channel

Enables the email channel for an application or updates the status and settings
of the email channel for an application.

Type annotations for `session.create_client("pinpoint").update_email_channel`
method.

Boto3 documentation:
[Pinpoint.Client.update_email_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_email_channel)

Asynchronous method. Use `await update_email_channel(...)` for a synchronous
call.

Arguments mapping described in
[UpdateEmailChannelRequestRequestTypeDef](./type_defs.md#updateemailchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EmailChannelRequest`:
  [EmailChannelRequestTypeDef](./type_defs.md#emailchannelrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateEmailChannelResponseTypeDef](./type_defs.md#updateemailchannelresponsetypedef).

<a id="update_email_template"></a>

### update_email_template

Updates an existing message template for messages that are sent through the
email channel.

Type annotations for `session.create_client("pinpoint").update_email_template`
method.

Boto3 documentation:
[Pinpoint.Client.update_email_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_email_template)

Asynchronous method. Use `await update_email_template(...)` for a synchronous
call.

Arguments mapping described in
[UpdateEmailTemplateRequestRequestTypeDef](./type_defs.md#updateemailtemplaterequestrequesttypedef).

Keyword-only arguments:

- `EmailTemplateRequest`:
  [EmailTemplateRequestTypeDef](./type_defs.md#emailtemplaterequesttypedef)
  *(required)*
- `TemplateName`: `str` *(required)*
- `CreateNewVersion`: `bool`
- `Version`: `str`

Returns a `Coroutine` for
[UpdateEmailTemplateResponseTypeDef](./type_defs.md#updateemailtemplateresponsetypedef).

<a id="update_endpoint"></a>

### update_endpoint

Creates a new endpoint for an application or updates the settings and
attributes of an existing endpoint for an application.

Type annotations for `session.create_client("pinpoint").update_endpoint`
method.

Boto3 documentation:
[Pinpoint.Client.update_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_endpoint)

Asynchronous method. Use `await update_endpoint(...)` for a synchronous call.

Arguments mapping described in
[UpdateEndpointRequestRequestTypeDef](./type_defs.md#updateendpointrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EndpointId`: `str` *(required)*
- `EndpointRequest`:
  [EndpointRequestTypeDef](./type_defs.md#endpointrequesttypedef) *(required)*

Returns a `Coroutine` for
[UpdateEndpointResponseTypeDef](./type_defs.md#updateendpointresponsetypedef).

<a id="update_endpoints_batch"></a>

### update_endpoints_batch

Creates a new batch of endpoints for an application or updates the settings and
attributes of a batch of existing endpoints for an application.

Type annotations for `session.create_client("pinpoint").update_endpoints_batch`
method.

Boto3 documentation:
[Pinpoint.Client.update_endpoints_batch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_endpoints_batch)

Asynchronous method. Use `await update_endpoints_batch(...)` for a synchronous
call.

Arguments mapping described in
[UpdateEndpointsBatchRequestRequestTypeDef](./type_defs.md#updateendpointsbatchrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EndpointBatchRequest`:
  [EndpointBatchRequestTypeDef](./type_defs.md#endpointbatchrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateEndpointsBatchResponseTypeDef](./type_defs.md#updateendpointsbatchresponsetypedef).

<a id="update_gcm_channel"></a>

### update_gcm_channel

Enables the GCM channel for an application or updates the status and settings
of the GCM channel for an application.

Type annotations for `session.create_client("pinpoint").update_gcm_channel`
method.

Boto3 documentation:
[Pinpoint.Client.update_gcm_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_gcm_channel)

Asynchronous method. Use `await update_gcm_channel(...)` for a synchronous
call.

Arguments mapping described in
[UpdateGcmChannelRequestRequestTypeDef](./type_defs.md#updategcmchannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `GCMChannelRequest`:
  [GCMChannelRequestTypeDef](./type_defs.md#gcmchannelrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateGcmChannelResponseTypeDef](./type_defs.md#updategcmchannelresponsetypedef).

<a id="update_in_app_template"></a>

### update_in_app_template

Updates an existing message template for messages sent through the in-app
message channel.

Type annotations for `session.create_client("pinpoint").update_in_app_template`
method.

Boto3 documentation:
[Pinpoint.Client.update_in_app_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_in_app_template)

Asynchronous method. Use `await update_in_app_template(...)` for a synchronous
call.

Arguments mapping described in
[UpdateInAppTemplateRequestRequestTypeDef](./type_defs.md#updateinapptemplaterequestrequesttypedef).

Keyword-only arguments:

- `InAppTemplateRequest`:
  [InAppTemplateRequestTypeDef](./type_defs.md#inapptemplaterequesttypedef)
  *(required)*
- `TemplateName`: `str` *(required)*
- `CreateNewVersion`: `bool`
- `Version`: `str`

Returns a `Coroutine` for
[UpdateInAppTemplateResponseTypeDef](./type_defs.md#updateinapptemplateresponsetypedef).

<a id="update_journey"></a>

### update_journey

Updates the configuration and other settings for a journey.

Type annotations for `session.create_client("pinpoint").update_journey` method.

Boto3 documentation:
[Pinpoint.Client.update_journey](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_journey)

Asynchronous method. Use `await update_journey(...)` for a synchronous call.

Arguments mapping described in
[UpdateJourneyRequestRequestTypeDef](./type_defs.md#updatejourneyrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `JourneyId`: `str` *(required)*
- `WriteJourneyRequest`:
  [WriteJourneyRequestTypeDef](./type_defs.md#writejourneyrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateJourneyResponseTypeDef](./type_defs.md#updatejourneyresponsetypedef).

<a id="update_journey_state"></a>

### update_journey_state

Cancels (stops) an active journey.

Type annotations for `session.create_client("pinpoint").update_journey_state`
method.

Boto3 documentation:
[Pinpoint.Client.update_journey_state](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_journey_state)

Asynchronous method. Use `await update_journey_state(...)` for a synchronous
call.

Arguments mapping described in
[UpdateJourneyStateRequestRequestTypeDef](./type_defs.md#updatejourneystaterequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `JourneyId`: `str` *(required)*
- `JourneyStateRequest`:
  [JourneyStateRequestTypeDef](./type_defs.md#journeystaterequesttypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateJourneyStateResponseTypeDef](./type_defs.md#updatejourneystateresponsetypedef).

<a id="update_push_template"></a>

### update_push_template

Updates an existing message template for messages that are sent through a push
notification channel.

Type annotations for `session.create_client("pinpoint").update_push_template`
method.

Boto3 documentation:
[Pinpoint.Client.update_push_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_push_template)

Asynchronous method. Use `await update_push_template(...)` for a synchronous
call.

Arguments mapping described in
[UpdatePushTemplateRequestRequestTypeDef](./type_defs.md#updatepushtemplaterequestrequesttypedef).

Keyword-only arguments:

- `PushNotificationTemplateRequest`:
  [PushNotificationTemplateRequestTypeDef](./type_defs.md#pushnotificationtemplaterequesttypedef)
  *(required)*
- `TemplateName`: `str` *(required)*
- `CreateNewVersion`: `bool`
- `Version`: `str`

Returns a `Coroutine` for
[UpdatePushTemplateResponseTypeDef](./type_defs.md#updatepushtemplateresponsetypedef).

<a id="update_recommender_configuration"></a>

### update_recommender_configuration

Updates an Amazon Pinpoint configuration for a recommender model.

Type annotations for
`session.create_client("pinpoint").update_recommender_configuration` method.

Boto3 documentation:
[Pinpoint.Client.update_recommender_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_recommender_configuration)

Asynchronous method. Use `await update_recommender_configuration(...)` for a
synchronous call.

Arguments mapping described in
[UpdateRecommenderConfigurationRequestRequestTypeDef](./type_defs.md#updaterecommenderconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `RecommenderId`: `str` *(required)*
- `UpdateRecommenderConfiguration`:
  [UpdateRecommenderConfigurationTypeDef](./type_defs.md#updaterecommenderconfigurationtypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateRecommenderConfigurationResponseTypeDef](./type_defs.md#updaterecommenderconfigurationresponsetypedef).

<a id="update_segment"></a>

### update_segment

Creates a new segment for an application or updates the configuration,
dimension, and other settings for an existing segment that's associated with an
application.

Type annotations for `session.create_client("pinpoint").update_segment` method.

Boto3 documentation:
[Pinpoint.Client.update_segment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_segment)

Asynchronous method. Use `await update_segment(...)` for a synchronous call.

Arguments mapping described in
[UpdateSegmentRequestRequestTypeDef](./type_defs.md#updatesegmentrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `SegmentId`: `str` *(required)*
- `WriteSegmentRequest`:
  [WriteSegmentRequestTypeDef](./type_defs.md#writesegmentrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateSegmentResponseTypeDef](./type_defs.md#updatesegmentresponsetypedef).

<a id="update_sms_channel"></a>

### update_sms_channel

Enables the SMS channel for an application or updates the status and settings
of the SMS channel for an application.

Type annotations for `session.create_client("pinpoint").update_sms_channel`
method.

Boto3 documentation:
[Pinpoint.Client.update_sms_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_sms_channel)

Asynchronous method. Use `await update_sms_channel(...)` for a synchronous
call.

Arguments mapping described in
[UpdateSmsChannelRequestRequestTypeDef](./type_defs.md#updatesmschannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `SMSChannelRequest`:
  [SMSChannelRequestTypeDef](./type_defs.md#smschannelrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateSmsChannelResponseTypeDef](./type_defs.md#updatesmschannelresponsetypedef).

<a id="update_sms_template"></a>

### update_sms_template

Updates an existing message template for messages that are sent through the SMS
channel.

Type annotations for `session.create_client("pinpoint").update_sms_template`
method.

Boto3 documentation:
[Pinpoint.Client.update_sms_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_sms_template)

Asynchronous method. Use `await update_sms_template(...)` for a synchronous
call.

Arguments mapping described in
[UpdateSmsTemplateRequestRequestTypeDef](./type_defs.md#updatesmstemplaterequestrequesttypedef).

Keyword-only arguments:

- `SMSTemplateRequest`:
  [SMSTemplateRequestTypeDef](./type_defs.md#smstemplaterequesttypedef)
  *(required)*
- `TemplateName`: `str` *(required)*
- `CreateNewVersion`: `bool`
- `Version`: `str`

Returns a `Coroutine` for
[UpdateSmsTemplateResponseTypeDef](./type_defs.md#updatesmstemplateresponsetypedef).

<a id="update_template_active_version"></a>

### update_template_active_version

Changes the status of a specific version of a message template to *active* .

Type annotations for
`session.create_client("pinpoint").update_template_active_version` method.

Boto3 documentation:
[Pinpoint.Client.update_template_active_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_template_active_version)

Asynchronous method. Use `await update_template_active_version(...)` for a
synchronous call.

Arguments mapping described in
[UpdateTemplateActiveVersionRequestRequestTypeDef](./type_defs.md#updatetemplateactiveversionrequestrequesttypedef).

Keyword-only arguments:

- `TemplateActiveVersionRequest`:
  [TemplateActiveVersionRequestTypeDef](./type_defs.md#templateactiveversionrequesttypedef)
  *(required)*
- `TemplateName`: `str` *(required)*
- `TemplateType`: `str` *(required)*

Returns a `Coroutine` for
[UpdateTemplateActiveVersionResponseTypeDef](./type_defs.md#updatetemplateactiveversionresponsetypedef).

<a id="update_voice_channel"></a>

### update_voice_channel

Enables the voice channel for an application or updates the status and settings
of the voice channel for an application.

Type annotations for `session.create_client("pinpoint").update_voice_channel`
method.

Boto3 documentation:
[Pinpoint.Client.update_voice_channel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_voice_channel)

Asynchronous method. Use `await update_voice_channel(...)` for a synchronous
call.

Arguments mapping described in
[UpdateVoiceChannelRequestRequestTypeDef](./type_defs.md#updatevoicechannelrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `VoiceChannelRequest`:
  [VoiceChannelRequestTypeDef](./type_defs.md#voicechannelrequesttypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateVoiceChannelResponseTypeDef](./type_defs.md#updatevoicechannelresponsetypedef).

<a id="update_voice_template"></a>

### update_voice_template

Updates an existing message template for messages that are sent through the
voice channel.

Type annotations for `session.create_client("pinpoint").update_voice_template`
method.

Boto3 documentation:
[Pinpoint.Client.update_voice_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_voice_template)

Asynchronous method. Use `await update_voice_template(...)` for a synchronous
call.

Arguments mapping described in
[UpdateVoiceTemplateRequestRequestTypeDef](./type_defs.md#updatevoicetemplaterequestrequesttypedef).

Keyword-only arguments:

- `TemplateName`: `str` *(required)*
- `VoiceTemplateRequest`:
  [VoiceTemplateRequestTypeDef](./type_defs.md#voicetemplaterequesttypedef)
  *(required)*
- `CreateNewVersion`: `bool`
- `Version`: `str`

Returns a `Coroutine` for
[UpdateVoiceTemplateResponseTypeDef](./type_defs.md#updatevoicetemplateresponsetypedef).

<a id="verify_otp_message"></a>

### verify_otp_message

Verify an OTP See also:
[AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/pinpoint-2016-12-01/VerifyOTPMessage).

Type annotations for `session.create_client("pinpoint").verify_otp_message`
method.

Boto3 documentation:
[Pinpoint.Client.verify_otp_message](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.verify_otp_message)

Asynchronous method. Use `await verify_otp_message(...)` for a synchronous
call.

Arguments mapping described in
[VerifyOTPMessageRequestRequestTypeDef](./type_defs.md#verifyotpmessagerequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `VerifyOTPMessageRequestParameters`:
  [VerifyOTPMessageRequestParametersTypeDef](./type_defs.md#verifyotpmessagerequestparameterstypedef)
  *(required)*

Returns a `Coroutine` for
[VerifyOTPMessageResponseTypeDef](./type_defs.md#verifyotpmessageresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("pinpoint").__aenter__` method.

Boto3 documentation:
[Pinpoint.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [PinpointClient](#pinpointclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("pinpoint").__aexit__` method.

Boto3 documentation:
[Pinpoint.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
