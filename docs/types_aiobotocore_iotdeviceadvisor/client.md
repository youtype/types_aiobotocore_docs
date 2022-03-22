<a id="iotdeviceadvisorclient-for-aiobotocore-iotdeviceadvisor-module"></a>

# IoTDeviceAdvisorClient for aiobotocore IoTDeviceAdvisor module

> [Index](../README.md) > [IoTDeviceAdvisor](./README.md) >
> IoTDeviceAdvisorClient

Auto-generated documentation for
[IoTDeviceAdvisor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
type annotations stubs module
[types-aiobotocore-iotdeviceadvisor](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor/).

- [IoTDeviceAdvisorClient for aiobotocore IoTDeviceAdvisor module](#iotdeviceadvisorclient-for-aiobotocore-iotdeviceadvisor-module)
  - [IoTDeviceAdvisorClient](#iotdeviceadvisorclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_suite_definition](#create_suite_definition)
    - [delete_suite_definition](#delete_suite_definition)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_endpoint](#get_endpoint)
    - [get_suite_definition](#get_suite_definition)
    - [get_suite_run](#get_suite_run)
    - [get_suite_run_report](#get_suite_run_report)
    - [list_suite_definitions](#list_suite_definitions)
    - [list_suite_runs](#list_suite_runs)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [start_suite_run](#start_suite_run)
    - [stop_suite_run](#stop_suite_run)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_suite_definition](#update_suite_definition)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="iotdeviceadvisorclient"></a>

## IoTDeviceAdvisorClient

Type annotations for `session.create_client("iotdeviceadvisor")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_iotdeviceadvisor.client import IoTDeviceAdvisorClient

session = get_session()
async with session.create_client("iotdeviceadvisor") as client:
    client: IoTDeviceAdvisorClient
```

Boto3 documentation:
[IoTDeviceAdvisor.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_iotdeviceadvisor.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

IoTDeviceAdvisorClient exceptions.

Type annotations for `session.create_client("iotdeviceadvisor").exceptions`
method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("iotdeviceadvisor").can_paginate`
method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_suite\_definition"></a>

### create_suite_definition

Creates a Device Advisor test suite.

Type annotations for
`session.create_client("iotdeviceadvisor").create_suite_definition` method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.create_suite_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.create_suite_definition)

Asynchronous method. Use `await create_suite_definition(...)` for a synchronous
call.

Arguments mapping described in
[CreateSuiteDefinitionRequestRequestTypeDef](./type_defs.md#createsuitedefinitionrequestrequesttypedef).

Keyword-only arguments:

- `suiteDefinitionConfiguration`:
  [SuiteDefinitionConfigurationTypeDef](./type_defs.md#suitedefinitionconfigurationtypedef)
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateSuiteDefinitionResponseTypeDef](./type_defs.md#createsuitedefinitionresponsetypedef).

<a id="delete\_suite\_definition"></a>

### delete_suite_definition

Deletes a Device Advisor test suite.

Type annotations for
`session.create_client("iotdeviceadvisor").delete_suite_definition` method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.delete_suite_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.delete_suite_definition)

Asynchronous method. Use `await delete_suite_definition(...)` for a synchronous
call.

Arguments mapping described in
[DeleteSuiteDefinitionRequestRequestTypeDef](./type_defs.md#deletesuitedefinitionrequestrequesttypedef).

Keyword-only arguments:

- `suiteDefinitionId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("iotdeviceadvisor").generate_presigned_url` method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_endpoint"></a>

### get_endpoint

Gets information about an Device Advisor endpoint.

Type annotations for `session.create_client("iotdeviceadvisor").get_endpoint`
method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.get_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.get_endpoint)

Asynchronous method. Use `await get_endpoint(...)` for a synchronous call.

Arguments mapping described in
[GetEndpointRequestRequestTypeDef](./type_defs.md#getendpointrequestrequesttypedef).

Keyword-only arguments:

- `thingArn`: `str`
- `certificateArn`: `str`

Returns a `Coroutine` for
[GetEndpointResponseTypeDef](./type_defs.md#getendpointresponsetypedef).

<a id="get\_suite\_definition"></a>

### get_suite_definition

Gets information about a Device Advisor test suite.

Type annotations for
`session.create_client("iotdeviceadvisor").get_suite_definition` method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.get_suite_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.get_suite_definition)

Asynchronous method. Use `await get_suite_definition(...)` for a synchronous
call.

Arguments mapping described in
[GetSuiteDefinitionRequestRequestTypeDef](./type_defs.md#getsuitedefinitionrequestrequesttypedef).

Keyword-only arguments:

- `suiteDefinitionId`: `str` *(required)*
- `suiteDefinitionVersion`: `str`

Returns a `Coroutine` for
[GetSuiteDefinitionResponseTypeDef](./type_defs.md#getsuitedefinitionresponsetypedef).

<a id="get\_suite\_run"></a>

### get_suite_run

Gets information about a Device Advisor test suite run.

Type annotations for `session.create_client("iotdeviceadvisor").get_suite_run`
method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.get_suite_run](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.get_suite_run)

Asynchronous method. Use `await get_suite_run(...)` for a synchronous call.

Arguments mapping described in
[GetSuiteRunRequestRequestTypeDef](./type_defs.md#getsuiterunrequestrequesttypedef).

Keyword-only arguments:

- `suiteDefinitionId`: `str` *(required)*
- `suiteRunId`: `str` *(required)*

Returns a `Coroutine` for
[GetSuiteRunResponseTypeDef](./type_defs.md#getsuiterunresponsetypedef).

<a id="get\_suite\_run\_report"></a>

### get_suite_run_report

Gets a report download link for a successful Device Advisor qualifying test
suite run.

Type annotations for
`session.create_client("iotdeviceadvisor").get_suite_run_report` method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.get_suite_run_report](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.get_suite_run_report)

Asynchronous method. Use `await get_suite_run_report(...)` for a synchronous
call.

Arguments mapping described in
[GetSuiteRunReportRequestRequestTypeDef](./type_defs.md#getsuiterunreportrequestrequesttypedef).

Keyword-only arguments:

- `suiteDefinitionId`: `str` *(required)*
- `suiteRunId`: `str` *(required)*

Returns a `Coroutine` for
[GetSuiteRunReportResponseTypeDef](./type_defs.md#getsuiterunreportresponsetypedef).

<a id="list\_suite\_definitions"></a>

### list_suite_definitions

Lists the Device Advisor test suites you have created.

Type annotations for
`session.create_client("iotdeviceadvisor").list_suite_definitions` method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.list_suite_definitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.list_suite_definitions)

Asynchronous method. Use `await list_suite_definitions(...)` for a synchronous
call.

Arguments mapping described in
[ListSuiteDefinitionsRequestRequestTypeDef](./type_defs.md#listsuitedefinitionsrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListSuiteDefinitionsResponseTypeDef](./type_defs.md#listsuitedefinitionsresponsetypedef).

<a id="list\_suite\_runs"></a>

### list_suite_runs

Lists runs of the specified Device Advisor test suite.

Type annotations for
`session.create_client("iotdeviceadvisor").list_suite_runs` method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.list_suite_runs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.list_suite_runs)

Asynchronous method. Use `await list_suite_runs(...)` for a synchronous call.

Arguments mapping described in
[ListSuiteRunsRequestRequestTypeDef](./type_defs.md#listsuiterunsrequestrequesttypedef).

Keyword-only arguments:

- `suiteDefinitionId`: `str`
- `suiteDefinitionVersion`: `str`
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListSuiteRunsResponseTypeDef](./type_defs.md#listsuiterunsresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Lists the tags attached to an IoT Device Advisor resource.

Type annotations for
`session.create_client("iotdeviceadvisor").list_tags_for_resource` method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="start\_suite\_run"></a>

### start_suite_run

Starts a Device Advisor test suite run.

Type annotations for
`session.create_client("iotdeviceadvisor").start_suite_run` method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.start_suite_run](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.start_suite_run)

Asynchronous method. Use `await start_suite_run(...)` for a synchronous call.

Arguments mapping described in
[StartSuiteRunRequestRequestTypeDef](./type_defs.md#startsuiterunrequestrequesttypedef).

Keyword-only arguments:

- `suiteDefinitionId`: `str` *(required)*
- `suiteDefinitionVersion`: `str`
- `suiteRunConfiguration`:
  [SuiteRunConfigurationTypeDef](./type_defs.md#suiterunconfigurationtypedef)
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[StartSuiteRunResponseTypeDef](./type_defs.md#startsuiterunresponsetypedef).

<a id="stop\_suite\_run"></a>

### stop_suite_run

Stops a Device Advisor test suite run that is currently running.

Type annotations for `session.create_client("iotdeviceadvisor").stop_suite_run`
method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.stop_suite_run](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.stop_suite_run)

Asynchronous method. Use `await stop_suite_run(...)` for a synchronous call.

Arguments mapping described in
[StopSuiteRunRequestRequestTypeDef](./type_defs.md#stopsuiterunrequestrequesttypedef).

Keyword-only arguments:

- `suiteDefinitionId`: `str` *(required)*
- `suiteRunId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="tag\_resource"></a>

### tag_resource

Adds to and modifies existing tags of an IoT Device Advisor resource.

Type annotations for `session.create_client("iotdeviceadvisor").tag_resource`
method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Removes tags from an IoT Device Advisor resource.

Type annotations for `session.create_client("iotdeviceadvisor").untag_resource`
method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_suite\_definition"></a>

### update_suite_definition

Updates a Device Advisor test suite.

Type annotations for
`session.create_client("iotdeviceadvisor").update_suite_definition` method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.update_suite_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.update_suite_definition)

Asynchronous method. Use `await update_suite_definition(...)` for a synchronous
call.

Arguments mapping described in
[UpdateSuiteDefinitionRequestRequestTypeDef](./type_defs.md#updatesuitedefinitionrequestrequesttypedef).

Keyword-only arguments:

- `suiteDefinitionId`: `str` *(required)*
- `suiteDefinitionConfiguration`:
  [SuiteDefinitionConfigurationTypeDef](./type_defs.md#suitedefinitionconfigurationtypedef)

Returns a `Coroutine` for
[UpdateSuiteDefinitionResponseTypeDef](./type_defs.md#updatesuitedefinitionresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("iotdeviceadvisor").__aenter__`
method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [IoTDeviceAdvisorClient](#iotdeviceadvisorclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("iotdeviceadvisor").__aexit__`
method.

Boto3 documentation:
[IoTDeviceAdvisor.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
