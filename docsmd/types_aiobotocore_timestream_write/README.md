# TimestreamWrite module

> [Index](../README.md) > TimestreamWrite


!!! note ""

    Auto-generated documentation for [TimestreamWrite](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#timestreamwrite)
    type annotations stubs module [types-aiobotocore-timestream-write](https://pypi.org/project/types-aiobotocore-timestream-write/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `TimestreamWrite` service.
1. Use provided commands to install generated packages.



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

```python
# TimestreamWriteClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_timestream_write.client import TimestreamWriteClient


session = get_session()
async with session.create_client("timestream-write") as client:
    client: TimestreamWriteClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BatchLoadDataFormatType usage example

from types_aiobotocore_timestream_write.literals import BatchLoadDataFormatType

def get_value() -> BatchLoadDataFormatType:
    return "CSV"
```

- [BatchLoadDataFormatType](./literals.md#batchloaddataformattype)
- [BatchLoadStatusType](./literals.md#batchloadstatustype)
- [DimensionValueTypeType](./literals.md#dimensionvaluetypetype)
- [MeasureValueTypeType](./literals.md#measurevaluetypetype)
- [PartitionKeyEnforcementLevelType](./literals.md#partitionkeyenforcementleveltype)
- [PartitionKeyTypeType](./literals.md#partitionkeytypetype)
- [S3EncryptionOptionType](./literals.md#s3encryptionoptiontype)
- [ScalarMeasureValueTypeType](./literals.md#scalarmeasurevaluetypetype)
- [TableStatusType](./literals.md#tablestatustype)
- [TimeUnitType](./literals.md#timeunittype)
- [TimestreamWriteServiceName](./literals.md#timestreamwriteservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BatchLoadProgressReportTypeDef](./type_defs.md#batchloadprogressreporttypedef)
- [BatchLoadTaskTypeDef](./type_defs.md#batchloadtasktypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DatabaseTypeDef](./type_defs.md#databasetypedef)
- [RetentionPropertiesTypeDef](./type_defs.md#retentionpropertiestypedef)
- [CsvConfigurationTypeDef](./type_defs.md#csvconfigurationtypedef)
- [DataModelS3ConfigurationTypeDef](./type_defs.md#datamodels3configurationtypedef)
- [DimensionMappingTypeDef](./type_defs.md#dimensionmappingtypedef)
- [DataSourceS3ConfigurationTypeDef](./type_defs.md#datasources3configurationtypedef)
- [DeleteDatabaseRequestTypeDef](./type_defs.md#deletedatabaserequesttypedef)
- [DeleteTableRequestTypeDef](./type_defs.md#deletetablerequesttypedef)
- [DescribeBatchLoadTaskRequestTypeDef](./type_defs.md#describebatchloadtaskrequesttypedef)
- [DescribeDatabaseRequestTypeDef](./type_defs.md#describedatabaserequesttypedef)
- [EndpointTypeDef](./type_defs.md#endpointtypedef)
- [DescribeTableRequestTypeDef](./type_defs.md#describetablerequesttypedef)
- [DimensionTypeDef](./type_defs.md#dimensiontypedef)
- [ListBatchLoadTasksRequestTypeDef](./type_defs.md#listbatchloadtasksrequesttypedef)
- [ListDatabasesRequestTypeDef](./type_defs.md#listdatabasesrequesttypedef)
- [ListTablesRequestTypeDef](./type_defs.md#listtablesrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [S3ConfigurationTypeDef](./type_defs.md#s3configurationtypedef)
- [MeasureValueTypeDef](./type_defs.md#measurevaluetypedef)
- [MultiMeasureAttributeMappingTypeDef](./type_defs.md#multimeasureattributemappingtypedef)
- [PartitionKeyTypeDef](./type_defs.md#partitionkeytypedef)
- [RecordsIngestedTypeDef](./type_defs.md#recordsingestedtypedef)
- [ReportS3ConfigurationTypeDef](./type_defs.md#reports3configurationtypedef)
- [ResumeBatchLoadTaskRequestTypeDef](./type_defs.md#resumebatchloadtaskrequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateDatabaseRequestTypeDef](./type_defs.md#updatedatabaserequesttypedef)
- [CreateBatchLoadTaskResponseTypeDef](./type_defs.md#createbatchloadtaskresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListBatchLoadTasksResponseTypeDef](./type_defs.md#listbatchloadtasksresponsetypedef)
- [CreateDatabaseRequestTypeDef](./type_defs.md#createdatabaserequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [CreateDatabaseResponseTypeDef](./type_defs.md#createdatabaseresponsetypedef)
- [DescribeDatabaseResponseTypeDef](./type_defs.md#describedatabaseresponsetypedef)
- [ListDatabasesResponseTypeDef](./type_defs.md#listdatabasesresponsetypedef)
- [UpdateDatabaseResponseTypeDef](./type_defs.md#updatedatabaseresponsetypedef)
- [DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef)
- [DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef)
- [MagneticStoreRejectedDataLocationTypeDef](./type_defs.md#magneticstorerejecteddatalocationtypedef)
- [RecordTypeDef](./type_defs.md#recordtypedef)
- [MixedMeasureMappingOutputTypeDef](./type_defs.md#mixedmeasuremappingoutputtypedef)
- [MixedMeasureMappingTypeDef](./type_defs.md#mixedmeasuremappingtypedef)
- [MultiMeasureMappingsOutputTypeDef](./type_defs.md#multimeasuremappingsoutputtypedef)
- [MultiMeasureMappingsTypeDef](./type_defs.md#multimeasuremappingstypedef)
- [SchemaOutputTypeDef](./type_defs.md#schemaoutputtypedef)
- [SchemaTypeDef](./type_defs.md#schematypedef)
- [WriteRecordsResponseTypeDef](./type_defs.md#writerecordsresponsetypedef)
- [ReportConfigurationTypeDef](./type_defs.md#reportconfigurationtypedef)
- [MagneticStoreWritePropertiesTypeDef](./type_defs.md#magneticstorewritepropertiestypedef)
- [WriteRecordsRequestTypeDef](./type_defs.md#writerecordsrequesttypedef)
- [DataModelOutputTypeDef](./type_defs.md#datamodeloutputtypedef)
- [DataModelTypeDef](./type_defs.md#datamodeltypedef)
- [SchemaUnionTypeDef](./type_defs.md#schemauniontypedef)
- [TableTypeDef](./type_defs.md#tabletypedef)
- [DataModelConfigurationOutputTypeDef](./type_defs.md#datamodelconfigurationoutputtypedef)
- [DataModelConfigurationTypeDef](./type_defs.md#datamodelconfigurationtypedef)
- [CreateTableRequestTypeDef](./type_defs.md#createtablerequesttypedef)
- [UpdateTableRequestTypeDef](./type_defs.md#updatetablerequesttypedef)
- [CreateTableResponseTypeDef](./type_defs.md#createtableresponsetypedef)
- [DescribeTableResponseTypeDef](./type_defs.md#describetableresponsetypedef)
- [ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef)
- [UpdateTableResponseTypeDef](./type_defs.md#updatetableresponsetypedef)
- [BatchLoadTaskDescriptionTypeDef](./type_defs.md#batchloadtaskdescriptiontypedef)
- [DataModelConfigurationUnionTypeDef](./type_defs.md#datamodelconfigurationuniontypedef)
- [DescribeBatchLoadTaskResponseTypeDef](./type_defs.md#describebatchloadtaskresponsetypedef)
- [CreateBatchLoadTaskRequestTypeDef](./type_defs.md#createbatchloadtaskrequesttypedef)

