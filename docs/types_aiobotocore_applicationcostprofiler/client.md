<a id="applicationcostprofilerclient-for-aiobotocore-applicationcostprofiler-module"></a>

# ApplicationCostProfilerClient for aiobotocore ApplicationCostProfiler module

> [Index](../README.md) > [ApplicationCostProfiler](./README.md) >
> ApplicationCostProfilerClient

Auto-generated documentation for
[ApplicationCostProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
type annotations stubs module
[types-aiobotocore-applicationcostprofiler](https://pypi.org/project/types-aiobotocore-applicationcostprofiler/).

- [ApplicationCostProfilerClient for aiobotocore ApplicationCostProfiler module](#applicationcostprofilerclient-for-aiobotocore-applicationcostprofiler-module)
  - [ApplicationCostProfilerClient](#applicationcostprofilerclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [delete_report_definition](#delete_report_definition)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_report_definition](#get_report_definition)
    - [import_application_usage](#import_application_usage)
    - [list_report_definitions](#list_report_definitions)
    - [put_report_definition](#put_report_definition)
    - [update_report_definition](#update_report_definition)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="applicationcostprofilerclient"></a>

## ApplicationCostProfilerClient

Type annotations for `session.create_client("applicationcostprofiler")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_applicationcostprofiler.client import ApplicationCostProfilerClient

session = get_session()
async with session.create_client("applicationcostprofiler") as client:
    client: ApplicationCostProfilerClient
```

Boto3 documentation:
[ApplicationCostProfiler.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_applicationcostprofiler.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.InternalServerException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ApplicationCostProfilerClient exceptions.

Type annotations for
`session.create_client("applicationcostprofiler").exceptions` method.

Boto3 documentation:
[ApplicationCostProfiler.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`session.create_client("applicationcostprofiler").can_paginate` method.

Boto3 documentation:
[ApplicationCostProfiler.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="delete\_report\_definition"></a>

### delete_report_definition

Deletes the specified report definition in AWS Application Cost Profiler.

Type annotations for
`session.create_client("applicationcostprofiler").delete_report_definition`
method.

Boto3 documentation:
[ApplicationCostProfiler.Client.delete_report_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.delete_report_definition)

Asynchronous method. Use `await delete_report_definition(...)` for a
synchronous call.

Arguments mapping described in
[DeleteReportDefinitionRequestRequestTypeDef](./type_defs.md#deletereportdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `reportId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteReportDefinitionResultTypeDef](./type_defs.md#deletereportdefinitionresulttypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("applicationcostprofiler").generate_presigned_url`
method.

Boto3 documentation:
[ApplicationCostProfiler.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_report\_definition"></a>

### get_report_definition

Retrieves the definition of a report already configured in AWS Application Cost
Profiler.

Type annotations for
`session.create_client("applicationcostprofiler").get_report_definition`
method.

Boto3 documentation:
[ApplicationCostProfiler.Client.get_report_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.get_report_definition)

Asynchronous method. Use `await get_report_definition(...)` for a synchronous
call.

Arguments mapping described in
[GetReportDefinitionRequestRequestTypeDef](./type_defs.md#getreportdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `reportId`: `str` *(required)*

Returns a `Coroutine` for
[GetReportDefinitionResultTypeDef](./type_defs.md#getreportdefinitionresulttypedef).

<a id="import\_application\_usage"></a>

### import_application_usage

Ingests application usage data from Amazon Simple Storage Service (Amazon S3).

Type annotations for
`session.create_client("applicationcostprofiler").import_application_usage`
method.

Boto3 documentation:
[ApplicationCostProfiler.Client.import_application_usage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.import_application_usage)

Asynchronous method. Use `await import_application_usage(...)` for a
synchronous call.

Arguments mapping described in
[ImportApplicationUsageRequestRequestTypeDef](./type_defs.md#importapplicationusagerequestrequesttypedef).

Keyword-only arguments:

- `sourceS3Location`:
  [SourceS3LocationTypeDef](./type_defs.md#sources3locationtypedef)
  *(required)*

Returns a `Coroutine` for
[ImportApplicationUsageResultTypeDef](./type_defs.md#importapplicationusageresulttypedef).

<a id="list\_report\_definitions"></a>

### list_report_definitions

Retrieves a list of all reports and their configurations for your AWS account.

Type annotations for
`session.create_client("applicationcostprofiler").list_report_definitions`
method.

Boto3 documentation:
[ApplicationCostProfiler.Client.list_report_definitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.list_report_definitions)

Asynchronous method. Use `await list_report_definitions(...)` for a synchronous
call.

Arguments mapping described in
[ListReportDefinitionsRequestRequestTypeDef](./type_defs.md#listreportdefinitionsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListReportDefinitionsResultTypeDef](./type_defs.md#listreportdefinitionsresulttypedef).

<a id="put\_report\_definition"></a>

### put_report_definition

Creates the report definition for a report in Application Cost Profiler.

Type annotations for
`session.create_client("applicationcostprofiler").put_report_definition`
method.

Boto3 documentation:
[ApplicationCostProfiler.Client.put_report_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.put_report_definition)

Asynchronous method. Use `await put_report_definition(...)` for a synchronous
call.

Arguments mapping described in
[PutReportDefinitionRequestRequestTypeDef](./type_defs.md#putreportdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `reportId`: `str` *(required)*
- `reportDescription`: `str` *(required)*
- `reportFrequency`: [ReportFrequencyType](./literals.md#reportfrequencytype)
  *(required)*
- `format`: [FormatType](./literals.md#formattype) *(required)*
- `destinationS3Location`:
  [S3LocationTypeDef](./type_defs.md#s3locationtypedef) *(required)*

Returns a `Coroutine` for
[PutReportDefinitionResultTypeDef](./type_defs.md#putreportdefinitionresulttypedef).

<a id="update\_report\_definition"></a>

### update_report_definition

Updates existing report in AWS Application Cost Profiler.

Type annotations for
`session.create_client("applicationcostprofiler").update_report_definition`
method.

Boto3 documentation:
[ApplicationCostProfiler.Client.update_report_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.update_report_definition)

Asynchronous method. Use `await update_report_definition(...)` for a
synchronous call.

Arguments mapping described in
[UpdateReportDefinitionRequestRequestTypeDef](./type_defs.md#updatereportdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `reportId`: `str` *(required)*
- `reportDescription`: `str` *(required)*
- `reportFrequency`: [ReportFrequencyType](./literals.md#reportfrequencytype)
  *(required)*
- `format`: [FormatType](./literals.md#formattype) *(required)*
- `destinationS3Location`:
  [S3LocationTypeDef](./type_defs.md#s3locationtypedef) *(required)*

Returns a `Coroutine` for
[UpdateReportDefinitionResultTypeDef](./type_defs.md#updatereportdefinitionresulttypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for
`session.create_client("applicationcostprofiler").__aenter__` method.

Boto3 documentation:
[ApplicationCostProfiler.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[ApplicationCostProfilerClient](#applicationcostprofilerclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for
`session.create_client("applicationcostprofiler").__aexit__` method.

Boto3 documentation:
[ApplicationCostProfiler.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for
`session.create_client("applicationcostprofiler").get_paginator` method with
overloads.

- `client.get_paginator("list_report_definitions")` ->
  [ListReportDefinitionsPaginator](./paginators.md#listreportdefinitionspaginator)
