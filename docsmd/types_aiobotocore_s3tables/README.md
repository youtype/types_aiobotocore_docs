# S3Tables module

> [Index](../README.md) > S3Tables


!!! note ""

    Auto-generated documentation for [S3Tables](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables.html#s3tables)
    type annotations stubs module [types-aiobotocore-s3tables](https://pypi.org/project/types-aiobotocore-s3tables/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `S3Tables` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `S3Tables` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[s3tables]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[s3tables]'

# standalone installation
python -m pip install types-aiobotocore-s3tables
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-s3tables
```

## Usage

Code samples can be found in [Examples](./usage.md).

## S3TablesClient

Type annotations and code completion for  `#!python session.create_client("s3tables")` as [S3TablesClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables.html#S3Tables.Client)

```python
# S3TablesClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3tables.client import S3TablesClient


session = get_session()
async with session.create_client("s3tables") as client:
    client: S3TablesClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("s3tables").get_paginator("...")`.

```python
# ListNamespacesPaginator usage example

from types_aiobotocore_s3tables.paginator import ListNamespacesPaginator

def get_list_namespaces_paginator() -> ListNamespacesPaginator:
    return client.get_paginator("list_namespaces"))
```

- [ListNamespacesPaginator](./paginators.md#listnamespacespaginator)
- [ListTableBucketsPaginator](./paginators.md#listtablebucketspaginator)
- [ListTablesPaginator](./paginators.md#listtablespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# JobStatusType usage example

from types_aiobotocore_s3tables.literals import JobStatusType

def get_value() -> JobStatusType:
    return "Disabled"
```

- [JobStatusType](./literals.md#jobstatustype)
- [ListNamespacesPaginatorName](./literals.md#listnamespacespaginatorname)
- [ListTableBucketsPaginatorName](./literals.md#listtablebucketspaginatorname)
- [ListTablesPaginatorName](./literals.md#listtablespaginatorname)
- [MaintenanceStatusType](./literals.md#maintenancestatustype)
- [OpenTableFormatType](./literals.md#opentableformattype)
- [TableBucketMaintenanceTypeType](./literals.md#tablebucketmaintenancetypetype)
- [TableMaintenanceJobTypeType](./literals.md#tablemaintenancejobtypetype)
- [TableMaintenanceTypeType](./literals.md#tablemaintenancetypetype)
- [TableTypeType](./literals.md#tabletypetype)
- [S3TablesServiceName](./literals.md#s3tablesservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CreateNamespaceRequestRequestTypeDef](./type_defs.md#createnamespacerequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateTableBucketRequestRequestTypeDef](./type_defs.md#createtablebucketrequestrequesttypedef)
- [CreateTableRequestRequestTypeDef](./type_defs.md#createtablerequestrequesttypedef)
- [DeleteNamespaceRequestRequestTypeDef](./type_defs.md#deletenamespacerequestrequesttypedef)
- [DeleteTableBucketPolicyRequestRequestTypeDef](./type_defs.md#deletetablebucketpolicyrequestrequesttypedef)
- [DeleteTableBucketRequestRequestTypeDef](./type_defs.md#deletetablebucketrequestrequesttypedef)
- [DeleteTablePolicyRequestRequestTypeDef](./type_defs.md#deletetablepolicyrequestrequesttypedef)
- [DeleteTableRequestRequestTypeDef](./type_defs.md#deletetablerequestrequesttypedef)
- [GetNamespaceRequestRequestTypeDef](./type_defs.md#getnamespacerequestrequesttypedef)
- [GetTableBucketMaintenanceConfigurationRequestRequestTypeDef](./type_defs.md#gettablebucketmaintenanceconfigurationrequestrequesttypedef)
- [GetTableBucketPolicyRequestRequestTypeDef](./type_defs.md#gettablebucketpolicyrequestrequesttypedef)
- [GetTableBucketRequestRequestTypeDef](./type_defs.md#gettablebucketrequestrequesttypedef)
- [GetTableMaintenanceConfigurationRequestRequestTypeDef](./type_defs.md#gettablemaintenanceconfigurationrequestrequesttypedef)
- [GetTableMaintenanceJobStatusRequestRequestTypeDef](./type_defs.md#gettablemaintenancejobstatusrequestrequesttypedef)
- [TableMaintenanceJobStatusValueTypeDef](./type_defs.md#tablemaintenancejobstatusvaluetypedef)
- [GetTableMetadataLocationRequestRequestTypeDef](./type_defs.md#gettablemetadatalocationrequestrequesttypedef)
- [GetTablePolicyRequestRequestTypeDef](./type_defs.md#gettablepolicyrequestrequesttypedef)
- [GetTableRequestRequestTypeDef](./type_defs.md#gettablerequestrequesttypedef)
- [IcebergCompactionSettingsTypeDef](./type_defs.md#icebergcompactionsettingstypedef)
- [IcebergSnapshotManagementSettingsTypeDef](./type_defs.md#icebergsnapshotmanagementsettingstypedef)
- [IcebergUnreferencedFileRemovalSettingsTypeDef](./type_defs.md#icebergunreferencedfileremovalsettingstypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListNamespacesRequestRequestTypeDef](./type_defs.md#listnamespacesrequestrequesttypedef)
- [NamespaceSummaryTypeDef](./type_defs.md#namespacesummarytypedef)
- [ListTableBucketsRequestRequestTypeDef](./type_defs.md#listtablebucketsrequestrequesttypedef)
- [TableBucketSummaryTypeDef](./type_defs.md#tablebucketsummarytypedef)
- [ListTablesRequestRequestTypeDef](./type_defs.md#listtablesrequestrequesttypedef)
- [TableSummaryTypeDef](./type_defs.md#tablesummarytypedef)
- [PutTableBucketPolicyRequestRequestTypeDef](./type_defs.md#puttablebucketpolicyrequestrequesttypedef)
- [PutTablePolicyRequestRequestTypeDef](./type_defs.md#puttablepolicyrequestrequesttypedef)
- [RenameTableRequestRequestTypeDef](./type_defs.md#renametablerequestrequesttypedef)
- [UpdateTableMetadataLocationRequestRequestTypeDef](./type_defs.md#updatetablemetadatalocationrequestrequesttypedef)
- [CreateNamespaceResponseTypeDef](./type_defs.md#createnamespaceresponsetypedef)
- [CreateTableBucketResponseTypeDef](./type_defs.md#createtablebucketresponsetypedef)
- [CreateTableResponseTypeDef](./type_defs.md#createtableresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetNamespaceResponseTypeDef](./type_defs.md#getnamespaceresponsetypedef)
- [GetTableBucketPolicyResponseTypeDef](./type_defs.md#gettablebucketpolicyresponsetypedef)
- [GetTableBucketResponseTypeDef](./type_defs.md#gettablebucketresponsetypedef)
- [GetTableMetadataLocationResponseTypeDef](./type_defs.md#gettablemetadatalocationresponsetypedef)
- [GetTablePolicyResponseTypeDef](./type_defs.md#gettablepolicyresponsetypedef)
- [GetTableResponseTypeDef](./type_defs.md#gettableresponsetypedef)
- [UpdateTableMetadataLocationResponseTypeDef](./type_defs.md#updatetablemetadatalocationresponsetypedef)
- [GetTableMaintenanceJobStatusResponseTypeDef](./type_defs.md#gettablemaintenancejobstatusresponsetypedef)
- [TableMaintenanceSettingsTypeDef](./type_defs.md#tablemaintenancesettingstypedef)
- [TableBucketMaintenanceSettingsTypeDef](./type_defs.md#tablebucketmaintenancesettingstypedef)
- [ListNamespacesRequestPaginateTypeDef](./type_defs.md#listnamespacesrequestpaginatetypedef)
- [ListTableBucketsRequestPaginateTypeDef](./type_defs.md#listtablebucketsrequestpaginatetypedef)
- [ListTablesRequestPaginateTypeDef](./type_defs.md#listtablesrequestpaginatetypedef)
- [ListNamespacesResponseTypeDef](./type_defs.md#listnamespacesresponsetypedef)
- [ListTableBucketsResponseTypeDef](./type_defs.md#listtablebucketsresponsetypedef)
- [ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef)
- [TableMaintenanceConfigurationValueTypeDef](./type_defs.md#tablemaintenanceconfigurationvaluetypedef)
- [TableBucketMaintenanceConfigurationValueTypeDef](./type_defs.md#tablebucketmaintenanceconfigurationvaluetypedef)
- [GetTableMaintenanceConfigurationResponseTypeDef](./type_defs.md#gettablemaintenanceconfigurationresponsetypedef)
- [PutTableMaintenanceConfigurationRequestRequestTypeDef](./type_defs.md#puttablemaintenanceconfigurationrequestrequesttypedef)
- [GetTableBucketMaintenanceConfigurationResponseTypeDef](./type_defs.md#gettablebucketmaintenanceconfigurationresponsetypedef)
- [PutTableBucketMaintenanceConfigurationRequestRequestTypeDef](./type_defs.md#puttablebucketmaintenanceconfigurationrequestrequesttypedef)

