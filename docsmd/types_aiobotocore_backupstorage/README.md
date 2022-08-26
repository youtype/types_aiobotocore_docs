# BackupStorage module

> [Index](../README.md) > BackupStorage


!!! note ""

    Auto-generated documentation for [BackupStorage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
    type annotations stubs module [types-aiobotocore-backupstorage](https://pypi.org/project/types-aiobotocore-backupstorage/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `BackupStorage` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[backupstorage]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[backupstorage]'


# standalone installation
python -m pip install types-aiobotocore-backupstorage
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-backupstorage
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BackupStorageClient

Type annotations and code completion for  `#!python session.create_client("backupstorage")` as [BackupStorageClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backupstorage.client import BackupStorageClient


session = get_session()
async with session.create_client("backupstorage") as client:
    client: BackupStorageClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_backupstorage.literals import DataChecksumAlgorithmType

def get_value() -> DataChecksumAlgorithmType:
    return "SHA256"
```

- [DataChecksumAlgorithmType](./literals.md#datachecksumalgorithmtype)
- [SummaryChecksumAlgorithmType](./literals.md#summarychecksumalgorithmtype)
- [BackupStorageServiceName](./literals.md#backupstorageservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_backupstorage.type_defs import BackupObjectTypeDef

def get_value() -> BackupObjectTypeDef:
    return {
        "Name": ...,
        "ObjectChecksum": ...,
        "ObjectChecksumAlgorithm": ...,
        "ObjectToken": ...,
    }
```

- [BackupObjectTypeDef](./type_defs.md#backupobjecttypedef)
- [ChunkTypeDef](./type_defs.md#chunktypedef)
- [DeleteObjectInputRequestTypeDef](./type_defs.md#deleteobjectinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetChunkInputRequestTypeDef](./type_defs.md#getchunkinputrequesttypedef)
- [GetObjectMetadataInputRequestTypeDef](./type_defs.md#getobjectmetadatainputrequesttypedef)
- [ListChunksInputRequestTypeDef](./type_defs.md#listchunksinputrequesttypedef)
- [ListObjectsInputRequestTypeDef](./type_defs.md#listobjectsinputrequesttypedef)
- [NotifyObjectCompleteInputRequestTypeDef](./type_defs.md#notifyobjectcompleteinputrequesttypedef)
- [PutChunkInputRequestTypeDef](./type_defs.md#putchunkinputrequesttypedef)
- [PutObjectInputRequestTypeDef](./type_defs.md#putobjectinputrequesttypedef)
- [StartObjectInputRequestTypeDef](./type_defs.md#startobjectinputrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetChunkOutputTypeDef](./type_defs.md#getchunkoutputtypedef)
- [GetObjectMetadataOutputTypeDef](./type_defs.md#getobjectmetadataoutputtypedef)
- [ListChunksOutputTypeDef](./type_defs.md#listchunksoutputtypedef)
- [ListObjectsOutputTypeDef](./type_defs.md#listobjectsoutputtypedef)
- [NotifyObjectCompleteOutputTypeDef](./type_defs.md#notifyobjectcompleteoutputtypedef)
- [PutChunkOutputTypeDef](./type_defs.md#putchunkoutputtypedef)
- [PutObjectOutputTypeDef](./type_defs.md#putobjectoutputtypedef)
- [StartObjectOutputTypeDef](./type_defs.md#startobjectoutputtypedef)

