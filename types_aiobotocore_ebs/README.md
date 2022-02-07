<a id="type-annotations-for-aiobotocore-ebs-module"></a>

# Type annotations for aiobotocore EBS module

> [Index](..) > EBS

Auto-generated documentation for
[EBS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
type annotations stubs module
[types-aiobotocore-ebs](https://pypi.org/project/types-aiobotocore-ebs/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[ebs]'

# Lite version does not provide session.create_client overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[ebs]'

# standalone installation
pip install types-aiobotocore-ebs
```

- [Type annotations for aiobotocore EBS module](#type-annotations-for-aiobotocore-ebs-module)
  - [EBSClient](#ebsclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="ebsclient"></a>

## EBSClient

Type annotations for `session.create_client("ebs")` as [EBSClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_ebs.client import EBSClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [complete_snapshot](./client.md#complete_snapshot)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_snapshot_block](./client.md#get_snapshot_block)
- [list_changed_blocks](./client.md#list_changed_blocks)
- [list_snapshot_blocks](./client.md#list_snapshot_blocks)
- [put_snapshot_block](./client.md#put_snapshot_block)
- [start_snapshot](./client.md#start_snapshot)

<a id="exceptions"></a>

### Exceptions

EBSClient [exceptions](./client.md#exceptions)

- AccessDeniedException
- ClientError
- ConcurrentLimitExceededException
- ConflictException
- InternalServerException
- RequestThrottledException
- ResourceNotFoundException
- ServiceQuotaExceededException
- ValidationException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_ebs.literals import ChecksumAggregationMethodType, ...
```

- [ChecksumAggregationMethodType](./literals.md#checksumaggregationmethodtype)
- [ChecksumAlgorithmType](./literals.md#checksumalgorithmtype)
- [StatusType](./literals.md#statustype)
- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_ebs.type_defs import BlockTypeDef, ...
```

- [BlockTypeDef](./type_defs.md#blocktypedef)
- [ChangedBlockTypeDef](./type_defs.md#changedblocktypedef)
- [CompleteSnapshotRequestRequestTypeDef](./type_defs.md#completesnapshotrequestrequesttypedef)
- [CompleteSnapshotResponseTypeDef](./type_defs.md#completesnapshotresponsetypedef)
- [GetSnapshotBlockRequestRequestTypeDef](./type_defs.md#getsnapshotblockrequestrequesttypedef)
- [GetSnapshotBlockResponseTypeDef](./type_defs.md#getsnapshotblockresponsetypedef)
- [ListChangedBlocksRequestRequestTypeDef](./type_defs.md#listchangedblocksrequestrequesttypedef)
- [ListChangedBlocksResponseTypeDef](./type_defs.md#listchangedblocksresponsetypedef)
- [ListSnapshotBlocksRequestRequestTypeDef](./type_defs.md#listsnapshotblocksrequestrequesttypedef)
- [ListSnapshotBlocksResponseTypeDef](./type_defs.md#listsnapshotblocksresponsetypedef)
- [PutSnapshotBlockRequestRequestTypeDef](./type_defs.md#putsnapshotblockrequestrequesttypedef)
- [PutSnapshotBlockResponseTypeDef](./type_defs.md#putsnapshotblockresponsetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [StartSnapshotRequestRequestTypeDef](./type_defs.md#startsnapshotrequestrequesttypedef)
- [StartSnapshotResponseTypeDef](./type_defs.md#startsnapshotresponsetypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
