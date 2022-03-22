<a id="kinesisanalyticsclient-for-aiobotocore-kinesisanalytics-module"></a>

# KinesisAnalyticsClient for aiobotocore KinesisAnalytics module

> [Index](../README.md) > [KinesisAnalytics](./README.md) >
> KinesisAnalyticsClient

Auto-generated documentation for
[KinesisAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
type annotations stubs module
[types-aiobotocore-kinesisanalytics](https://pypi.org/project/types-aiobotocore-kinesisanalytics/).

- [KinesisAnalyticsClient for aiobotocore KinesisAnalytics module](#kinesisanalyticsclient-for-aiobotocore-kinesisanalytics-module)
  - [KinesisAnalyticsClient](#kinesisanalyticsclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [add_application_cloud_watch_logging_option](#add_application_cloud_watch_logging_option)
    - [add_application_input](#add_application_input)
    - [add_application_input_processing_configuration](#add_application_input_processing_configuration)
    - [add_application_output](#add_application_output)
    - [add_application_reference_data_source](#add_application_reference_data_source)
    - [can_paginate](#can_paginate)
    - [create_application](#create_application)
    - [delete_application](#delete_application)
    - [delete_application_cloud_watch_logging_option](#delete_application_cloud_watch_logging_option)
    - [delete_application_input_processing_configuration](#delete_application_input_processing_configuration)
    - [delete_application_output](#delete_application_output)
    - [delete_application_reference_data_source](#delete_application_reference_data_source)
    - [describe_application](#describe_application)
    - [discover_input_schema](#discover_input_schema)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_applications](#list_applications)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [start_application](#start_application)
    - [stop_application](#stop_application)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_application](#update_application)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="kinesisanalyticsclient"></a>

## KinesisAnalyticsClient

Type annotations for `session.create_client("kinesisanalytics")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_kinesisanalytics.client import KinesisAnalyticsClient

session = get_session()
async with session.create_client("kinesisanalytics") as client:
    client: KinesisAnalyticsClient
```

Boto3 documentation:
[KinesisAnalytics.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_kinesisanalytics.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.CodeValidationException`
- `Exceptions.ConcurrentModificationException`
- `Exceptions.InvalidApplicationConfigurationException`
- `Exceptions.InvalidArgumentException`
- `Exceptions.LimitExceededException`
- `Exceptions.ResourceInUseException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ResourceProvisionedThroughputExceededException`
- `Exceptions.ServiceUnavailableException`
- `Exceptions.TooManyTagsException`
- `Exceptions.UnableToDetectSchemaException`
- `Exceptions.UnsupportedOperationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

KinesisAnalyticsClient exceptions.

Type annotations for `session.create_client("kinesisanalytics").exceptions`
method.

Boto3 documentation:
[KinesisAnalytics.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="add\_application\_cloud\_watch\_logging\_option"></a>

### add_application_cloud_watch_logging_option

.

Type annotations for
`session.create_client("kinesisanalytics").add_application_cloud_watch_logging_option`
method.

Boto3 documentation:
[KinesisAnalytics.Client.add_application_cloud_watch_logging_option](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.add_application_cloud_watch_logging_option)

Asynchronous method. Use
`await add_application_cloud_watch_logging_option(...)` for a synchronous call.

Arguments mapping described in
[AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef](./type_defs.md#addapplicationcloudwatchloggingoptionrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*
- `CurrentApplicationVersionId`: `int` *(required)*
- `CloudWatchLoggingOption`:
  [CloudWatchLoggingOptionTypeDef](./type_defs.md#cloudwatchloggingoptiontypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="add\_application\_input"></a>

### add_application_input

.

Type annotations for
`session.create_client("kinesisanalytics").add_application_input` method.

Boto3 documentation:
[KinesisAnalytics.Client.add_application_input](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.add_application_input)

Asynchronous method. Use `await add_application_input(...)` for a synchronous
call.

Arguments mapping described in
[AddApplicationInputRequestRequestTypeDef](./type_defs.md#addapplicationinputrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*
- `CurrentApplicationVersionId`: `int` *(required)*
- `Input`: [InputTypeDef](./type_defs.md#inputtypedef) *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="add\_application\_input\_processing\_configuration"></a>

### add_application_input_processing_configuration

.

Type annotations for
`session.create_client("kinesisanalytics").add_application_input_processing_configuration`
method.

Boto3 documentation:
[KinesisAnalytics.Client.add_application_input_processing_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.add_application_input_processing_configuration)

Asynchronous method. Use
`await add_application_input_processing_configuration(...)` for a synchronous
call.

Arguments mapping described in
[AddApplicationInputProcessingConfigurationRequestRequestTypeDef](./type_defs.md#addapplicationinputprocessingconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*
- `CurrentApplicationVersionId`: `int` *(required)*
- `InputId`: `str` *(required)*
- `InputProcessingConfiguration`:
  [InputProcessingConfigurationTypeDef](./type_defs.md#inputprocessingconfigurationtypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="add\_application\_output"></a>

### add_application_output

.

Type annotations for
`session.create_client("kinesisanalytics").add_application_output` method.

Boto3 documentation:
[KinesisAnalytics.Client.add_application_output](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.add_application_output)

Asynchronous method. Use `await add_application_output(...)` for a synchronous
call.

Arguments mapping described in
[AddApplicationOutputRequestRequestTypeDef](./type_defs.md#addapplicationoutputrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*
- `CurrentApplicationVersionId`: `int` *(required)*
- `Output`: [OutputTypeDef](./type_defs.md#outputtypedef) *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="add\_application\_reference\_data\_source"></a>

### add_application_reference_data_source

.

Type annotations for
`session.create_client("kinesisanalytics").add_application_reference_data_source`
method.

Boto3 documentation:
[KinesisAnalytics.Client.add_application_reference_data_source](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.add_application_reference_data_source)

Asynchronous method. Use `await add_application_reference_data_source(...)` for
a synchronous call.

Arguments mapping described in
[AddApplicationReferenceDataSourceRequestRequestTypeDef](./type_defs.md#addapplicationreferencedatasourcerequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*
- `CurrentApplicationVersionId`: `int` *(required)*
- `ReferenceDataSource`:
  [ReferenceDataSourceTypeDef](./type_defs.md#referencedatasourcetypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("kinesisanalytics").can_paginate`
method.

Boto3 documentation:
[KinesisAnalytics.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_application"></a>

### create_application

.

Type annotations for
`session.create_client("kinesisanalytics").create_application` method.

Boto3 documentation:
[KinesisAnalytics.Client.create_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.create_application)

Asynchronous method. Use `await create_application(...)` for a synchronous
call.

Arguments mapping described in
[CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*
- `ApplicationDescription`: `str`
- `Inputs`: `Sequence`\[[InputTypeDef](./type_defs.md#inputtypedef)\]
- `Outputs`: `Sequence`\[[OutputTypeDef](./type_defs.md#outputtypedef)\]
- `CloudWatchLoggingOptions`:
  `Sequence`\[[CloudWatchLoggingOptionTypeDef](./type_defs.md#cloudwatchloggingoptiontypedef)\]
- `ApplicationCode`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef).

<a id="delete\_application"></a>

### delete_application

.

Type annotations for
`session.create_client("kinesisanalytics").delete_application` method.

Boto3 documentation:
[KinesisAnalytics.Client.delete_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.delete_application)

Asynchronous method. Use `await delete_application(...)` for a synchronous
call.

Arguments mapping described in
[DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*
- `CreateTimestamp`: `Union`\[`datetime`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_application\_cloud\_watch\_logging\_option"></a>

### delete_application_cloud_watch_logging_option

.

Type annotations for
`session.create_client("kinesisanalytics").delete_application_cloud_watch_logging_option`
method.

Boto3 documentation:
[KinesisAnalytics.Client.delete_application_cloud_watch_logging_option](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.delete_application_cloud_watch_logging_option)

Asynchronous method. Use
`await delete_application_cloud_watch_logging_option(...)` for a synchronous
call.

Arguments mapping described in
[DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef](./type_defs.md#deleteapplicationcloudwatchloggingoptionrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*
- `CurrentApplicationVersionId`: `int` *(required)*
- `CloudWatchLoggingOptionId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_application\_input\_processing\_configuration"></a>

### delete_application_input_processing_configuration

.

Type annotations for
`session.create_client("kinesisanalytics").delete_application_input_processing_configuration`
method.

Boto3 documentation:
[KinesisAnalytics.Client.delete_application_input_processing_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.delete_application_input_processing_configuration)

Asynchronous method. Use
`await delete_application_input_processing_configuration(...)` for a
synchronous call.

Arguments mapping described in
[DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef](./type_defs.md#deleteapplicationinputprocessingconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*
- `CurrentApplicationVersionId`: `int` *(required)*
- `InputId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_application\_output"></a>

### delete_application_output

.

Type annotations for
`session.create_client("kinesisanalytics").delete_application_output` method.

Boto3 documentation:
[KinesisAnalytics.Client.delete_application_output](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.delete_application_output)

Asynchronous method. Use `await delete_application_output(...)` for a
synchronous call.

Arguments mapping described in
[DeleteApplicationOutputRequestRequestTypeDef](./type_defs.md#deleteapplicationoutputrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*
- `CurrentApplicationVersionId`: `int` *(required)*
- `OutputId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_application\_reference\_data\_source"></a>

### delete_application_reference_data_source

.

Type annotations for
`session.create_client("kinesisanalytics").delete_application_reference_data_source`
method.

Boto3 documentation:
[KinesisAnalytics.Client.delete_application_reference_data_source](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.delete_application_reference_data_source)

Asynchronous method. Use `await delete_application_reference_data_source(...)`
for a synchronous call.

Arguments mapping described in
[DeleteApplicationReferenceDataSourceRequestRequestTypeDef](./type_defs.md#deleteapplicationreferencedatasourcerequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*
- `CurrentApplicationVersionId`: `int` *(required)*
- `ReferenceId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe\_application"></a>

### describe_application

.

Type annotations for
`session.create_client("kinesisanalytics").describe_application` method.

Boto3 documentation:
[KinesisAnalytics.Client.describe_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.describe_application)

Asynchronous method. Use `await describe_application(...)` for a synchronous
call.

Arguments mapping described in
[DescribeApplicationRequestRequestTypeDef](./type_defs.md#describeapplicationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeApplicationResponseTypeDef](./type_defs.md#describeapplicationresponsetypedef).

<a id="discover\_input\_schema"></a>

### discover_input_schema

.

Type annotations for
`session.create_client("kinesisanalytics").discover_input_schema` method.

Boto3 documentation:
[KinesisAnalytics.Client.discover_input_schema](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.discover_input_schema)

Asynchronous method. Use `await discover_input_schema(...)` for a synchronous
call.

Arguments mapping described in
[DiscoverInputSchemaRequestRequestTypeDef](./type_defs.md#discoverinputschemarequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str`
- `RoleARN`: `str`
- `InputStartingPositionConfiguration`:
  [InputStartingPositionConfigurationTypeDef](./type_defs.md#inputstartingpositionconfigurationtypedef)
- `S3Configuration`:
  [S3ConfigurationTypeDef](./type_defs.md#s3configurationtypedef)
- `InputProcessingConfiguration`:
  [InputProcessingConfigurationTypeDef](./type_defs.md#inputprocessingconfigurationtypedef)

Returns a `Coroutine` for
[DiscoverInputSchemaResponseTypeDef](./type_defs.md#discoverinputschemaresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("kinesisanalytics").generate_presigned_url` method.

Boto3 documentation:
[KinesisAnalytics.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list\_applications"></a>

### list_applications

.

Type annotations for
`session.create_client("kinesisanalytics").list_applications` method.

Boto3 documentation:
[KinesisAnalytics.Client.list_applications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.list_applications)

Asynchronous method. Use `await list_applications(...)` for a synchronous call.

Arguments mapping described in
[ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef).

Keyword-only arguments:

- `Limit`: `int`
- `ExclusiveStartApplicationName`: `str`

Returns a `Coroutine` for
[ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Retrieves the list of key-value tags assigned to the application.

Type annotations for
`session.create_client("kinesisanalytics").list_tags_for_resource` method.

Boto3 documentation:
[KinesisAnalytics.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="start\_application"></a>

### start_application

.

Type annotations for
`session.create_client("kinesisanalytics").start_application` method.

Boto3 documentation:
[KinesisAnalytics.Client.start_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.start_application)

Asynchronous method. Use `await start_application(...)` for a synchronous call.

Arguments mapping described in
[StartApplicationRequestRequestTypeDef](./type_defs.md#startapplicationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*
- `InputConfigurations`:
  `Sequence`\[[InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef)\]
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="stop\_application"></a>

### stop_application

.

Type annotations for
`session.create_client("kinesisanalytics").stop_application` method.

Boto3 documentation:
[KinesisAnalytics.Client.stop_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.stop_application)

Asynchronous method. Use `await stop_application(...)` for a synchronous call.

Arguments mapping described in
[StopApplicationRequestRequestTypeDef](./type_defs.md#stopapplicationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="tag\_resource"></a>

### tag_resource

Adds one or more key-value tags to a Kinesis Analytics application.

Type annotations for `session.create_client("kinesisanalytics").tag_resource`
method.

Boto3 documentation:
[KinesisAnalytics.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Removes one or more tags from a Kinesis Analytics application.

Type annotations for `session.create_client("kinesisanalytics").untag_resource`
method.

Boto3 documentation:
[KinesisAnalytics.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_application"></a>

### update_application

.

Type annotations for
`session.create_client("kinesisanalytics").update_application` method.

Boto3 documentation:
[KinesisAnalytics.Client.update_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.update_application)

Asynchronous method. Use `await update_application(...)` for a synchronous
call.

Arguments mapping described in
[UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationName`: `str` *(required)*
- `CurrentApplicationVersionId`: `int` *(required)*
- `ApplicationUpdate`:
  [ApplicationUpdateTypeDef](./type_defs.md#applicationupdatetypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("kinesisanalytics").__aenter__`
method.

Boto3 documentation:
[KinesisAnalytics.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [KinesisAnalyticsClient](#kinesisanalyticsclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("kinesisanalytics").__aexit__`
method.

Boto3 documentation:
[KinesisAnalytics.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
