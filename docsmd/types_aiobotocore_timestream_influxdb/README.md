# TimestreamInfluxDB module

> [Index](../README.md) > TimestreamInfluxDB


!!! note ""

    Auto-generated documentation for [TimestreamInfluxDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB)
    type annotations stubs module [types-aiobotocore-timestream-influxdb](https://pypi.org/project/types-aiobotocore-timestream-influxdb/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `TimestreamInfluxDB` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[timestream-influxdb]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[timestream-influxdb]'


# standalone installation
python -m pip install types-aiobotocore-timestream-influxdb
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-timestream-influxdb
```

## Usage

Code samples can be found in [Examples](./usage.md).

## TimestreamInfluxDBClient

Type annotations and code completion for  `#!python session.create_client("timestream-influxdb")` as [TimestreamInfluxDBClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Client)

```python
# TimestreamInfluxDBClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_timestream_influxdb.client import TimestreamInfluxDBClient


session = get_session()
async with session.create_client("timestream-influxdb") as client:
    client: TimestreamInfluxDBClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("timestream-influxdb").get_paginator("...")`.

```python
# ListDbInstancesPaginator usage example

from types_aiobotocore_timestream_influxdb.paginator import ListDbInstancesPaginator

def get_list_db_instances_paginator() -> ListDbInstancesPaginator:
    return client.get_paginator("list_db_instances"))
```

- [ListDbInstancesPaginator](./paginators.md#listdbinstancespaginator)
- [ListDbParameterGroupsPaginator](./paginators.md#listdbparametergroupspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DbInstanceTypeType usage example

from types_aiobotocore_timestream_influxdb.literals import DbInstanceTypeType

def get_value() -> DbInstanceTypeType:
    return "db.influx.12xlarge"
```

- [DbInstanceTypeType](./literals.md#dbinstancetypetype)
- [DbStorageTypeType](./literals.md#dbstoragetypetype)
- [DeploymentTypeType](./literals.md#deploymenttypetype)
- [DurationTypeType](./literals.md#durationtypetype)
- [ListDbInstancesPaginatorName](./literals.md#listdbinstancespaginatorname)
- [ListDbParameterGroupsPaginatorName](./literals.md#listdbparametergroupspaginatorname)
- [LogLevelType](./literals.md#logleveltype)
- [StatusType](./literals.md#statustype)
- [TracingTypeType](./literals.md#tracingtypetype)
- [TimestreamInfluxDBServiceName](./literals.md#timestreaminfluxdbservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DbInstanceSummaryTypeDef](./type_defs.md#dbinstancesummarytypedef)
- [DbParameterGroupSummaryTypeDef](./type_defs.md#dbparametergroupsummarytypedef)
- [DeleteDbInstanceInputRequestTypeDef](./type_defs.md#deletedbinstanceinputrequesttypedef)
- [DurationTypeDef](./type_defs.md#durationtypedef)
- [GetDbInstanceInputRequestTypeDef](./type_defs.md#getdbinstanceinputrequesttypedef)
- [GetDbParameterGroupInputRequestTypeDef](./type_defs.md#getdbparametergroupinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDbInstancesInputRequestTypeDef](./type_defs.md#listdbinstancesinputrequesttypedef)
- [ListDbParameterGroupsInputRequestTypeDef](./type_defs.md#listdbparametergroupsinputrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [S3ConfigurationTypeDef](./type_defs.md#s3configurationtypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListDbInstancesOutputTypeDef](./type_defs.md#listdbinstancesoutputtypedef)
- [ListDbParameterGroupsOutputTypeDef](./type_defs.md#listdbparametergroupsoutputtypedef)
- [InfluxDBv2ParametersTypeDef](./type_defs.md#influxdbv2parameterstypedef)
- [ListDbInstancesInputListDbInstancesPaginateTypeDef](./type_defs.md#listdbinstancesinputlistdbinstancespaginatetypedef)
- [ListDbParameterGroupsInputListDbParameterGroupsPaginateTypeDef](./type_defs.md#listdbparametergroupsinputlistdbparametergroupspaginatetypedef)
- [LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef)
- [ParametersTypeDef](./type_defs.md#parameterstypedef)
- [CreateDbInstanceInputRequestTypeDef](./type_defs.md#createdbinstanceinputrequesttypedef)
- [CreateDbInstanceOutputTypeDef](./type_defs.md#createdbinstanceoutputtypedef)
- [DeleteDbInstanceOutputTypeDef](./type_defs.md#deletedbinstanceoutputtypedef)
- [GetDbInstanceOutputTypeDef](./type_defs.md#getdbinstanceoutputtypedef)
- [UpdateDbInstanceInputRequestTypeDef](./type_defs.md#updatedbinstanceinputrequesttypedef)
- [UpdateDbInstanceOutputTypeDef](./type_defs.md#updatedbinstanceoutputtypedef)
- [CreateDbParameterGroupInputRequestTypeDef](./type_defs.md#createdbparametergroupinputrequesttypedef)
- [CreateDbParameterGroupOutputTypeDef](./type_defs.md#createdbparametergroupoutputtypedef)
- [GetDbParameterGroupOutputTypeDef](./type_defs.md#getdbparametergroupoutputtypedef)

