<a id="costandusagereportserviceclient-for-aiobotocore-costandusagereportservice-module"></a>

# CostandUsageReportServiceClient for aiobotocore CostandUsageReportService module

> [Index](..) > [CostandUsageReportService](.) >
> CostandUsageReportServiceClient

Auto-generated documentation for
[CostandUsageReportService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
type annotations stubs module
[types-aiobotocore-cur](https://pypi.org/project/types-aiobotocore-cur/).

- [CostandUsageReportServiceClient for aiobotocore CostandUsageReportService module](#costandusagereportserviceclient-for-aiobotocore-costandusagereportservice-module)
  - [CostandUsageReportServiceClient](#costandusagereportserviceclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [delete_report_definition](#delete_report_definition)
    - [describe_report_definitions](#describe_report_definitions)
    - [generate_presigned_url](#generate_presigned_url)
    - [modify_report_definition](#modify_report_definition)
    - [put_report_definition](#put_report_definition)
    - [get_paginator](#get_paginator)

<a id="costandusagereportserviceclient"></a>

## CostandUsageReportServiceClient

Type annotations for `aiobotocore.create_client("cur")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_cur.client import CostandUsageReportServiceClient

def get_cur_client() -> CostandUsageReportServiceClient:
    return Session().client("cur")
```

Boto3 documentation:
[CostandUsageReportService.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_cur.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.DuplicateReportNameException`
- `Exceptions.InternalErrorException`
- `Exceptions.ReportLimitReachedException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

CostandUsageReportServiceClient exceptions.

Type annotations for `aiobotocore.create_client("cur").exceptions` method.

Boto3 documentation:
[CostandUsageReportService.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("cur").can_paginate` method.

Boto3 documentation:
[CostandUsageReportService.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="delete_report_definition"></a>

### delete_report_definition

Deletes the specified report.

Type annotations for
`aiobotocore.create_client("cur").delete_report_definition` method.

Boto3 documentation:
[CostandUsageReportService.Client.delete_report_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.delete_report_definition)

Asynchronous method. Use `await delete_report_definition(...)` for a
synchronous call.

Arguments mapping described in
[DeleteReportDefinitionRequestRequestTypeDef](./type_defs.md#deletereportdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `ReportName`: `str`

Returns a `Coroutine` for
[DeleteReportDefinitionResponseTypeDef](./type_defs.md#deletereportdefinitionresponsetypedef).

<a id="describe_report_definitions"></a>

### describe_report_definitions

Lists the AWS Cost and Usage reports available to this account.

Type annotations for
`aiobotocore.create_client("cur").describe_report_definitions` method.

Boto3 documentation:
[CostandUsageReportService.Client.describe_report_definitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.describe_report_definitions)

Asynchronous method. Use `await describe_report_definitions(...)` for a
synchronous call.

Arguments mapping described in
[DescribeReportDefinitionsRequestRequestTypeDef](./type_defs.md#describereportdefinitionsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeReportDefinitionsResponseTypeDef](./type_defs.md#describereportdefinitionsresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `aiobotocore.create_client("cur").generate_presigned_url`
method.

Boto3 documentation:
[CostandUsageReportService.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="modify_report_definition"></a>

### modify_report_definition

Allows you to programatically update your report preferences.

Type annotations for
`aiobotocore.create_client("cur").modify_report_definition` method.

Boto3 documentation:
[CostandUsageReportService.Client.modify_report_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.modify_report_definition)

Asynchronous method. Use `await modify_report_definition(...)` for a
synchronous call.

Arguments mapping described in
[ModifyReportDefinitionRequestRequestTypeDef](./type_defs.md#modifyreportdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `ReportName`: `str` *(required)*
- `ReportDefinition`:
  [ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="put_report_definition"></a>

### put_report_definition

Creates a new report using the description that you provide.

Type annotations for `aiobotocore.create_client("cur").put_report_definition`
method.

Boto3 documentation:
[CostandUsageReportService.Client.put_report_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.put_report_definition)

Asynchronous method. Use `await put_report_definition(...)` for a synchronous
call.

Arguments mapping described in
[PutReportDefinitionRequestRequestTypeDef](./type_defs.md#putreportdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `ReportDefinition`:
  [ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("cur").get_paginator` method
with overloads.

- `client.get_paginator("describe_report_definitions")` ->
  [DescribeReportDefinitionsPaginator](./paginators.md#describereportdefinitionspaginator)
