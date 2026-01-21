# EBS module

> [Index](../README.md) > EBS


!!! note ""

    Auto-generated documentation for [EBS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#ebs)
    type annotations stubs module [types-aiobotocore-ebs](https://pypi.org/project/types-aiobotocore-ebs/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `EBS` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `EBS` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[ebs]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[ebs]'

# standalone installation
python -m pip install types-aiobotocore-ebs
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-ebs
```

## Usage

Code samples can be found in [Examples](./usage.md).

## EBSClient

Type annotations and code completion for  `#!python session.create_client("ebs")` as [EBSClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)

```python
# EBSClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_ebs.client import EBSClient


session = get_session()
async with session.create_client("ebs") as client:
    client: EBSClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ChecksumAggregationMethodType usage example

from types_aiobotocore_ebs.literals import ChecksumAggregationMethodType

def get_value() -> ChecksumAggregationMethodType:
    return "LINEAR"
```

- [ChecksumAggregationMethodType](./literals.md#checksumaggregationmethodtype)
- [ChecksumAlgorithmType](./literals.md#checksumalgorithmtype)
- [SSETypeType](./literals.md#ssetypetype)
- [StatusType](./literals.md#statustype)
- [EBSServiceName](./literals.md#ebsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BlobTypeDef](./type_defs.md#blobtypedef)
- [BlockTypeDef](./type_defs.md#blocktypedef)
- [ChangedBlockTypeDef](./type_defs.md#changedblocktypedef)
- [CompleteSnapshotRequestTypeDef](./type_defs.md#completesnapshotrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetSnapshotBlockRequestTypeDef](./type_defs.md#getsnapshotblockrequesttypedef)
- [ListChangedBlocksRequestTypeDef](./type_defs.md#listchangedblocksrequesttypedef)
- [ListSnapshotBlocksRequestTypeDef](./type_defs.md#listsnapshotblocksrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [PutSnapshotBlockRequestTypeDef](./type_defs.md#putsnapshotblockrequesttypedef)
- [CompleteSnapshotResponseTypeDef](./type_defs.md#completesnapshotresponsetypedef)
- [GetSnapshotBlockResponseTypeDef](./type_defs.md#getsnapshotblockresponsetypedef)
- [ListChangedBlocksResponseTypeDef](./type_defs.md#listchangedblocksresponsetypedef)
- [ListSnapshotBlocksResponseTypeDef](./type_defs.md#listsnapshotblocksresponsetypedef)
- [PutSnapshotBlockResponseTypeDef](./type_defs.md#putsnapshotblockresponsetypedef)
- [StartSnapshotRequestTypeDef](./type_defs.md#startsnapshotrequesttypedef)
- [StartSnapshotResponseTypeDef](./type_defs.md#startsnapshotresponsetypedef)

