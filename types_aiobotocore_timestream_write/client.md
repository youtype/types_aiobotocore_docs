<a id="timestreamwriteclient-for-aiobotocore-timestreamwrite-module"></a>

# TimestreamWriteClient for aiobotocore TimestreamWrite module

> [Index](..) > [TimestreamWrite](.) > TimestreamWriteClient

Auto-generated documentation for
[TimestreamWrite](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
type annotations stubs module
[types-aiobotocore-timestream-write](https://pypi.org/project/types-aiobotocore-timestream-write/).

- [TimestreamWriteClient for aiobotocore TimestreamWrite module](#timestreamwriteclient-for-aiobotocore-timestreamwrite-module)
  - [TimestreamWriteClient](#timestreamwriteclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_database](#create_database)
    - [create_table](#create_table)
    - [delete_database](#delete_database)
    - [delete_table](#delete_table)
    - [describe_database](#describe_database)
    - [describe_endpoints](#describe_endpoints)
    - [describe_table](#describe_table)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_databases](#list_databases)
    - [list_tables](#list_tables)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_database](#update_database)
    - [update_table](#update_table)
    - [write_records](#write_records)

<a id="timestreamwriteclient"></a>

## TimestreamWriteClient

Type annotations for `aiobotocore.create_client("timestream-write")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_timestream_write.client import TimestreamWriteClient

def get_timestream-write_client() -> TimestreamWriteClient:
    return Session().client("timestream-write")
```

Boto3 documentation:
[TimestreamWrite.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_timestream_write.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.InvalidEndpointException`
- `Exceptions.RejectedRecordsException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

TimestreamWriteClient exceptions.

Type annotations for `aiobotocore.create_client("timestream-write").exceptions`
method.

Boto3 documentation:
[TimestreamWrite.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`aiobotocore.create_client("timestream-write").can_paginate` method.

Boto3 documentation:
[TimestreamWrite.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_database"></a>

### create_database

Creates a new Timestream database.

Type annotations for
`aiobotocore.create_client("timestream-write").create_database` method.

Boto3 documentation:
[TimestreamWrite.Client.create_database](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_database)

Asynchronous method. Use `await create_database(...)` for a synchronous call.

Arguments mapping described in
[CreateDatabaseRequestRequestTypeDef](./type_defs.md#createdatabaserequestrequesttypedef).

Keyword-only arguments:

- `DatabaseName`: `str` *(required)*
- `KmsKeyId`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateDatabaseResponseTypeDef](./type_defs.md#createdatabaseresponsetypedef).

<a id="create_table"></a>

### create_table

The CreateTable operation adds a new table to an existing database in your
account.

Type annotations for
`aiobotocore.create_client("timestream-write").create_table` method.

Boto3 documentation:
[TimestreamWrite.Client.create_table](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)

Asynchronous method. Use `await create_table(...)` for a synchronous call.

Arguments mapping described in
[CreateTableRequestRequestTypeDef](./type_defs.md#createtablerequestrequesttypedef).

Keyword-only arguments:

- `DatabaseName`: `str` *(required)*
- `TableName`: `str` *(required)*
- `RetentionProperties`:
  [RetentionPropertiesTypeDef](./type_defs.md#retentionpropertiestypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `MagneticStoreWriteProperties`:
  [MagneticStoreWritePropertiesTypeDef](./type_defs.md#magneticstorewritepropertiestypedef)

Returns a `Coroutine` for
[CreateTableResponseTypeDef](./type_defs.md#createtableresponsetypedef).

<a id="delete_database"></a>

### delete_database

Deletes a given Timestream database.

Type annotations for
`aiobotocore.create_client("timestream-write").delete_database` method.

Boto3 documentation:
[TimestreamWrite.Client.delete_database](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.delete_database)

Asynchronous method. Use `await delete_database(...)` for a synchronous call.

Arguments mapping described in
[DeleteDatabaseRequestRequestTypeDef](./type_defs.md#deletedatabaserequestrequesttypedef).

Keyword-only arguments:

- `DatabaseName`: `str` *(required)*

<a id="delete_table"></a>

### delete_table

Deletes a given Timestream table.

Type annotations for
`aiobotocore.create_client("timestream-write").delete_table` method.

Boto3 documentation:
[TimestreamWrite.Client.delete_table](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.delete_table)

Asynchronous method. Use `await delete_table(...)` for a synchronous call.

Arguments mapping described in
[DeleteTableRequestRequestTypeDef](./type_defs.md#deletetablerequestrequesttypedef).

Keyword-only arguments:

- `DatabaseName`: `str` *(required)*
- `TableName`: `str` *(required)*

<a id="describe_database"></a>

### describe_database

Returns information about the database, including the database name, time that
the database was created, and the total number of tables found within the
database.

Type annotations for
`aiobotocore.create_client("timestream-write").describe_database` method.

Boto3 documentation:
[TimestreamWrite.Client.describe_database](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.describe_database)

Asynchronous method. Use `await describe_database(...)` for a synchronous call.

Arguments mapping described in
[DescribeDatabaseRequestRequestTypeDef](./type_defs.md#describedatabaserequestrequesttypedef).

Keyword-only arguments:

- `DatabaseName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDatabaseResponseTypeDef](./type_defs.md#describedatabaseresponsetypedef).

<a id="describe_endpoints"></a>

### describe_endpoints

DescribeEndpoints returns a list of available endpoints to make Timestream API
calls against.

Type annotations for
`aiobotocore.create_client("timestream-write").describe_endpoints` method.

Boto3 documentation:
[TimestreamWrite.Client.describe_endpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.describe_endpoints)

Asynchronous method. Use `await describe_endpoints(...)` for a synchronous
call.

Returns a `Coroutine` for
[DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef).

<a id="describe_table"></a>

### describe_table

Returns information about the table, including the table name, database name,
retention duration of the memory store and the magnetic store.

Type annotations for
`aiobotocore.create_client("timestream-write").describe_table` method.

Boto3 documentation:
[TimestreamWrite.Client.describe_table](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.describe_table)

Asynchronous method. Use `await describe_table(...)` for a synchronous call.

Arguments mapping described in
[DescribeTableRequestRequestTypeDef](./type_defs.md#describetablerequestrequesttypedef).

Keyword-only arguments:

- `DatabaseName`: `str` *(required)*
- `TableName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeTableResponseTypeDef](./type_defs.md#describetableresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("timestream-write").generate_presigned_url` method.

Boto3 documentation:
[TimestreamWrite.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_databases"></a>

### list_databases

Returns a list of your Timestream databases.

Type annotations for
`aiobotocore.create_client("timestream-write").list_databases` method.

Boto3 documentation:
[TimestreamWrite.Client.list_databases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.list_databases)

Asynchronous method. Use `await list_databases(...)` for a synchronous call.

Arguments mapping described in
[ListDatabasesRequestRequestTypeDef](./type_defs.md#listdatabasesrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListDatabasesResponseTypeDef](./type_defs.md#listdatabasesresponsetypedef).

<a id="list_tables"></a>

### list_tables

A list of tables, along with the name, status and retention properties of each
table.

Type annotations for
`aiobotocore.create_client("timestream-write").list_tables` method.

Boto3 documentation:
[TimestreamWrite.Client.list_tables](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.list_tables)

Asynchronous method. Use `await list_tables(...)` for a synchronous call.

Arguments mapping described in
[ListTablesRequestRequestTypeDef](./type_defs.md#listtablesrequestrequesttypedef).

Keyword-only arguments:

- `DatabaseName`: `str`
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

List all tags on a Timestream resource.

Type annotations for
`aiobotocore.create_client("timestream-write").list_tags_for_resource` method.

Boto3 documentation:
[TimestreamWrite.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Associate a set of tags with a Timestream resource.

Type annotations for
`aiobotocore.create_client("timestream-write").tag_resource` method.

Boto3 documentation:
[TimestreamWrite.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes the association of tags from a Timestream resource.

Type annotations for
`aiobotocore.create_client("timestream-write").untag_resource` method.

Boto3 documentation:
[TimestreamWrite.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_database"></a>

### update_database

Modifies the KMS key for an existing database.

Type annotations for
`aiobotocore.create_client("timestream-write").update_database` method.

Boto3 documentation:
[TimestreamWrite.Client.update_database](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_database)

Asynchronous method. Use `await update_database(...)` for a synchronous call.

Arguments mapping described in
[UpdateDatabaseRequestRequestTypeDef](./type_defs.md#updatedatabaserequestrequesttypedef).

Keyword-only arguments:

- `DatabaseName`: `str` *(required)*
- `KmsKeyId`: `str` *(required)*

Returns a `Coroutine` for
[UpdateDatabaseResponseTypeDef](./type_defs.md#updatedatabaseresponsetypedef).

<a id="update_table"></a>

### update_table

Modifies the retention duration of the memory store and magnetic store for your
Timestream table.

Type annotations for
`aiobotocore.create_client("timestream-write").update_table` method.

Boto3 documentation:
[TimestreamWrite.Client.update_table](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)

Asynchronous method. Use `await update_table(...)` for a synchronous call.

Arguments mapping described in
[UpdateTableRequestRequestTypeDef](./type_defs.md#updatetablerequestrequesttypedef).

Keyword-only arguments:

- `DatabaseName`: `str` *(required)*
- `TableName`: `str` *(required)*
- `RetentionProperties`:
  [RetentionPropertiesTypeDef](./type_defs.md#retentionpropertiestypedef)
- `MagneticStoreWriteProperties`:
  [MagneticStoreWritePropertiesTypeDef](./type_defs.md#magneticstorewritepropertiestypedef)

Returns a `Coroutine` for
[UpdateTableResponseTypeDef](./type_defs.md#updatetableresponsetypedef).

<a id="write_records"></a>

### write_records

The WriteRecords operation enables you to write your time series data into
Timestream.

Type annotations for
`aiobotocore.create_client("timestream-write").write_records` method.

Boto3 documentation:
[TimestreamWrite.Client.write_records](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.write_records)

Asynchronous method. Use `await write_records(...)` for a synchronous call.

Arguments mapping described in
[WriteRecordsRequestRequestTypeDef](./type_defs.md#writerecordsrequestrequesttypedef).

Keyword-only arguments:

- `DatabaseName`: `str` *(required)*
- `TableName`: `str` *(required)*
- `Records`: `Sequence`\[[RecordTypeDef](./type_defs.md#recordtypedef)\]
  *(required)*
- `CommonAttributes`: [RecordTypeDef](./type_defs.md#recordtypedef)

Returns a `Coroutine` for
[WriteRecordsResponseTypeDef](./type_defs.md#writerecordsresponsetypedef).
