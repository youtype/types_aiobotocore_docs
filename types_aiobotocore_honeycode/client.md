<a id="honeycodeclient-for-aiobotocore-honeycode-module"></a>

# HoneycodeClient for aiobotocore Honeycode module

> [Index](..) > [Honeycode](.) > HoneycodeClient

Auto-generated documentation for
[Honeycode](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
type annotations stubs module
[types-aiobotocore-honeycode](https://pypi.org/project/types-aiobotocore-honeycode/).

- [HoneycodeClient for aiobotocore Honeycode module](#honeycodeclient-for-aiobotocore-honeycode-module)
  - [HoneycodeClient](#honeycodeclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [batch_create_table_rows](#batch_create_table_rows)
    - [batch_delete_table_rows](#batch_delete_table_rows)
    - [batch_update_table_rows](#batch_update_table_rows)
    - [batch_upsert_table_rows](#batch_upsert_table_rows)
    - [can_paginate](#can_paginate)
    - [describe_table_data_import_job](#describe_table_data_import_job)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_screen_data](#get_screen_data)
    - [invoke_screen_automation](#invoke_screen_automation)
    - [list_table_columns](#list_table_columns)
    - [list_table_rows](#list_table_rows)
    - [list_tables](#list_tables)
    - [query_table_rows](#query_table_rows)
    - [start_table_data_import_job](#start_table_data_import_job)
    - [get_paginator](#get_paginator)

<a id="honeycodeclient"></a>

## HoneycodeClient

Type annotations for `aiobotocore.create_client("honeycode")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_honeycode.client import HoneycodeClient

def get_honeycode_client() -> HoneycodeClient:
    return Session().client("honeycode")
```

Boto3 documentation:
[Honeycode.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_honeycode.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.AutomationExecutionException`
- `Exceptions.AutomationExecutionTimeoutException`
- `Exceptions.ClientError`
- `Exceptions.InternalServerException`
- `Exceptions.RequestTimeoutException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ServiceUnavailableException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

HoneycodeClient exceptions.

Type annotations for `aiobotocore.create_client("honeycode").exceptions`
method.

Boto3 documentation:
[Honeycode.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="batch_create_table_rows"></a>

### batch_create_table_rows

The BatchCreateTableRows API allows you to create one or more rows at the end
of a table in a workbook.

Type annotations for
`aiobotocore.create_client("honeycode").batch_create_table_rows` method.

Boto3 documentation:
[Honeycode.Client.batch_create_table_rows](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.batch_create_table_rows)

Asynchronous method. Use `await batch_create_table_rows(...)` for a synchronous
call.

Arguments mapping described in
[BatchCreateTableRowsRequestRequestTypeDef](./type_defs.md#batchcreatetablerowsrequestrequesttypedef).

Keyword-only arguments:

- `workbookId`: `str` *(required)*
- `tableId`: `str` *(required)*
- `rowsToCreate`:
  `Sequence`\[[CreateRowDataTypeDef](./type_defs.md#createrowdatatypedef)\]
  *(required)*
- `clientRequestToken`: `str`

Returns a `Coroutine` for
[BatchCreateTableRowsResultTypeDef](./type_defs.md#batchcreatetablerowsresulttypedef).

<a id="batch_delete_table_rows"></a>

### batch_delete_table_rows

The BatchDeleteTableRows API allows you to delete one or more rows from a table
in a workbook.

Type annotations for
`aiobotocore.create_client("honeycode").batch_delete_table_rows` method.

Boto3 documentation:
[Honeycode.Client.batch_delete_table_rows](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.batch_delete_table_rows)

Asynchronous method. Use `await batch_delete_table_rows(...)` for a synchronous
call.

Arguments mapping described in
[BatchDeleteTableRowsRequestRequestTypeDef](./type_defs.md#batchdeletetablerowsrequestrequesttypedef).

Keyword-only arguments:

- `workbookId`: `str` *(required)*
- `tableId`: `str` *(required)*
- `rowIds`: `Sequence`\[`str`\] *(required)*
- `clientRequestToken`: `str`

Returns a `Coroutine` for
[BatchDeleteTableRowsResultTypeDef](./type_defs.md#batchdeletetablerowsresulttypedef).

<a id="batch_update_table_rows"></a>

### batch_update_table_rows

The BatchUpdateTableRows API allows you to update one or more rows in a table
in a workbook.

Type annotations for
`aiobotocore.create_client("honeycode").batch_update_table_rows` method.

Boto3 documentation:
[Honeycode.Client.batch_update_table_rows](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.batch_update_table_rows)

Asynchronous method. Use `await batch_update_table_rows(...)` for a synchronous
call.

Arguments mapping described in
[BatchUpdateTableRowsRequestRequestTypeDef](./type_defs.md#batchupdatetablerowsrequestrequesttypedef).

Keyword-only arguments:

- `workbookId`: `str` *(required)*
- `tableId`: `str` *(required)*
- `rowsToUpdate`:
  `Sequence`\[[UpdateRowDataTypeDef](./type_defs.md#updaterowdatatypedef)\]
  *(required)*
- `clientRequestToken`: `str`

Returns a `Coroutine` for
[BatchUpdateTableRowsResultTypeDef](./type_defs.md#batchupdatetablerowsresulttypedef).

<a id="batch_upsert_table_rows"></a>

### batch_upsert_table_rows

The BatchUpsertTableRows API allows you to upsert one or more rows in a table.

Type annotations for
`aiobotocore.create_client("honeycode").batch_upsert_table_rows` method.

Boto3 documentation:
[Honeycode.Client.batch_upsert_table_rows](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.batch_upsert_table_rows)

Asynchronous method. Use `await batch_upsert_table_rows(...)` for a synchronous
call.

Arguments mapping described in
[BatchUpsertTableRowsRequestRequestTypeDef](./type_defs.md#batchupserttablerowsrequestrequesttypedef).

Keyword-only arguments:

- `workbookId`: `str` *(required)*
- `tableId`: `str` *(required)*
- `rowsToUpsert`:
  `Sequence`\[[UpsertRowDataTypeDef](./type_defs.md#upsertrowdatatypedef)\]
  *(required)*
- `clientRequestToken`: `str`

Returns a `Coroutine` for
[BatchUpsertTableRowsResultTypeDef](./type_defs.md#batchupserttablerowsresulttypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("honeycode").can_paginate`
method.

Boto3 documentation:
[Honeycode.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="describe_table_data_import_job"></a>

### describe_table_data_import_job

The DescribeTableDataImportJob API allows you to retrieve the status and
details of a table data import job.

Type annotations for
`aiobotocore.create_client("honeycode").describe_table_data_import_job` method.

Boto3 documentation:
[Honeycode.Client.describe_table_data_import_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.describe_table_data_import_job)

Asynchronous method. Use `await describe_table_data_import_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeTableDataImportJobRequestRequestTypeDef](./type_defs.md#describetabledataimportjobrequestrequesttypedef).

Keyword-only arguments:

- `workbookId`: `str` *(required)*
- `tableId`: `str` *(required)*
- `jobId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeTableDataImportJobResultTypeDef](./type_defs.md#describetabledataimportjobresulttypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("honeycode").generate_presigned_url` method.

Boto3 documentation:
[Honeycode.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_screen_data"></a>

### get_screen_data

The GetScreenData API allows retrieval of data from a screen in a Honeycode
app.

Type annotations for `aiobotocore.create_client("honeycode").get_screen_data`
method.

Boto3 documentation:
[Honeycode.Client.get_screen_data](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.get_screen_data)

Asynchronous method. Use `await get_screen_data(...)` for a synchronous call.

Arguments mapping described in
[GetScreenDataRequestRequestTypeDef](./type_defs.md#getscreendatarequestrequesttypedef).

Keyword-only arguments:

- `workbookId`: `str` *(required)*
- `appId`: `str` *(required)*
- `screenId`: `str` *(required)*
- `variables`: `Mapping`\[`str`,
  [VariableValueTypeDef](./type_defs.md#variablevaluetypedef)\]
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[GetScreenDataResultTypeDef](./type_defs.md#getscreendataresulttypedef).

<a id="invoke_screen_automation"></a>

### invoke_screen_automation

The InvokeScreenAutomation API allows invoking an action defined in a screen in
a Honeycode app.

Type annotations for
`aiobotocore.create_client("honeycode").invoke_screen_automation` method.

Boto3 documentation:
[Honeycode.Client.invoke_screen_automation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.invoke_screen_automation)

Asynchronous method. Use `await invoke_screen_automation(...)` for a
synchronous call.

Arguments mapping described in
[InvokeScreenAutomationRequestRequestTypeDef](./type_defs.md#invokescreenautomationrequestrequesttypedef).

Keyword-only arguments:

- `workbookId`: `str` *(required)*
- `appId`: `str` *(required)*
- `screenId`: `str` *(required)*
- `screenAutomationId`: `str` *(required)*
- `variables`: `Mapping`\[`str`,
  [VariableValueTypeDef](./type_defs.md#variablevaluetypedef)\]
- `rowId`: `str`
- `clientRequestToken`: `str`

Returns a `Coroutine` for
[InvokeScreenAutomationResultTypeDef](./type_defs.md#invokescreenautomationresulttypedef).

<a id="list_table_columns"></a>

### list_table_columns

The ListTableColumns API allows you to retrieve a list of all the columns in a
table in a workbook.

Type annotations for
`aiobotocore.create_client("honeycode").list_table_columns` method.

Boto3 documentation:
[Honeycode.Client.list_table_columns](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.list_table_columns)

Asynchronous method. Use `await list_table_columns(...)` for a synchronous
call.

Arguments mapping described in
[ListTableColumnsRequestRequestTypeDef](./type_defs.md#listtablecolumnsrequestrequesttypedef).

Keyword-only arguments:

- `workbookId`: `str` *(required)*
- `tableId`: `str` *(required)*
- `nextToken`: `str`

Returns a `Coroutine` for
[ListTableColumnsResultTypeDef](./type_defs.md#listtablecolumnsresulttypedef).

<a id="list_table_rows"></a>

### list_table_rows

The ListTableRows API allows you to retrieve a list of all the rows in a table
in a workbook.

Type annotations for `aiobotocore.create_client("honeycode").list_table_rows`
method.

Boto3 documentation:
[Honeycode.Client.list_table_rows](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.list_table_rows)

Asynchronous method. Use `await list_table_rows(...)` for a synchronous call.

Arguments mapping described in
[ListTableRowsRequestRequestTypeDef](./type_defs.md#listtablerowsrequestrequesttypedef).

Keyword-only arguments:

- `workbookId`: `str` *(required)*
- `tableId`: `str` *(required)*
- `rowIds`: `Sequence`\[`str`\]
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListTableRowsResultTypeDef](./type_defs.md#listtablerowsresulttypedef).

<a id="list_tables"></a>

### list_tables

The ListTables API allows you to retrieve a list of all the tables in a
workbook.

Type annotations for `aiobotocore.create_client("honeycode").list_tables`
method.

Boto3 documentation:
[Honeycode.Client.list_tables](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.list_tables)

Asynchronous method. Use `await list_tables(...)` for a synchronous call.

Arguments mapping described in
[ListTablesRequestRequestTypeDef](./type_defs.md#listtablesrequestrequesttypedef).

Keyword-only arguments:

- `workbookId`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListTablesResultTypeDef](./type_defs.md#listtablesresulttypedef).

<a id="query_table_rows"></a>

### query_table_rows

The QueryTableRows API allows you to use a filter formula to query for specific
rows in a table.

Type annotations for `aiobotocore.create_client("honeycode").query_table_rows`
method.

Boto3 documentation:
[Honeycode.Client.query_table_rows](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.query_table_rows)

Asynchronous method. Use `await query_table_rows(...)` for a synchronous call.

Arguments mapping described in
[QueryTableRowsRequestRequestTypeDef](./type_defs.md#querytablerowsrequestrequesttypedef).

Keyword-only arguments:

- `workbookId`: `str` *(required)*
- `tableId`: `str` *(required)*
- `filterFormula`: [FilterTypeDef](./type_defs.md#filtertypedef) *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[QueryTableRowsResultTypeDef](./type_defs.md#querytablerowsresulttypedef).

<a id="start_table_data_import_job"></a>

### start_table_data_import_job

The StartTableDataImportJob API allows you to start an import job on a table.

Type annotations for
`aiobotocore.create_client("honeycode").start_table_data_import_job` method.

Boto3 documentation:
[Honeycode.Client.start_table_data_import_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.start_table_data_import_job)

Asynchronous method. Use `await start_table_data_import_job(...)` for a
synchronous call.

Arguments mapping described in
[StartTableDataImportJobRequestRequestTypeDef](./type_defs.md#starttabledataimportjobrequestrequesttypedef).

Keyword-only arguments:

- `workbookId`: `str` *(required)*
- `dataSource`:
  [ImportDataSourceTypeDef](./type_defs.md#importdatasourcetypedef)
  *(required)*
- `dataFormat`: `Literal['DELIMITED_TEXT']` (see
  [ImportSourceDataFormatType](./literals.md#importsourcedataformattype))
  *(required)*
- `destinationTableId`: `str` *(required)*
- `importOptions`: [ImportOptionsTypeDef](./type_defs.md#importoptionstypedef)
  *(required)*
- `clientRequestToken`: `str` *(required)*

Returns a `Coroutine` for
[StartTableDataImportJobResultTypeDef](./type_defs.md#starttabledataimportjobresulttypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("honeycode").get_paginator`
method with overloads.

- `client.get_paginator("list_table_columns")` ->
  [ListTableColumnsPaginator](./paginators.md#listtablecolumnspaginator)
- `client.get_paginator("list_table_rows")` ->
  [ListTableRowsPaginator](./paginators.md#listtablerowspaginator)
- `client.get_paginator("list_tables")` ->
  [ListTablesPaginator](./paginators.md#listtablespaginator)
- `client.get_paginator("query_table_rows")` ->
  [QueryTableRowsPaginator](./paginators.md#querytablerowspaginator)
