# EBS module

> [Index](../README.md) > EBS


!!! note ""

    Auto-generated documentation for [EBS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
    type annotations stubs module [types-aiobotocore-ebs](https://pypi.org/project/types-aiobotocore-ebs/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `EBS`.

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

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ebs.client import EBSClient


session = get_session()
async with session.create_client("ebs") as client:
    client: EBSClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_ebs.literals import ChecksumAggregationMethodType

def get_value() -> ChecksumAggregationMethodType:
    return "LINEAR"
```

- [ChecksumAggregationMethodType](./literals.md#checksumaggregationmethodtype)
- [ChecksumAlgorithmType](./literals.md#checksumalgorithmtype)
- [StatusType](./literals.md#statustype)
- [EBSServiceName](./literals.md#ebsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_ebs.type_defs import BlockTypeDef

def get_value() -> BlockTypeDef:
    return {
        "BlockIndex": ...,
    }
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

