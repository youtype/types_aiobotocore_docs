# TimestreamWrite module

> [Index](../README.md) > TimestreamWrite


!!! note ""

    Auto-generated documentation for [TimestreamWrite](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
    type annotations stubs module [types-aiobotocore-timestream-write](https://pypi.org/project/types-aiobotocore-timestream-write/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `TimestreamWrite`.

### From PyPI with pip

Install `types-aiobotocore` for `TimestreamWrite` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[timestream-write]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[timestream-write]'


# standalone installation
python -m pip install types-aiobotocore-timestream-write
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-timestream-write
```

## Usage

Code samples can be found in [Examples](./usage.md).

## TimestreamWriteClient

Type annotations and code completion for  `#!python session.create_client("timestream-write")` as [TimestreamWriteClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_timestream_write.client import TimestreamWriteClient


session = get_session()
async with session.create_client("timestream-write") as client:
    client: TimestreamWriteClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_timestream_write.literals import DimensionValueTypeType

def get_value() -> DimensionValueTypeType:
    return "VARCHAR"
```

- [DimensionValueTypeType](./literals.md#dimensionvaluetypetype)
- [MeasureValueTypeType](./literals.md#measurevaluetypetype)
- [S3EncryptionOptionType](./literals.md#s3encryptionoptiontype)
- [TableStatusType](./literals.md#tablestatustype)
- [TimeUnitType](./literals.md#timeunittype)
- [TimestreamWriteServiceName](./literals.md#timestreamwriteservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_timestream_write.type_defs import CreateDatabaseRequestRequestTypeDef

def get_value() -> CreateDatabaseRequestRequestTypeDef:
    return {
        "DatabaseName": ...,
    }
```

- [CreateDatabaseRequestRequestTypeDef](./type_defs.md#createdatabaserequestrequesttypedef)
- [CreateDatabaseResponseTypeDef](./type_defs.md#createdatabaseresponsetypedef)
- [CreateTableRequestRequestTypeDef](./type_defs.md#createtablerequestrequesttypedef)
- [CreateTableResponseTypeDef](./type_defs.md#createtableresponsetypedef)
- [DatabaseTypeDef](./type_defs.md#databasetypedef)
- [DeleteDatabaseRequestRequestTypeDef](./type_defs.md#deletedatabaserequestrequesttypedef)
- [DeleteTableRequestRequestTypeDef](./type_defs.md#deletetablerequestrequesttypedef)
- [DescribeDatabaseRequestRequestTypeDef](./type_defs.md#describedatabaserequestrequesttypedef)
- [DescribeDatabaseResponseTypeDef](./type_defs.md#describedatabaseresponsetypedef)
- [DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef)
- [DescribeTableRequestRequestTypeDef](./type_defs.md#describetablerequestrequesttypedef)
- [DescribeTableResponseTypeDef](./type_defs.md#describetableresponsetypedef)
- [DimensionTypeDef](./type_defs.md#dimensiontypedef)
- [EndpointTypeDef](./type_defs.md#endpointtypedef)
- [ListDatabasesRequestRequestTypeDef](./type_defs.md#listdatabasesrequestrequesttypedef)
- [ListDatabasesResponseTypeDef](./type_defs.md#listdatabasesresponsetypedef)
- [ListTablesRequestRequestTypeDef](./type_defs.md#listtablesrequestrequesttypedef)
- [ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [MagneticStoreRejectedDataLocationTypeDef](./type_defs.md#magneticstorerejecteddatalocationtypedef)
- [MagneticStoreWritePropertiesTypeDef](./type_defs.md#magneticstorewritepropertiestypedef)
- [MeasureValueTypeDef](./type_defs.md#measurevaluetypedef)
- [RecordTypeDef](./type_defs.md#recordtypedef)
- [RecordsIngestedTypeDef](./type_defs.md#recordsingestedtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [RetentionPropertiesTypeDef](./type_defs.md#retentionpropertiestypedef)
- [S3ConfigurationTypeDef](./type_defs.md#s3configurationtypedef)
- [TableTypeDef](./type_defs.md#tabletypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDatabaseRequestRequestTypeDef](./type_defs.md#updatedatabaserequestrequesttypedef)
- [UpdateDatabaseResponseTypeDef](./type_defs.md#updatedatabaseresponsetypedef)
- [UpdateTableRequestRequestTypeDef](./type_defs.md#updatetablerequestrequesttypedef)
- [UpdateTableResponseTypeDef](./type_defs.md#updatetableresponsetypedef)
- [WriteRecordsRequestRequestTypeDef](./type_defs.md#writerecordsrequestrequesttypedef)
- [WriteRecordsResponseTypeDef](./type_defs.md#writerecordsresponsetypedef)

