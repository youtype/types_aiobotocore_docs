<a id="mediaconvertclient-for-aiobotocore-mediaconvert-module"></a>

# MediaConvertClient for aiobotocore MediaConvert module

> [Index](..) > [MediaConvert](.) > MediaConvertClient

Auto-generated documentation for
[MediaConvert](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
type annotations stubs module
[types-aiobotocore-mediaconvert](https://pypi.org/project/types-aiobotocore-mediaconvert/).

- [MediaConvertClient for aiobotocore MediaConvert module](#mediaconvertclient-for-aiobotocore-mediaconvert-module)
  - [MediaConvertClient](#mediaconvertclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [associate_certificate](#associate_certificate)
    - [can_paginate](#can_paginate)
    - [cancel_job](#cancel_job)
    - [create_job](#create_job)
    - [create_job_template](#create_job_template)
    - [create_preset](#create_preset)
    - [create_queue](#create_queue)
    - [delete_job_template](#delete_job_template)
    - [delete_policy](#delete_policy)
    - [delete_preset](#delete_preset)
    - [delete_queue](#delete_queue)
    - [describe_endpoints](#describe_endpoints)
    - [disassociate_certificate](#disassociate_certificate)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_job](#get_job)
    - [get_job_template](#get_job_template)
    - [get_policy](#get_policy)
    - [get_preset](#get_preset)
    - [get_queue](#get_queue)
    - [list_job_templates](#list_job_templates)
    - [list_jobs](#list_jobs)
    - [list_presets](#list_presets)
    - [list_queues](#list_queues)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [put_policy](#put_policy)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_job_template](#update_job_template)
    - [update_preset](#update_preset)
    - [update_queue](#update_queue)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="mediaconvertclient"></a>

## MediaConvertClient

Type annotations for `session.create_client("mediaconvert")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_mediaconvert.client import MediaConvertClient

session = get_session()
async with session.create_client("mediaconvert") as client:
    client: MediaConvertClient
```

Boto3 documentation:
[MediaConvert.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_mediaconvert.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.ForbiddenException`
- `Exceptions.InternalServerErrorException`
- `Exceptions.NotFoundException`
- `Exceptions.TooManyRequestsException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

MediaConvertClient exceptions.

Type annotations for `session.create_client("mediaconvert").exceptions` method.

Boto3 documentation:
[MediaConvert.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="associate_certificate"></a>

### associate_certificate

Associates an AWS Certificate Manager (ACM) Amazon Resource Name (ARN) with AWS
Elemental MediaConvert.

Type annotations for
`session.create_client("mediaconvert").associate_certificate` method.

Boto3 documentation:
[MediaConvert.Client.associate_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.associate_certificate)

Asynchronous method. Use `await associate_certificate(...)` for a synchronous
call.

Arguments mapping described in
[AssociateCertificateRequestRequestTypeDef](./type_defs.md#associatecertificaterequestrequesttypedef).

Keyword-only arguments:

- `Arn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("mediaconvert").can_paginate`
method.

Boto3 documentation:
[MediaConvert.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel_job"></a>

### cancel_job

Permanently cancel a job.

Type annotations for `session.create_client("mediaconvert").cancel_job` method.

Boto3 documentation:
[MediaConvert.Client.cancel_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.cancel_job)

Asynchronous method. Use `await cancel_job(...)` for a synchronous call.

Arguments mapping described in
[CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="create_job"></a>

### create_job

Create a new transcoding job.

Type annotations for `session.create_client("mediaconvert").create_job` method.

Boto3 documentation:
[MediaConvert.Client.create_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_job)

Asynchronous method. Use `await create_job(...)` for a synchronous call.

Arguments mapping described in
[CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef).

Keyword-only arguments:

- `Role`: `str` *(required)*
- `Settings`: [JobSettingsTypeDef](./type_defs.md#jobsettingstypedef)
  *(required)*
- `AccelerationSettings`:
  [AccelerationSettingsTypeDef](./type_defs.md#accelerationsettingstypedef)
- `BillingTagsSource`:
  [BillingTagsSourceType](./literals.md#billingtagssourcetype)
- `ClientRequestToken`: `str`
- `HopDestinations`:
  `Sequence`\[[HopDestinationTypeDef](./type_defs.md#hopdestinationtypedef)\]
- `JobTemplate`: `str`
- `Priority`: `int`
- `Queue`: `str`
- `SimulateReservedQueue`:
  [SimulateReservedQueueType](./literals.md#simulatereservedqueuetype)
- `StatusUpdateInterval`:
  [StatusUpdateIntervalType](./literals.md#statusupdateintervaltype)
- `Tags`: `Mapping`\[`str`, `str`\]
- `UserMetadata`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef).

<a id="create_job_template"></a>

### create_job_template

Create a new job template.

Type annotations for
`session.create_client("mediaconvert").create_job_template` method.

Boto3 documentation:
[MediaConvert.Client.create_job_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_job_template)

Asynchronous method. Use `await create_job_template(...)` for a synchronous
call.

Arguments mapping described in
[CreateJobTemplateRequestRequestTypeDef](./type_defs.md#createjobtemplaterequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Settings`:
  [JobTemplateSettingsTypeDef](./type_defs.md#jobtemplatesettingstypedef)
  *(required)*
- `AccelerationSettings`:
  [AccelerationSettingsTypeDef](./type_defs.md#accelerationsettingstypedef)
- `Category`: `str`
- `Description`: `str`
- `HopDestinations`:
  `Sequence`\[[HopDestinationTypeDef](./type_defs.md#hopdestinationtypedef)\]
- `Priority`: `int`
- `Queue`: `str`
- `StatusUpdateInterval`:
  [StatusUpdateIntervalType](./literals.md#statusupdateintervaltype)
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateJobTemplateResponseTypeDef](./type_defs.md#createjobtemplateresponsetypedef).

<a id="create_preset"></a>

### create_preset

Create a new preset.

Type annotations for `session.create_client("mediaconvert").create_preset`
method.

Boto3 documentation:
[MediaConvert.Client.create_preset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_preset)

Asynchronous method. Use `await create_preset(...)` for a synchronous call.

Arguments mapping described in
[CreatePresetRequestRequestTypeDef](./type_defs.md#createpresetrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Settings`: [PresetSettingsTypeDef](./type_defs.md#presetsettingstypedef)
  *(required)*
- `Category`: `str`
- `Description`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreatePresetResponseTypeDef](./type_defs.md#createpresetresponsetypedef).

<a id="create_queue"></a>

### create_queue

Create a new transcoding queue.

Type annotations for `session.create_client("mediaconvert").create_queue`
method.

Boto3 documentation:
[MediaConvert.Client.create_queue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_queue)

Asynchronous method. Use `await create_queue(...)` for a synchronous call.

Arguments mapping described in
[CreateQueueRequestRequestTypeDef](./type_defs.md#createqueuerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Description`: `str`
- `PricingPlan`: [PricingPlanType](./literals.md#pricingplantype)
- `ReservationPlanSettings`:
  [ReservationPlanSettingsTypeDef](./type_defs.md#reservationplansettingstypedef)
- `Status`: [QueueStatusType](./literals.md#queuestatustype)
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateQueueResponseTypeDef](./type_defs.md#createqueueresponsetypedef).

<a id="delete_job_template"></a>

### delete_job_template

Permanently delete a job template you have created.

Type annotations for
`session.create_client("mediaconvert").delete_job_template` method.

Boto3 documentation:
[MediaConvert.Client.delete_job_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.delete_job_template)

Asynchronous method. Use `await delete_job_template(...)` for a synchronous
call.

Arguments mapping described in
[DeleteJobTemplateRequestRequestTypeDef](./type_defs.md#deletejobtemplaterequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_policy"></a>

### delete_policy

Permanently delete a policy that you created.

Type annotations for `session.create_client("mediaconvert").delete_policy`
method.

Boto3 documentation:
[MediaConvert.Client.delete_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.delete_policy)

Asynchronous method. Use `await delete_policy(...)` for a synchronous call.

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_preset"></a>

### delete_preset

Permanently delete a preset you have created.

Type annotations for `session.create_client("mediaconvert").delete_preset`
method.

Boto3 documentation:
[MediaConvert.Client.delete_preset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.delete_preset)

Asynchronous method. Use `await delete_preset(...)` for a synchronous call.

Arguments mapping described in
[DeletePresetRequestRequestTypeDef](./type_defs.md#deletepresetrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_queue"></a>

### delete_queue

Permanently delete a queue you have created.

Type annotations for `session.create_client("mediaconvert").delete_queue`
method.

Boto3 documentation:
[MediaConvert.Client.delete_queue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.delete_queue)

Asynchronous method. Use `await delete_queue(...)` for a synchronous call.

Arguments mapping described in
[DeleteQueueRequestRequestTypeDef](./type_defs.md#deletequeuerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_endpoints"></a>

### describe_endpoints

Send an request with an empty body to the regional API endpoint to get your
account API endpoint.

Type annotations for `session.create_client("mediaconvert").describe_endpoints`
method.

Boto3 documentation:
[MediaConvert.Client.describe_endpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.describe_endpoints)

Asynchronous method. Use `await describe_endpoints(...)` for a synchronous
call.

Arguments mapping described in
[DescribeEndpointsRequestRequestTypeDef](./type_defs.md#describeendpointsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `Mode`: [DescribeEndpointsModeType](./literals.md#describeendpointsmodetype)
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef).

<a id="disassociate_certificate"></a>

### disassociate_certificate

Removes an association between the Amazon Resource Name (ARN) of an AWS
Certificate Manager (ACM) certificate and an AWS Elemental MediaConvert
resource.

Type annotations for
`session.create_client("mediaconvert").disassociate_certificate` method.

Boto3 documentation:
[MediaConvert.Client.disassociate_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.disassociate_certificate)

Asynchronous method. Use `await disassociate_certificate(...)` for a
synchronous call.

Arguments mapping described in
[DisassociateCertificateRequestRequestTypeDef](./type_defs.md#disassociatecertificaterequestrequesttypedef).

Keyword-only arguments:

- `Arn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("mediaconvert").generate_presigned_url` method.

Boto3 documentation:
[MediaConvert.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_job"></a>

### get_job

Retrieve the JSON for a specific completed transcoding job.

Type annotations for `session.create_client("mediaconvert").get_job` method.

Boto3 documentation:
[MediaConvert.Client.get_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.get_job)

Asynchronous method. Use `await get_job(...)` for a synchronous call.

Arguments mapping described in
[GetJobRequestRequestTypeDef](./type_defs.md#getjobrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetJobResponseTypeDef](./type_defs.md#getjobresponsetypedef).

<a id="get_job_template"></a>

### get_job_template

Retrieve the JSON for a specific job template.

Type annotations for `session.create_client("mediaconvert").get_job_template`
method.

Boto3 documentation:
[MediaConvert.Client.get_job_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.get_job_template)

Asynchronous method. Use `await get_job_template(...)` for a synchronous call.

Arguments mapping described in
[GetJobTemplateRequestRequestTypeDef](./type_defs.md#getjobtemplaterequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[GetJobTemplateResponseTypeDef](./type_defs.md#getjobtemplateresponsetypedef).

<a id="get_policy"></a>

### get_policy

Retrieve the JSON for your policy.

Type annotations for `session.create_client("mediaconvert").get_policy` method.

Boto3 documentation:
[MediaConvert.Client.get_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.get_policy)

Asynchronous method. Use `await get_policy(...)` for a synchronous call.

Returns a `Coroutine` for
[GetPolicyResponseTypeDef](./type_defs.md#getpolicyresponsetypedef).

<a id="get_preset"></a>

### get_preset

Retrieve the JSON for a specific preset.

Type annotations for `session.create_client("mediaconvert").get_preset` method.

Boto3 documentation:
[MediaConvert.Client.get_preset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.get_preset)

Asynchronous method. Use `await get_preset(...)` for a synchronous call.

Arguments mapping described in
[GetPresetRequestRequestTypeDef](./type_defs.md#getpresetrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[GetPresetResponseTypeDef](./type_defs.md#getpresetresponsetypedef).

<a id="get_queue"></a>

### get_queue

Retrieve the JSON for a specific queue.

Type annotations for `session.create_client("mediaconvert").get_queue` method.

Boto3 documentation:
[MediaConvert.Client.get_queue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.get_queue)

Asynchronous method. Use `await get_queue(...)` for a synchronous call.

Arguments mapping described in
[GetQueueRequestRequestTypeDef](./type_defs.md#getqueuerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[GetQueueResponseTypeDef](./type_defs.md#getqueueresponsetypedef).

<a id="list_job_templates"></a>

### list_job_templates

Retrieve a JSON array of up to twenty of your job templates.

Type annotations for `session.create_client("mediaconvert").list_job_templates`
method.

Boto3 documentation:
[MediaConvert.Client.list_job_templates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.list_job_templates)

Asynchronous method. Use `await list_job_templates(...)` for a synchronous
call.

Arguments mapping described in
[ListJobTemplatesRequestRequestTypeDef](./type_defs.md#listjobtemplatesrequestrequesttypedef).

Keyword-only arguments:

- `Category`: `str`
- `ListBy`: [JobTemplateListByType](./literals.md#jobtemplatelistbytype)
- `MaxResults`: `int`
- `NextToken`: `str`
- `Order`: [OrderType](./literals.md#ordertype)

Returns a `Coroutine` for
[ListJobTemplatesResponseTypeDef](./type_defs.md#listjobtemplatesresponsetypedef).

<a id="list_jobs"></a>

### list_jobs

Retrieve a JSON array of up to twenty of your most recently created jobs.

Type annotations for `session.create_client("mediaconvert").list_jobs` method.

Boto3 documentation:
[MediaConvert.Client.list_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.list_jobs)

Asynchronous method. Use `await list_jobs(...)` for a synchronous call.

Arguments mapping described in
[ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`
- `Order`: [OrderType](./literals.md#ordertype)
- `Queue`: `str`
- `Status`: [JobStatusType](./literals.md#jobstatustype)

Returns a `Coroutine` for
[ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef).

<a id="list_presets"></a>

### list_presets

Retrieve a JSON array of up to twenty of your presets.

Type annotations for `session.create_client("mediaconvert").list_presets`
method.

Boto3 documentation:
[MediaConvert.Client.list_presets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.list_presets)

Asynchronous method. Use `await list_presets(...)` for a synchronous call.

Arguments mapping described in
[ListPresetsRequestRequestTypeDef](./type_defs.md#listpresetsrequestrequesttypedef).

Keyword-only arguments:

- `Category`: `str`
- `ListBy`: [PresetListByType](./literals.md#presetlistbytype)
- `MaxResults`: `int`
- `NextToken`: `str`
- `Order`: [OrderType](./literals.md#ordertype)

Returns a `Coroutine` for
[ListPresetsResponseTypeDef](./type_defs.md#listpresetsresponsetypedef).

<a id="list_queues"></a>

### list_queues

Retrieve a JSON array of up to twenty of your queues.

Type annotations for `session.create_client("mediaconvert").list_queues`
method.

Boto3 documentation:
[MediaConvert.Client.list_queues](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.list_queues)

Asynchronous method. Use `await list_queues(...)` for a synchronous call.

Arguments mapping described in
[ListQueuesRequestRequestTypeDef](./type_defs.md#listqueuesrequestrequesttypedef).

Keyword-only arguments:

- `ListBy`: [QueueListByType](./literals.md#queuelistbytype)
- `MaxResults`: `int`
- `NextToken`: `str`
- `Order`: [OrderType](./literals.md#ordertype)

Returns a `Coroutine` for
[ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Retrieve the tags for a MediaConvert resource.

Type annotations for
`session.create_client("mediaconvert").list_tags_for_resource` method.

Boto3 documentation:
[MediaConvert.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `Arn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="put_policy"></a>

### put_policy

Create or change your policy.

Type annotations for `session.create_client("mediaconvert").put_policy` method.

Boto3 documentation:
[MediaConvert.Client.put_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.put_policy)

Asynchronous method. Use `await put_policy(...)` for a synchronous call.

Arguments mapping described in
[PutPolicyRequestRequestTypeDef](./type_defs.md#putpolicyrequestrequesttypedef).

Keyword-only arguments:

- `Policy`: [PolicyTypeDef](./type_defs.md#policytypedef) *(required)*

Returns a `Coroutine` for
[PutPolicyResponseTypeDef](./type_defs.md#putpolicyresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Add tags to a MediaConvert queue, preset, or job template.

Type annotations for `session.create_client("mediaconvert").tag_resource`
method.

Boto3 documentation:
[MediaConvert.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `Arn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Remove tags from a MediaConvert queue, preset, or job template.

Type annotations for `session.create_client("mediaconvert").untag_resource`
method.

Boto3 documentation:
[MediaConvert.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `Arn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_job_template"></a>

### update_job_template

Modify one of your existing job templates.

Type annotations for
`session.create_client("mediaconvert").update_job_template` method.

Boto3 documentation:
[MediaConvert.Client.update_job_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_job_template)

Asynchronous method. Use `await update_job_template(...)` for a synchronous
call.

Arguments mapping described in
[UpdateJobTemplateRequestRequestTypeDef](./type_defs.md#updatejobtemplaterequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `AccelerationSettings`:
  [AccelerationSettingsTypeDef](./type_defs.md#accelerationsettingstypedef)
- `Category`: `str`
- `Description`: `str`
- `HopDestinations`:
  `Sequence`\[[HopDestinationTypeDef](./type_defs.md#hopdestinationtypedef)\]
- `Priority`: `int`
- `Queue`: `str`
- `Settings`:
  [JobTemplateSettingsTypeDef](./type_defs.md#jobtemplatesettingstypedef)
- `StatusUpdateInterval`:
  [StatusUpdateIntervalType](./literals.md#statusupdateintervaltype)

Returns a `Coroutine` for
[UpdateJobTemplateResponseTypeDef](./type_defs.md#updatejobtemplateresponsetypedef).

<a id="update_preset"></a>

### update_preset

Modify one of your existing presets.

Type annotations for `session.create_client("mediaconvert").update_preset`
method.

Boto3 documentation:
[MediaConvert.Client.update_preset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_preset)

Asynchronous method. Use `await update_preset(...)` for a synchronous call.

Arguments mapping described in
[UpdatePresetRequestRequestTypeDef](./type_defs.md#updatepresetrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Category`: `str`
- `Description`: `str`
- `Settings`: [PresetSettingsTypeDef](./type_defs.md#presetsettingstypedef)

Returns a `Coroutine` for
[UpdatePresetResponseTypeDef](./type_defs.md#updatepresetresponsetypedef).

<a id="update_queue"></a>

### update_queue

Modify one of your existing queues.

Type annotations for `session.create_client("mediaconvert").update_queue`
method.

Boto3 documentation:
[MediaConvert.Client.update_queue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_queue)

Asynchronous method. Use `await update_queue(...)` for a synchronous call.

Arguments mapping described in
[UpdateQueueRequestRequestTypeDef](./type_defs.md#updatequeuerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Description`: `str`
- `ReservationPlanSettings`:
  [ReservationPlanSettingsTypeDef](./type_defs.md#reservationplansettingstypedef)
- `Status`: [QueueStatusType](./literals.md#queuestatustype)

Returns a `Coroutine` for
[UpdateQueueResponseTypeDef](./type_defs.md#updatequeueresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("mediaconvert").__aenter__` method.

Boto3 documentation:
[MediaConvert.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [MediaConvertClient](#mediaconvertclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("mediaconvert").__aexit__` method.

Boto3 documentation:
[MediaConvert.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("mediaconvert").get_paginator`
method with overloads.

- `client.get_paginator("describe_endpoints")` ->
  [DescribeEndpointsPaginator](./paginators.md#describeendpointspaginator)
- `client.get_paginator("list_job_templates")` ->
  [ListJobTemplatesPaginator](./paginators.md#listjobtemplatespaginator)
- `client.get_paginator("list_jobs")` ->
  [ListJobsPaginator](./paginators.md#listjobspaginator)
- `client.get_paginator("list_presets")` ->
  [ListPresetsPaginator](./paginators.md#listpresetspaginator)
- `client.get_paginator("list_queues")` ->
  [ListQueuesPaginator](./paginators.md#listqueuespaginator)
