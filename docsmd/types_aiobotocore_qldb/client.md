# QLDBClient

> [Index](../README.md) > [QLDB](./README.md) > QLDBClient

!!! note ""

    Auto-generated documentation for [QLDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#qldb)
    type annotations stubs module [types-aiobotocore-qldb](https://pypi.org/project/types-aiobotocore-qldb/).

## QLDBClient

Type annotations and code completion for `#!python session.create_client("qldb")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client)

```python
# QLDBClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_qldb.client import QLDBClient

session = get_session()
async with session.create_client("qldb") as client:
    client: QLDBClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("qldb").exceptions` structure.

```python
# QLDBClient.exceptions usage example

async with session.create_client("qldb") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InvalidParameterException,
        client.LimitExceededException,
        client.ResourceAlreadyExistsException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.ResourcePreconditionNotMetException,
    ) as e:
        print(e)
```

```python
# QLDBClient usage type checking example

from types_aiobotocore_qldb.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("qldb").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("qldb").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### cancel\_journal\_kinesis\_stream

Ends a given Amazon QLDB journal stream.

Type annotations and code completion for `#!python session.create_client("qldb").cancel_journal_kinesis_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/cancel_journal_kinesis_stream.html)

```python
# cancel_journal_kinesis_stream method definition

await def cancel_journal_kinesis_stream(
    self,
    *,
    LedgerName: str,
    StreamId: str,
) -> CancelJournalKinesisStreamResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelJournalKinesisStreamResponseTypeDef](./type_defs.md#canceljournalkinesisstreamresponsetypedef) 


```python
# cancel_journal_kinesis_stream method usage example with argument unpacking

kwargs: CancelJournalKinesisStreamRequestTypeDef = {  # (1)
    "LedgerName": ...,
    "StreamId": ...,
}

parent.cancel_journal_kinesis_stream(**kwargs)
```

1. See [:material-code-braces: CancelJournalKinesisStreamRequestTypeDef](./type_defs.md#canceljournalkinesisstreamrequesttypedef) 

### create\_ledger

Creates a new ledger in your Amazon Web Services account in the current Region.

Type annotations and code completion for `#!python session.create_client("qldb").create_ledger` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/create_ledger.html)

```python
# create_ledger method definition

await def create_ledger(
    self,
    *,
    Name: str,
    PermissionsMode: PermissionsModeType,  # (1)
    Tags: Mapping[str, str] = ...,
    DeletionProtection: bool = ...,
    KmsKey: str = ...,
) -> CreateLedgerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PermissionsModeType](./literals.md#permissionsmodetype) 
2. See [:material-code-braces: CreateLedgerResponseTypeDef](./type_defs.md#createledgerresponsetypedef) 


```python
# create_ledger method usage example with argument unpacking

kwargs: CreateLedgerRequestTypeDef = {  # (1)
    "Name": ...,
    "PermissionsMode": ...,
}

parent.create_ledger(**kwargs)
```

1. See [:material-code-braces: CreateLedgerRequestTypeDef](./type_defs.md#createledgerrequesttypedef) 

### delete\_ledger

Deletes a ledger and all of its contents.

Type annotations and code completion for `#!python session.create_client("qldb").delete_ledger` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/delete_ledger.html)

```python
# delete_ledger method definition

await def delete_ledger(
    self,
    *,
    Name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_ledger method usage example with argument unpacking

kwargs: DeleteLedgerRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_ledger(**kwargs)
```

1. See [:material-code-braces: DeleteLedgerRequestTypeDef](./type_defs.md#deleteledgerrequesttypedef) 

### describe\_journal\_kinesis\_stream

Returns detailed information about a given Amazon QLDB journal stream.

Type annotations and code completion for `#!python session.create_client("qldb").describe_journal_kinesis_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/describe_journal_kinesis_stream.html)

```python
# describe_journal_kinesis_stream method definition

await def describe_journal_kinesis_stream(
    self,
    *,
    LedgerName: str,
    StreamId: str,
) -> DescribeJournalKinesisStreamResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeJournalKinesisStreamResponseTypeDef](./type_defs.md#describejournalkinesisstreamresponsetypedef) 


```python
# describe_journal_kinesis_stream method usage example with argument unpacking

kwargs: DescribeJournalKinesisStreamRequestTypeDef = {  # (1)
    "LedgerName": ...,
    "StreamId": ...,
}

parent.describe_journal_kinesis_stream(**kwargs)
```

1. See [:material-code-braces: DescribeJournalKinesisStreamRequestTypeDef](./type_defs.md#describejournalkinesisstreamrequesttypedef) 

### describe\_journal\_s3\_export

Returns information about a journal export job, including the ledger name,
export ID, creation time, current status, and the parameters of the original
export creation request.

Type annotations and code completion for `#!python session.create_client("qldb").describe_journal_s3_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/describe_journal_s3_export.html)

```python
# describe_journal_s3_export method definition

await def describe_journal_s3_export(
    self,
    *,
    Name: str,
    ExportId: str,
) -> DescribeJournalS3ExportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeJournalS3ExportResponseTypeDef](./type_defs.md#describejournals3exportresponsetypedef) 


```python
# describe_journal_s3_export method usage example with argument unpacking

kwargs: DescribeJournalS3ExportRequestTypeDef = {  # (1)
    "Name": ...,
    "ExportId": ...,
}

parent.describe_journal_s3_export(**kwargs)
```

1. See [:material-code-braces: DescribeJournalS3ExportRequestTypeDef](./type_defs.md#describejournals3exportrequesttypedef) 

### describe\_ledger

Returns information about a ledger, including its state, permissions mode,
encryption at rest settings, and when it was created.

Type annotations and code completion for `#!python session.create_client("qldb").describe_ledger` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/describe_ledger.html)

```python
# describe_ledger method definition

await def describe_ledger(
    self,
    *,
    Name: str,
) -> DescribeLedgerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLedgerResponseTypeDef](./type_defs.md#describeledgerresponsetypedef) 


```python
# describe_ledger method usage example with argument unpacking

kwargs: DescribeLedgerRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_ledger(**kwargs)
```

1. See [:material-code-braces: DescribeLedgerRequestTypeDef](./type_defs.md#describeledgerrequesttypedef) 

### export\_journal\_to\_s3

Exports journal contents within a date and time range from a ledger into a
specified Amazon Simple Storage Service (Amazon S3) bucket.

Type annotations and code completion for `#!python session.create_client("qldb").export_journal_to_s3` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/export_journal_to_s3.html)

```python
# export_journal_to_s3 method definition

await def export_journal_to_s3(
    self,
    *,
    Name: str,
    InclusiveStartTime: TimestampTypeDef,
    ExclusiveEndTime: TimestampTypeDef,
    S3ExportConfiguration: S3ExportConfigurationTypeDef,  # (1)
    RoleArn: str,
    OutputFormat: OutputFormatType = ...,  # (2)
) -> ExportJournalToS3ResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: S3ExportConfigurationTypeDef](./type_defs.md#s3exportconfigurationtypedef) 
2. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
3. See [:material-code-braces: ExportJournalToS3ResponseTypeDef](./type_defs.md#exportjournaltos3responsetypedef) 


```python
# export_journal_to_s3 method usage example with argument unpacking

kwargs: ExportJournalToS3RequestTypeDef = {  # (1)
    "Name": ...,
    "InclusiveStartTime": ...,
    "ExclusiveEndTime": ...,
    "S3ExportConfiguration": ...,
    "RoleArn": ...,
}

parent.export_journal_to_s3(**kwargs)
```

1. See [:material-code-braces: ExportJournalToS3RequestTypeDef](./type_defs.md#exportjournaltos3requesttypedef) 

### get\_block

Returns a block object at a specified address in a journal.

Type annotations and code completion for `#!python session.create_client("qldb").get_block` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/get_block.html)

```python
# get_block method definition

await def get_block(
    self,
    *,
    Name: str,
    BlockAddress: ValueHolderTypeDef,  # (1)
    DigestTipAddress: ValueHolderTypeDef = ...,  # (1)
) -> GetBlockResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
2. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
3. See [:material-code-braces: GetBlockResponseTypeDef](./type_defs.md#getblockresponsetypedef) 


```python
# get_block method usage example with argument unpacking

kwargs: GetBlockRequestTypeDef = {  # (1)
    "Name": ...,
    "BlockAddress": ...,
}

parent.get_block(**kwargs)
```

1. See [:material-code-braces: GetBlockRequestTypeDef](./type_defs.md#getblockrequesttypedef) 

### get\_digest

Returns the digest of a ledger at the latest committed block in the journal.

Type annotations and code completion for `#!python session.create_client("qldb").get_digest` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/get_digest.html)

```python
# get_digest method definition

await def get_digest(
    self,
    *,
    Name: str,
) -> GetDigestResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDigestResponseTypeDef](./type_defs.md#getdigestresponsetypedef) 


```python
# get_digest method usage example with argument unpacking

kwargs: GetDigestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_digest(**kwargs)
```

1. See [:material-code-braces: GetDigestRequestTypeDef](./type_defs.md#getdigestrequesttypedef) 

### get\_revision

Returns a revision data object for a specified document ID and block address.

Type annotations and code completion for `#!python session.create_client("qldb").get_revision` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/get_revision.html)

```python
# get_revision method definition

await def get_revision(
    self,
    *,
    Name: str,
    BlockAddress: ValueHolderTypeDef,  # (1)
    DocumentId: str,
    DigestTipAddress: ValueHolderTypeDef = ...,  # (1)
) -> GetRevisionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
2. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
3. See [:material-code-braces: GetRevisionResponseTypeDef](./type_defs.md#getrevisionresponsetypedef) 


```python
# get_revision method usage example with argument unpacking

kwargs: GetRevisionRequestTypeDef = {  # (1)
    "Name": ...,
    "BlockAddress": ...,
    "DocumentId": ...,
}

parent.get_revision(**kwargs)
```

1. See [:material-code-braces: GetRevisionRequestTypeDef](./type_defs.md#getrevisionrequesttypedef) 

### list\_journal\_kinesis\_streams\_for\_ledger

Returns all Amazon QLDB journal streams for a given ledger.

Type annotations and code completion for `#!python session.create_client("qldb").list_journal_kinesis_streams_for_ledger` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/list_journal_kinesis_streams_for_ledger.html)

```python
# list_journal_kinesis_streams_for_ledger method definition

await def list_journal_kinesis_streams_for_ledger(
    self,
    *,
    LedgerName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListJournalKinesisStreamsForLedgerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJournalKinesisStreamsForLedgerResponseTypeDef](./type_defs.md#listjournalkinesisstreamsforledgerresponsetypedef) 


```python
# list_journal_kinesis_streams_for_ledger method usage example with argument unpacking

kwargs: ListJournalKinesisStreamsForLedgerRequestTypeDef = {  # (1)
    "LedgerName": ...,
}

parent.list_journal_kinesis_streams_for_ledger(**kwargs)
```

1. See [:material-code-braces: ListJournalKinesisStreamsForLedgerRequestTypeDef](./type_defs.md#listjournalkinesisstreamsforledgerrequesttypedef) 

### list\_journal\_s3\_exports

Returns all journal export jobs for all ledgers that are associated with the
current Amazon Web Services account and Region.

Type annotations and code completion for `#!python session.create_client("qldb").list_journal_s3_exports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/list_journal_s3_exports.html)

```python
# list_journal_s3_exports method definition

await def list_journal_s3_exports(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListJournalS3ExportsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJournalS3ExportsResponseTypeDef](./type_defs.md#listjournals3exportsresponsetypedef) 


```python
# list_journal_s3_exports method usage example with argument unpacking

kwargs: ListJournalS3ExportsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_journal_s3_exports(**kwargs)
```

1. See [:material-code-braces: ListJournalS3ExportsRequestTypeDef](./type_defs.md#listjournals3exportsrequesttypedef) 

### list\_journal\_s3\_exports\_for\_ledger

Returns all journal export jobs for a specified ledger.

Type annotations and code completion for `#!python session.create_client("qldb").list_journal_s3_exports_for_ledger` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/list_journal_s3_exports_for_ledger.html)

```python
# list_journal_s3_exports_for_ledger method definition

await def list_journal_s3_exports_for_ledger(
    self,
    *,
    Name: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListJournalS3ExportsForLedgerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJournalS3ExportsForLedgerResponseTypeDef](./type_defs.md#listjournals3exportsforledgerresponsetypedef) 


```python
# list_journal_s3_exports_for_ledger method usage example with argument unpacking

kwargs: ListJournalS3ExportsForLedgerRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.list_journal_s3_exports_for_ledger(**kwargs)
```

1. See [:material-code-braces: ListJournalS3ExportsForLedgerRequestTypeDef](./type_defs.md#listjournals3exportsforledgerrequesttypedef) 

### list\_ledgers

Returns all ledgers that are associated with the current Amazon Web Services
account and Region.

Type annotations and code completion for `#!python session.create_client("qldb").list_ledgers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/list_ledgers.html)

```python
# list_ledgers method definition

await def list_ledgers(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListLedgersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLedgersResponseTypeDef](./type_defs.md#listledgersresponsetypedef) 


```python
# list_ledgers method usage example with argument unpacking

kwargs: ListLedgersRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_ledgers(**kwargs)
```

1. See [:material-code-braces: ListLedgersRequestTypeDef](./type_defs.md#listledgersrequesttypedef) 

### list\_tags\_for\_resource

Returns all tags for a specified Amazon QLDB resource.

Type annotations and code completion for `#!python session.create_client("qldb").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### stream\_journal\_to\_kinesis

Creates a journal stream for a given Amazon QLDB ledger.

Type annotations and code completion for `#!python session.create_client("qldb").stream_journal_to_kinesis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/stream_journal_to_kinesis.html)

```python
# stream_journal_to_kinesis method definition

await def stream_journal_to_kinesis(
    self,
    *,
    LedgerName: str,
    RoleArn: str,
    InclusiveStartTime: TimestampTypeDef,
    KinesisConfiguration: KinesisConfigurationTypeDef,  # (1)
    StreamName: str,
    Tags: Mapping[str, str] = ...,
    ExclusiveEndTime: TimestampTypeDef = ...,
) -> StreamJournalToKinesisResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: KinesisConfigurationTypeDef](./type_defs.md#kinesisconfigurationtypedef) 
2. See [:material-code-braces: StreamJournalToKinesisResponseTypeDef](./type_defs.md#streamjournaltokinesisresponsetypedef) 


```python
# stream_journal_to_kinesis method usage example with argument unpacking

kwargs: StreamJournalToKinesisRequestTypeDef = {  # (1)
    "LedgerName": ...,
    "RoleArn": ...,
    "InclusiveStartTime": ...,
    "KinesisConfiguration": ...,
    "StreamName": ...,
}

parent.stream_journal_to_kinesis(**kwargs)
```

1. See [:material-code-braces: StreamJournalToKinesisRequestTypeDef](./type_defs.md#streamjournaltokinesisrequesttypedef) 

### tag\_resource

Adds one or more tags to a specified Amazon QLDB resource.

Type annotations and code completion for `#!python session.create_client("qldb").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes one or more tags from a specified Amazon QLDB resource.

Type annotations and code completion for `#!python session.create_client("qldb").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_ledger

Updates properties on a ledger.

Type annotations and code completion for `#!python session.create_client("qldb").update_ledger` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/update_ledger.html)

```python
# update_ledger method definition

await def update_ledger(
    self,
    *,
    Name: str,
    DeletionProtection: bool = ...,
    KmsKey: str = ...,
) -> UpdateLedgerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateLedgerResponseTypeDef](./type_defs.md#updateledgerresponsetypedef) 


```python
# update_ledger method usage example with argument unpacking

kwargs: UpdateLedgerRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_ledger(**kwargs)
```

1. See [:material-code-braces: UpdateLedgerRequestTypeDef](./type_defs.md#updateledgerrequesttypedef) 

### update\_ledger\_permissions\_mode

Updates the permissions mode of a ledger.

Type annotations and code completion for `#!python session.create_client("qldb").update_ledger_permissions_mode` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb/client/update_ledger_permissions_mode.html)

```python
# update_ledger_permissions_mode method definition

await def update_ledger_permissions_mode(
    self,
    *,
    Name: str,
    PermissionsMode: PermissionsModeType,  # (1)
) -> UpdateLedgerPermissionsModeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PermissionsModeType](./literals.md#permissionsmodetype) 
2. See [:material-code-braces: UpdateLedgerPermissionsModeResponseTypeDef](./type_defs.md#updateledgerpermissionsmoderesponsetypedef) 


```python
# update_ledger_permissions_mode method usage example with argument unpacking

kwargs: UpdateLedgerPermissionsModeRequestTypeDef = {  # (1)
    "Name": ...,
    "PermissionsMode": ...,
}

parent.update_ledger_permissions_mode(**kwargs)
```

1. See [:material-code-braces: UpdateLedgerPermissionsModeRequestTypeDef](./type_defs.md#updateledgerpermissionsmoderequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("qldb").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("qldb").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```





