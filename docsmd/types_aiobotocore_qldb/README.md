# QLDB module

> [Index](../README.md) > QLDB


!!! note ""

    Auto-generated documentation for [QLDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#qldb)
    type annotations stubs module [types-aiobotocore-qldb](https://pypi.org/project/types-aiobotocore-qldb/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.23.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `QLDB` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `QLDB` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[qldb]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[qldb]'

# standalone installation
python -m pip install types-aiobotocore-qldb
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-qldb
```

## Usage

Code samples can be found in [Examples](./usage.md).

## QLDBClient

Type annotations and code completion for  `#!python session.create_client("qldb")` as [QLDBClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client)

```python
# QLDBClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_qldb.client import QLDBClient


session = get_session()
async with session.create_client("qldb") as client:
    client: QLDBClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# EncryptionStatusType usage example

from types_aiobotocore_qldb.literals import EncryptionStatusType

def get_value() -> EncryptionStatusType:
    return "ENABLED"
```

- [EncryptionStatusType](./literals.md#encryptionstatustype)
- [ErrorCauseType](./literals.md#errorcausetype)
- [ExportStatusType](./literals.md#exportstatustype)
- [LedgerStateType](./literals.md#ledgerstatetype)
- [OutputFormatType](./literals.md#outputformattype)
- [PermissionsModeType](./literals.md#permissionsmodetype)
- [S3ObjectEncryptionTypeType](./literals.md#s3objectencryptiontypetype)
- [StreamStatusType](./literals.md#streamstatustype)
- [QLDBServiceName](./literals.md#qldbservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CancelJournalKinesisStreamRequestTypeDef](./type_defs.md#canceljournalkinesisstreamrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateLedgerRequestTypeDef](./type_defs.md#createledgerrequesttypedef)
- [DeleteLedgerRequestTypeDef](./type_defs.md#deleteledgerrequesttypedef)
- [DescribeJournalKinesisStreamRequestTypeDef](./type_defs.md#describejournalkinesisstreamrequesttypedef)
- [DescribeJournalS3ExportRequestTypeDef](./type_defs.md#describejournals3exportrequesttypedef)
- [DescribeLedgerRequestTypeDef](./type_defs.md#describeledgerrequesttypedef)
- [LedgerEncryptionDescriptionTypeDef](./type_defs.md#ledgerencryptiondescriptiontypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ValueHolderTypeDef](./type_defs.md#valueholdertypedef)
- [GetDigestRequestTypeDef](./type_defs.md#getdigestrequesttypedef)
- [KinesisConfigurationTypeDef](./type_defs.md#kinesisconfigurationtypedef)
- [LedgerSummaryTypeDef](./type_defs.md#ledgersummarytypedef)
- [ListJournalKinesisStreamsForLedgerRequestTypeDef](./type_defs.md#listjournalkinesisstreamsforledgerrequesttypedef)
- [ListJournalS3ExportsForLedgerRequestTypeDef](./type_defs.md#listjournals3exportsforledgerrequesttypedef)
- [ListJournalS3ExportsRequestTypeDef](./type_defs.md#listjournals3exportsrequesttypedef)
- [ListLedgersRequestTypeDef](./type_defs.md#listledgersrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [S3EncryptionConfigurationTypeDef](./type_defs.md#s3encryptionconfigurationtypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateLedgerPermissionsModeRequestTypeDef](./type_defs.md#updateledgerpermissionsmoderequesttypedef)
- [UpdateLedgerRequestTypeDef](./type_defs.md#updateledgerrequesttypedef)
- [CancelJournalKinesisStreamResponseTypeDef](./type_defs.md#canceljournalkinesisstreamresponsetypedef)
- [CreateLedgerResponseTypeDef](./type_defs.md#createledgerresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExportJournalToS3ResponseTypeDef](./type_defs.md#exportjournaltos3responsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StreamJournalToKinesisResponseTypeDef](./type_defs.md#streamjournaltokinesisresponsetypedef)
- [UpdateLedgerPermissionsModeResponseTypeDef](./type_defs.md#updateledgerpermissionsmoderesponsetypedef)
- [DescribeLedgerResponseTypeDef](./type_defs.md#describeledgerresponsetypedef)
- [UpdateLedgerResponseTypeDef](./type_defs.md#updateledgerresponsetypedef)
- [GetBlockRequestTypeDef](./type_defs.md#getblockrequesttypedef)
- [GetBlockResponseTypeDef](./type_defs.md#getblockresponsetypedef)
- [GetDigestResponseTypeDef](./type_defs.md#getdigestresponsetypedef)
- [GetRevisionRequestTypeDef](./type_defs.md#getrevisionrequesttypedef)
- [GetRevisionResponseTypeDef](./type_defs.md#getrevisionresponsetypedef)
- [JournalKinesisStreamDescriptionTypeDef](./type_defs.md#journalkinesisstreamdescriptiontypedef)
- [StreamJournalToKinesisRequestTypeDef](./type_defs.md#streamjournaltokinesisrequesttypedef)
- [ListLedgersResponseTypeDef](./type_defs.md#listledgersresponsetypedef)
- [S3ExportConfigurationTypeDef](./type_defs.md#s3exportconfigurationtypedef)
- [DescribeJournalKinesisStreamResponseTypeDef](./type_defs.md#describejournalkinesisstreamresponsetypedef)
- [ListJournalKinesisStreamsForLedgerResponseTypeDef](./type_defs.md#listjournalkinesisstreamsforledgerresponsetypedef)
- [ExportJournalToS3RequestTypeDef](./type_defs.md#exportjournaltos3requesttypedef)
- [JournalS3ExportDescriptionTypeDef](./type_defs.md#journals3exportdescriptiontypedef)
- [DescribeJournalS3ExportResponseTypeDef](./type_defs.md#describejournals3exportresponsetypedef)
- [ListJournalS3ExportsForLedgerResponseTypeDef](./type_defs.md#listjournals3exportsforledgerresponsetypedef)
- [ListJournalS3ExportsResponseTypeDef](./type_defs.md#listjournals3exportsresponsetypedef)

