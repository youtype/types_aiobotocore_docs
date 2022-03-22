<a id="qldbclient-for-aiobotocore-qldb-module"></a>

# QLDBClient for aiobotocore QLDB module

> [Index](../README.md) > [QLDB](./README.md) > QLDBClient

Auto-generated documentation for
[QLDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
type annotations stubs module
[types-aiobotocore-qldb](https://pypi.org/project/types-aiobotocore-qldb/).

- [QLDBClient for aiobotocore QLDB module](#qldbclient-for-aiobotocore-qldb-module)
  - [QLDBClient](#qldbclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [cancel_journal_kinesis_stream](#cancel_journal_kinesis_stream)
    - [create_ledger](#create_ledger)
    - [delete_ledger](#delete_ledger)
    - [describe_journal_kinesis_stream](#describe_journal_kinesis_stream)
    - [describe_journal_s3_export](#describe_journal_s3_export)
    - [describe_ledger](#describe_ledger)
    - [export_journal_to_s3](#export_journal_to_s3)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_block](#get_block)
    - [get_digest](#get_digest)
    - [get_revision](#get_revision)
    - [list_journal_kinesis_streams_for_ledger](#list_journal_kinesis_streams_for_ledger)
    - [list_journal_s3_exports](#list_journal_s3_exports)
    - [list_journal_s3_exports_for_ledger](#list_journal_s3_exports_for_ledger)
    - [list_ledgers](#list_ledgers)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [stream_journal_to_kinesis](#stream_journal_to_kinesis)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_ledger](#update_ledger)
    - [update_ledger_permissions_mode](#update_ledger_permissions_mode)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="qldbclient"></a>

## QLDBClient

Type annotations for `session.create_client("qldb")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_qldb.client import QLDBClient

session = get_session()
async with session.create_client("qldb") as client:
    client: QLDBClient
```

Boto3 documentation:
[QLDB.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_qldb.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InvalidParameterException`
- `Exceptions.LimitExceededException`
- `Exceptions.ResourceAlreadyExistsException`
- `Exceptions.ResourceInUseException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ResourcePreconditionNotMetException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

QLDBClient exceptions.

Type annotations for `session.create_client("qldb").exceptions` method.

Boto3 documentation:
[QLDB.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("qldb").can_paginate` method.

Boto3 documentation:
[QLDB.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel\_journal\_kinesis\_stream"></a>

### cancel_journal_kinesis_stream

Ends a given Amazon QLDB journal stream.

Type annotations for
`session.create_client("qldb").cancel_journal_kinesis_stream` method.

Boto3 documentation:
[QLDB.Client.cancel_journal_kinesis_stream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.cancel_journal_kinesis_stream)

Asynchronous method. Use `await cancel_journal_kinesis_stream(...)` for a
synchronous call.

Arguments mapping described in
[CancelJournalKinesisStreamRequestRequestTypeDef](./type_defs.md#canceljournalkinesisstreamrequestrequesttypedef).

Keyword-only arguments:

- `LedgerName`: `str` *(required)*
- `StreamId`: `str` *(required)*

Returns a `Coroutine` for
[CancelJournalKinesisStreamResponseTypeDef](./type_defs.md#canceljournalkinesisstreamresponsetypedef).

<a id="create\_ledger"></a>

### create_ledger

Creates a new ledger in your Amazon Web Services account in the current Region.

Type annotations for `session.create_client("qldb").create_ledger` method.

Boto3 documentation:
[QLDB.Client.create_ledger](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.create_ledger)

Asynchronous method. Use `await create_ledger(...)` for a synchronous call.

Arguments mapping described in
[CreateLedgerRequestRequestTypeDef](./type_defs.md#createledgerrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `PermissionsMode`: [PermissionsModeType](./literals.md#permissionsmodetype)
  *(required)*
- `Tags`: `Mapping`\[`str`, `str`\]
- `DeletionProtection`: `bool`
- `KmsKey`: `str`

Returns a `Coroutine` for
[CreateLedgerResponseTypeDef](./type_defs.md#createledgerresponsetypedef).

<a id="delete\_ledger"></a>

### delete_ledger

Deletes a ledger and all of its contents.

Type annotations for `session.create_client("qldb").delete_ledger` method.

Boto3 documentation:
[QLDB.Client.delete_ledger](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.delete_ledger)

Asynchronous method. Use `await delete_ledger(...)` for a synchronous call.

Arguments mapping described in
[DeleteLedgerRequestRequestTypeDef](./type_defs.md#deleteledgerrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

<a id="describe\_journal\_kinesis\_stream"></a>

### describe_journal_kinesis_stream

Returns detailed information about a given Amazon QLDB journal stream.

Type annotations for
`session.create_client("qldb").describe_journal_kinesis_stream` method.

Boto3 documentation:
[QLDB.Client.describe_journal_kinesis_stream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.describe_journal_kinesis_stream)

Asynchronous method. Use `await describe_journal_kinesis_stream(...)` for a
synchronous call.

Arguments mapping described in
[DescribeJournalKinesisStreamRequestRequestTypeDef](./type_defs.md#describejournalkinesisstreamrequestrequesttypedef).

Keyword-only arguments:

- `LedgerName`: `str` *(required)*
- `StreamId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeJournalKinesisStreamResponseTypeDef](./type_defs.md#describejournalkinesisstreamresponsetypedef).

<a id="describe\_journal\_s3\_export"></a>

### describe_journal_s3_export

Returns information about a journal export job, including the ledger name,
export ID, creation time, current status, and the parameters of the original
export creation request.

Type annotations for `session.create_client("qldb").describe_journal_s3_export`
method.

Boto3 documentation:
[QLDB.Client.describe_journal_s3_export](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.describe_journal_s3_export)

Asynchronous method. Use `await describe_journal_s3_export(...)` for a
synchronous call.

Arguments mapping described in
[DescribeJournalS3ExportRequestRequestTypeDef](./type_defs.md#describejournals3exportrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ExportId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeJournalS3ExportResponseTypeDef](./type_defs.md#describejournals3exportresponsetypedef).

<a id="describe\_ledger"></a>

### describe_ledger

Returns information about a ledger, including its state, permissions mode,
encryption at rest settings, and when it was created.

Type annotations for `session.create_client("qldb").describe_ledger` method.

Boto3 documentation:
[QLDB.Client.describe_ledger](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.describe_ledger)

Asynchronous method. Use `await describe_ledger(...)` for a synchronous call.

Arguments mapping described in
[DescribeLedgerRequestRequestTypeDef](./type_defs.md#describeledgerrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[DescribeLedgerResponseTypeDef](./type_defs.md#describeledgerresponsetypedef).

<a id="export\_journal\_to\_s3"></a>

### export_journal_to_s3

Exports journal contents within a date and time range from a ledger into a
specified Amazon Simple Storage Service (Amazon S3) bucket.

Type annotations for `session.create_client("qldb").export_journal_to_s3`
method.

Boto3 documentation:
[QLDB.Client.export_journal_to_s3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.export_journal_to_s3)

Asynchronous method. Use `await export_journal_to_s3(...)` for a synchronous
call.

Arguments mapping described in
[ExportJournalToS3RequestRequestTypeDef](./type_defs.md#exportjournaltos3requestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `InclusiveStartTime`: `Union`\[`datetime`, `str`\] *(required)*
- `ExclusiveEndTime`: `Union`\[`datetime`, `str`\] *(required)*
- `S3ExportConfiguration`:
  [S3ExportConfigurationTypeDef](./type_defs.md#s3exportconfigurationtypedef)
  *(required)*
- `RoleArn`: `str` *(required)*
- `OutputFormat`: [OutputFormatType](./literals.md#outputformattype)

Returns a `Coroutine` for
[ExportJournalToS3ResponseTypeDef](./type_defs.md#exportjournaltos3responsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("qldb").generate_presigned_url`
method.

Boto3 documentation:
[QLDB.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_block"></a>

### get_block

Returns a block object at a specified address in a journal.

Type annotations for `session.create_client("qldb").get_block` method.

Boto3 documentation:
[QLDB.Client.get_block](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.get_block)

Asynchronous method. Use `await get_block(...)` for a synchronous call.

Arguments mapping described in
[GetBlockRequestRequestTypeDef](./type_defs.md#getblockrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `BlockAddress`: [ValueHolderTypeDef](./type_defs.md#valueholdertypedef)
  *(required)*
- `DigestTipAddress`: [ValueHolderTypeDef](./type_defs.md#valueholdertypedef)

Returns a `Coroutine` for
[GetBlockResponseTypeDef](./type_defs.md#getblockresponsetypedef).

<a id="get\_digest"></a>

### get_digest

Returns the digest of a ledger at the latest committed block in the journal.

Type annotations for `session.create_client("qldb").get_digest` method.

Boto3 documentation:
[QLDB.Client.get_digest](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.get_digest)

Asynchronous method. Use `await get_digest(...)` for a synchronous call.

Arguments mapping described in
[GetDigestRequestRequestTypeDef](./type_defs.md#getdigestrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[GetDigestResponseTypeDef](./type_defs.md#getdigestresponsetypedef).

<a id="get\_revision"></a>

### get_revision

Returns a revision data object for a specified document ID and block address.

Type annotations for `session.create_client("qldb").get_revision` method.

Boto3 documentation:
[QLDB.Client.get_revision](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.get_revision)

Asynchronous method. Use `await get_revision(...)` for a synchronous call.

Arguments mapping described in
[GetRevisionRequestRequestTypeDef](./type_defs.md#getrevisionrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `BlockAddress`: [ValueHolderTypeDef](./type_defs.md#valueholdertypedef)
  *(required)*
- `DocumentId`: `str` *(required)*
- `DigestTipAddress`: [ValueHolderTypeDef](./type_defs.md#valueholdertypedef)

Returns a `Coroutine` for
[GetRevisionResponseTypeDef](./type_defs.md#getrevisionresponsetypedef).

<a id="list\_journal\_kinesis\_streams\_for\_ledger"></a>

### list_journal_kinesis_streams_for_ledger

Returns an array of all Amazon QLDB journal stream descriptors for a given
ledger.

Type annotations for
`session.create_client("qldb").list_journal_kinesis_streams_for_ledger` method.

Boto3 documentation:
[QLDB.Client.list_journal_kinesis_streams_for_ledger](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.list_journal_kinesis_streams_for_ledger)

Asynchronous method. Use `await list_journal_kinesis_streams_for_ledger(...)`
for a synchronous call.

Arguments mapping described in
[ListJournalKinesisStreamsForLedgerRequestRequestTypeDef](./type_defs.md#listjournalkinesisstreamsforledgerrequestrequesttypedef).

Keyword-only arguments:

- `LedgerName`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListJournalKinesisStreamsForLedgerResponseTypeDef](./type_defs.md#listjournalkinesisstreamsforledgerresponsetypedef).

<a id="list\_journal\_s3\_exports"></a>

### list_journal_s3_exports

Returns an array of journal export job descriptions for all ledgers that are
associated with the current Amazon Web Services account and Region.

Type annotations for `session.create_client("qldb").list_journal_s3_exports`
method.

Boto3 documentation:
[QLDB.Client.list_journal_s3_exports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.list_journal_s3_exports)

Asynchronous method. Use `await list_journal_s3_exports(...)` for a synchronous
call.

Arguments mapping described in
[ListJournalS3ExportsRequestRequestTypeDef](./type_defs.md#listjournals3exportsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListJournalS3ExportsResponseTypeDef](./type_defs.md#listjournals3exportsresponsetypedef).

<a id="list\_journal\_s3\_exports\_for\_ledger"></a>

### list_journal_s3_exports_for_ledger

Returns an array of journal export job descriptions for a specified ledger.

Type annotations for
`session.create_client("qldb").list_journal_s3_exports_for_ledger` method.

Boto3 documentation:
[QLDB.Client.list_journal_s3_exports_for_ledger](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.list_journal_s3_exports_for_ledger)

Asynchronous method. Use `await list_journal_s3_exports_for_ledger(...)` for a
synchronous call.

Arguments mapping described in
[ListJournalS3ExportsForLedgerRequestRequestTypeDef](./type_defs.md#listjournals3exportsforledgerrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListJournalS3ExportsForLedgerResponseTypeDef](./type_defs.md#listjournals3exportsforledgerresponsetypedef).

<a id="list\_ledgers"></a>

### list_ledgers

Returns an array of ledger summaries that are associated with the current
Amazon Web Services account and Region.

Type annotations for `session.create_client("qldb").list_ledgers` method.

Boto3 documentation:
[QLDB.Client.list_ledgers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.list_ledgers)

Asynchronous method. Use `await list_ledgers(...)` for a synchronous call.

Arguments mapping described in
[ListLedgersRequestRequestTypeDef](./type_defs.md#listledgersrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListLedgersResponseTypeDef](./type_defs.md#listledgersresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Returns all tags for a specified Amazon QLDB resource.

Type annotations for `session.create_client("qldb").list_tags_for_resource`
method.

Boto3 documentation:
[QLDB.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="stream\_journal\_to\_kinesis"></a>

### stream_journal_to_kinesis

Creates a journal stream for a given Amazon QLDB ledger.

Type annotations for `session.create_client("qldb").stream_journal_to_kinesis`
method.

Boto3 documentation:
[QLDB.Client.stream_journal_to_kinesis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.stream_journal_to_kinesis)

Asynchronous method. Use `await stream_journal_to_kinesis(...)` for a
synchronous call.

Arguments mapping described in
[StreamJournalToKinesisRequestRequestTypeDef](./type_defs.md#streamjournaltokinesisrequestrequesttypedef).

Keyword-only arguments:

- `LedgerName`: `str` *(required)*
- `RoleArn`: `str` *(required)*
- `InclusiveStartTime`: `Union`\[`datetime`, `str`\] *(required)*
- `KinesisConfiguration`:
  [KinesisConfigurationTypeDef](./type_defs.md#kinesisconfigurationtypedef)
  *(required)*
- `StreamName`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\]
- `ExclusiveEndTime`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for
[StreamJournalToKinesisResponseTypeDef](./type_defs.md#streamjournaltokinesisresponsetypedef).

<a id="tag\_resource"></a>

### tag_resource

Adds one or more tags to a specified Amazon QLDB resource.

Type annotations for `session.create_client("qldb").tag_resource` method.

Boto3 documentation:
[QLDB.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Removes one or more tags from a specified Amazon QLDB resource.

Type annotations for `session.create_client("qldb").untag_resource` method.

Boto3 documentation:
[QLDB.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_ledger"></a>

### update_ledger

Updates properties on a ledger.

Type annotations for `session.create_client("qldb").update_ledger` method.

Boto3 documentation:
[QLDB.Client.update_ledger](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.update_ledger)

Asynchronous method. Use `await update_ledger(...)` for a synchronous call.

Arguments mapping described in
[UpdateLedgerRequestRequestTypeDef](./type_defs.md#updateledgerrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `DeletionProtection`: `bool`
- `KmsKey`: `str`

Returns a `Coroutine` for
[UpdateLedgerResponseTypeDef](./type_defs.md#updateledgerresponsetypedef).

<a id="update\_ledger\_permissions\_mode"></a>

### update_ledger_permissions_mode

Updates the permissions mode of a ledger.

Type annotations for
`session.create_client("qldb").update_ledger_permissions_mode` method.

Boto3 documentation:
[QLDB.Client.update_ledger_permissions_mode](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.update_ledger_permissions_mode)

Asynchronous method. Use `await update_ledger_permissions_mode(...)` for a
synchronous call.

Arguments mapping described in
[UpdateLedgerPermissionsModeRequestRequestTypeDef](./type_defs.md#updateledgerpermissionsmoderequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `PermissionsMode`: [PermissionsModeType](./literals.md#permissionsmodetype)
  *(required)*

Returns a `Coroutine` for
[UpdateLedgerPermissionsModeResponseTypeDef](./type_defs.md#updateledgerpermissionsmoderesponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("qldb").__aenter__` method.

Boto3 documentation:
[QLDB.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [QLDBClient](#qldbclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("qldb").__aexit__` method.

Boto3 documentation:
[QLDB.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
