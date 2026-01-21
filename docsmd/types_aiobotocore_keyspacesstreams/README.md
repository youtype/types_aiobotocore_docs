# KeyspacesStreams module

> [Index](../README.md) > KeyspacesStreams


!!! note ""

    Auto-generated documentation for [KeyspacesStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspacesstreams.html#keyspacesstreams)
    type annotations stubs module [types-aiobotocore-keyspacesstreams](https://pypi.org/project/types-aiobotocore-keyspacesstreams/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `KeyspacesStreams` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `KeyspacesStreams` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[keyspacesstreams]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[keyspacesstreams]'

# standalone installation
python -m pip install types-aiobotocore-keyspacesstreams
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-keyspacesstreams
```

## Usage

Code samples can be found in [Examples](./usage.md).

## KeyspacesStreamsClient

Type annotations and code completion for  `#!python session.create_client("keyspacesstreams")` as [KeyspacesStreamsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspacesstreams.html#KeyspacesStreams.Client)

```python
# KeyspacesStreamsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_keyspacesstreams.client import KeyspacesStreamsClient


session = get_session()
async with session.create_client("keyspacesstreams") as client:
    client: KeyspacesStreamsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("keyspacesstreams").get_paginator("...")`.

```python
# GetStreamPaginator usage example

from types_aiobotocore_keyspacesstreams.paginator import GetStreamPaginator

def get_get_stream_paginator() -> GetStreamPaginator:
    return client.get_paginator("get_stream"))
```

- [GetStreamPaginator](./paginators.md#getstreampaginator)
- [ListStreamsPaginator](./paginators.md#liststreamspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# GetStreamPaginatorName usage example

from types_aiobotocore_keyspacesstreams.literals import GetStreamPaginatorName

def get_value() -> GetStreamPaginatorName:
    return "get_stream"
```

- [GetStreamPaginatorName](./literals.md#getstreampaginatorname)
- [ListStreamsPaginatorName](./literals.md#liststreamspaginatorname)
- [OriginTypeType](./literals.md#origintypetype)
- [ShardFilterTypeType](./literals.md#shardfiltertypetype)
- [ShardIteratorTypeType](./literals.md#sharditeratortypetype)
- [StreamStatusType](./literals.md#streamstatustype)
- [StreamViewTypeType](./literals.md#streamviewtypetype)
- [KeyspacesStreamsServiceName](./literals.md#keyspacesstreamsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [GetRecordsInputTypeDef](./type_defs.md#getrecordsinputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetShardIteratorInputTypeDef](./type_defs.md#getsharditeratorinputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ShardFilterTypeDef](./type_defs.md#shardfiltertypedef)
- [KeyspacesMetadataTypeDef](./type_defs.md#keyspacesmetadatatypedef)
- [ListStreamsInputTypeDef](./type_defs.md#liststreamsinputtypedef)
- [StreamTypeDef](./type_defs.md#streamtypedef)
- [SequenceNumberRangeTypeDef](./type_defs.md#sequencenumberrangetypedef)
- [GetShardIteratorOutputTypeDef](./type_defs.md#getsharditeratoroutputtypedef)
- [ListStreamsInputPaginateTypeDef](./type_defs.md#liststreamsinputpaginatetypedef)
- [GetStreamInputPaginateTypeDef](./type_defs.md#getstreaminputpaginatetypedef)
- [GetStreamInputTypeDef](./type_defs.md#getstreaminputtypedef)
- [KeyspacesCellMapDefinitionTypeDef](./type_defs.md#keyspacescellmapdefinitiontypedef)
- [KeyspacesCellTypeDef](./type_defs.md#keyspacescelltypedef)
- [ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef)
- [ShardTypeDef](./type_defs.md#shardtypedef)
- [KeyspacesCellValueTypeDef](./type_defs.md#keyspacescellvaluetypedef)
- [KeyspacesRowTypeDef](./type_defs.md#keyspacesrowtypedef)
- [GetStreamOutputTypeDef](./type_defs.md#getstreamoutputtypedef)
- [RecordTypeDef](./type_defs.md#recordtypedef)
- [GetRecordsOutputTypeDef](./type_defs.md#getrecordsoutputtypedef)

