# DynamoDBStreams module

> [Index](../README.md) > DynamoDBStreams


!!! note ""

    Auto-generated documentation for [DynamoDBStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#dynamodbstreams)
    type annotations stubs module [types-aiobotocore-dynamodbstreams](https://pypi.org/project/types-aiobotocore-dynamodbstreams/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `DynamoDBStreams` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `DynamoDBStreams` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[dynamodbstreams]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[dynamodbstreams]'

# standalone installation
python -m pip install types-aiobotocore-dynamodbstreams
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-dynamodbstreams
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DynamoDBStreamsClient

Type annotations and code completion for  `#!python session.create_client("dynamodbstreams")` as [DynamoDBStreamsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)

```python
# DynamoDBStreamsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_dynamodbstreams.client import DynamoDBStreamsClient


session = get_session()
async with session.create_client("dynamodbstreams") as client:
    client: DynamoDBStreamsClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# KeyTypeType usage example

from types_aiobotocore_dynamodbstreams.literals import KeyTypeType

def get_value() -> KeyTypeType:
    return "HASH"
```

- [KeyTypeType](./literals.md#keytypetype)
- [OperationTypeType](./literals.md#operationtypetype)
- [ShardFilterTypeType](./literals.md#shardfiltertypetype)
- [ShardIteratorTypeType](./literals.md#sharditeratortypetype)
- [StreamStatusType](./literals.md#streamstatustype)
- [StreamViewTypeType](./literals.md#streamviewtypetype)
- [DynamoDBStreamsServiceName](./literals.md#dynamodbstreamsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AttributeValueTypeDef](./type_defs.md#attributevaluetypedef)
- [ShardFilterTypeDef](./type_defs.md#shardfiltertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetRecordsInputTypeDef](./type_defs.md#getrecordsinputtypedef)
- [GetShardIteratorInputTypeDef](./type_defs.md#getsharditeratorinputtypedef)
- [IdentityTypeDef](./type_defs.md#identitytypedef)
- [KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef)
- [ListStreamsInputTypeDef](./type_defs.md#liststreamsinputtypedef)
- [StreamTypeDef](./type_defs.md#streamtypedef)
- [SequenceNumberRangeTypeDef](./type_defs.md#sequencenumberrangetypedef)
- [StreamRecordTypeDef](./type_defs.md#streamrecordtypedef)
- [DescribeStreamInputTypeDef](./type_defs.md#describestreaminputtypedef)
- [GetShardIteratorOutputTypeDef](./type_defs.md#getsharditeratoroutputtypedef)
- [ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef)
- [ShardTypeDef](./type_defs.md#shardtypedef)
- [RecordTypeDef](./type_defs.md#recordtypedef)
- [StreamDescriptionTypeDef](./type_defs.md#streamdescriptiontypedef)
- [GetRecordsOutputTypeDef](./type_defs.md#getrecordsoutputtypedef)
- [DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef)

