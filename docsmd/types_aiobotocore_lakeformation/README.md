# LakeFormation module

> [Index](../README.md) > LakeFormation


!!! note ""

    Auto-generated documentation for [LakeFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#lakeformation)
    type annotations stubs module [types-aiobotocore-lakeformation](https://pypi.org/project/types-aiobotocore-lakeformation/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `LakeFormation` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `LakeFormation` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[lakeformation]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[lakeformation]'

# standalone installation
python -m pip install types-aiobotocore-lakeformation
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-lakeformation
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LakeFormationClient

Type annotations and code completion for  `#!python session.create_client("lakeformation")` as [LakeFormationClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# LakeFormationClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.client import LakeFormationClient


session = get_session()
async with session.create_client("lakeformation") as client:
    client: LakeFormationClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("lakeformation").get_paginator("...")`.

```python
# GetWorkUnitsPaginator usage example

from types_aiobotocore_lakeformation.paginator import GetWorkUnitsPaginator

def get_get_work_units_paginator() -> GetWorkUnitsPaginator:
    return client.get_paginator("get_work_units"))
```

- [GetWorkUnitsPaginator](./paginators.md#getworkunitspaginator)
- [ListDataCellsFilterPaginator](./paginators.md#listdatacellsfilterpaginator)
- [ListLFTagExpressionsPaginator](./paginators.md#listlftagexpressionspaginator)
- [ListLFTagsPaginator](./paginators.md#listlftagspaginator)
- [SearchDatabasesByLFTagsPaginator](./paginators.md#searchdatabasesbylftagspaginator)
- [SearchTablesByLFTagsPaginator](./paginators.md#searchtablesbylftagspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ApplicationStatusType usage example

from types_aiobotocore_lakeformation.literals import ApplicationStatusType

def get_value() -> ApplicationStatusType:
    return "DISABLED"
```

- [ApplicationStatusType](./literals.md#applicationstatustype)
- [ComparisonOperatorType](./literals.md#comparisonoperatortype)
- [DataLakeResourceTypeType](./literals.md#datalakeresourcetypetype)
- [EnableStatusType](./literals.md#enablestatustype)
- [FieldNameStringType](./literals.md#fieldnamestringtype)
- [GetWorkUnitsPaginatorName](./literals.md#getworkunitspaginatorname)
- [ListDataCellsFilterPaginatorName](./literals.md#listdatacellsfilterpaginatorname)
- [ListLFTagExpressionsPaginatorName](./literals.md#listlftagexpressionspaginatorname)
- [ListLFTagsPaginatorName](./literals.md#listlftagspaginatorname)
- [OptimizerTypeType](./literals.md#optimizertypetype)
- [PermissionType](./literals.md#permissiontype)
- [PermissionTypeType](./literals.md#permissiontypetype)
- [QueryStateStringType](./literals.md#querystatestringtype)
- [ResourceShareTypeType](./literals.md#resourcesharetypetype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [SearchDatabasesByLFTagsPaginatorName](./literals.md#searchdatabasesbylftagspaginatorname)
- [SearchTablesByLFTagsPaginatorName](./literals.md#searchtablesbylftagspaginatorname)
- [TransactionStatusFilterType](./literals.md#transactionstatusfiltertype)
- [TransactionStatusType](./literals.md#transactionstatustype)
- [TransactionTypeType](./literals.md#transactiontypetype)
- [LakeFormationServiceName](./literals.md#lakeformationservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AddObjectInputTypeDef](./type_defs.md#addobjectinputtypedef)
- [AssumeDecoratedRoleWithSAMLRequestRequestTypeDef](./type_defs.md#assumedecoratedrolewithsamlrequestrequesttypedef)
- [AuditContextTypeDef](./type_defs.md#auditcontexttypedef)
- [ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)
- [DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef)
- [CancelTransactionRequestRequestTypeDef](./type_defs.md#canceltransactionrequestrequesttypedef)
- [CatalogResourceTypeDef](./type_defs.md#catalogresourcetypedef)
- [LFTagPairOutputTypeDef](./type_defs.md#lftagpairoutputtypedef)
- [ColumnWildcardOutputTypeDef](./type_defs.md#columnwildcardoutputtypedef)
- [ColumnWildcardTypeDef](./type_defs.md#columnwildcardtypedef)
- [CommitTransactionRequestRequestTypeDef](./type_defs.md#committransactionrequestrequesttypedef)
- [ConditionTypeDef](./type_defs.md#conditiontypedef)
- [CreateLFTagRequestRequestTypeDef](./type_defs.md#createlftagrequestrequesttypedef)
- [ExternalFilteringConfigurationTypeDef](./type_defs.md#externalfilteringconfigurationtypedef)
- [RowFilterOutputTypeDef](./type_defs.md#rowfilteroutputtypedef)
- [DataCellsFilterResourceTypeDef](./type_defs.md#datacellsfilterresourcetypedef)
- [DataLocationResourceTypeDef](./type_defs.md#datalocationresourcetypedef)
- [DatabaseResourceTypeDef](./type_defs.md#databaseresourcetypedef)
- [DeleteDataCellsFilterRequestRequestTypeDef](./type_defs.md#deletedatacellsfilterrequestrequesttypedef)
- [DeleteLFTagExpressionRequestRequestTypeDef](./type_defs.md#deletelftagexpressionrequestrequesttypedef)
- [DeleteLFTagRequestRequestTypeDef](./type_defs.md#deletelftagrequestrequesttypedef)
- [DeleteLakeFormationIdentityCenterConfigurationRequestRequestTypeDef](./type_defs.md#deletelakeformationidentitycenterconfigurationrequestrequesttypedef)
- [DeleteObjectInputTypeDef](./type_defs.md#deleteobjectinputtypedef)
- [VirtualObjectTypeDef](./type_defs.md#virtualobjecttypedef)
- [DeregisterResourceRequestRequestTypeDef](./type_defs.md#deregisterresourcerequestrequesttypedef)
- [DescribeLakeFormationIdentityCenterConfigurationRequestRequestTypeDef](./type_defs.md#describelakeformationidentitycenterconfigurationrequestrequesttypedef)
- [ExternalFilteringConfigurationOutputTypeDef](./type_defs.md#externalfilteringconfigurationoutputtypedef)
- [DescribeResourceRequestRequestTypeDef](./type_defs.md#describeresourcerequestrequesttypedef)
- [ResourceInfoTypeDef](./type_defs.md#resourceinfotypedef)
- [DescribeTransactionRequestRequestTypeDef](./type_defs.md#describetransactionrequestrequesttypedef)
- [TransactionDescriptionTypeDef](./type_defs.md#transactiondescriptiontypedef)
- [DetailsMapTypeDef](./type_defs.md#detailsmaptypedef)
- [ExecutionStatisticsTypeDef](./type_defs.md#executionstatisticstypedef)
- [ExtendTransactionRequestRequestTypeDef](./type_defs.md#extendtransactionrequestrequesttypedef)
- [FilterConditionTypeDef](./type_defs.md#filterconditiontypedef)
- [GetDataCellsFilterRequestRequestTypeDef](./type_defs.md#getdatacellsfilterrequestrequesttypedef)
- [GetDataLakeSettingsRequestRequestTypeDef](./type_defs.md#getdatalakesettingsrequestrequesttypedef)
- [GetEffectivePermissionsForPathRequestRequestTypeDef](./type_defs.md#geteffectivepermissionsforpathrequestrequesttypedef)
- [GetLFTagExpressionRequestRequestTypeDef](./type_defs.md#getlftagexpressionrequestrequesttypedef)
- [LFTagOutputTypeDef](./type_defs.md#lftagoutputtypedef)
- [GetLFTagRequestRequestTypeDef](./type_defs.md#getlftagrequestrequesttypedef)
- [GetQueryStateRequestRequestTypeDef](./type_defs.md#getquerystaterequestrequesttypedef)
- [GetQueryStatisticsRequestRequestTypeDef](./type_defs.md#getquerystatisticsrequestrequesttypedef)
- [PlanningStatisticsTypeDef](./type_defs.md#planningstatisticstypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef)
- [GetWorkUnitResultsRequestRequestTypeDef](./type_defs.md#getworkunitresultsrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetWorkUnitsRequestRequestTypeDef](./type_defs.md#getworkunitsrequestrequesttypedef)
- [WorkUnitRangeTypeDef](./type_defs.md#workunitrangetypedef)
- [LFTagExpressionResourceTypeDef](./type_defs.md#lftagexpressionresourcetypedef)
- [LFTagKeyResourceOutputTypeDef](./type_defs.md#lftagkeyresourceoutputtypedef)
- [LFTagKeyResourceTypeDef](./type_defs.md#lftagkeyresourcetypedef)
- [LFTagPairTypeDef](./type_defs.md#lftagpairtypedef)
- [LFTagTypeDef](./type_defs.md#lftagtypedef)
- [TableResourceTypeDef](./type_defs.md#tableresourcetypedef)
- [ListLFTagExpressionsRequestRequestTypeDef](./type_defs.md#listlftagexpressionsrequestrequesttypedef)
- [ListLFTagsRequestRequestTypeDef](./type_defs.md#listlftagsrequestrequesttypedef)
- [ListTableStorageOptimizersRequestRequestTypeDef](./type_defs.md#listtablestorageoptimizersrequestrequesttypedef)
- [StorageOptimizerTypeDef](./type_defs.md#storageoptimizertypedef)
- [ListTransactionsRequestRequestTypeDef](./type_defs.md#listtransactionsrequestrequesttypedef)
- [TableObjectTypeDef](./type_defs.md#tableobjecttypedef)
- [RegisterResourceRequestRequestTypeDef](./type_defs.md#registerresourcerequestrequesttypedef)
- [TableResourceOutputTypeDef](./type_defs.md#tableresourceoutputtypedef)
- [RowFilterTypeDef](./type_defs.md#rowfiltertypedef)
- [StartTransactionRequestRequestTypeDef](./type_defs.md#starttransactionrequestrequesttypedef)
- [UpdateLFTagRequestRequestTypeDef](./type_defs.md#updatelftagrequestrequesttypedef)
- [UpdateResourceRequestRequestTypeDef](./type_defs.md#updateresourcerequestrequesttypedef)
- [UpdateTableStorageOptimizerRequestRequestTypeDef](./type_defs.md#updatetablestorageoptimizerrequestrequesttypedef)
- [AssumeDecoratedRoleWithSAMLResponseTypeDef](./type_defs.md#assumedecoratedrolewithsamlresponsetypedef)
- [CommitTransactionResponseTypeDef](./type_defs.md#committransactionresponsetypedef)
- [CreateLakeFormationIdentityCenterConfigurationResponseTypeDef](./type_defs.md#createlakeformationidentitycenterconfigurationresponsetypedef)
- [GetDataLakePrincipalResponseTypeDef](./type_defs.md#getdatalakeprincipalresponsetypedef)
- [GetLFTagResponseTypeDef](./type_defs.md#getlftagresponsetypedef)
- [GetQueryStateResponseTypeDef](./type_defs.md#getquerystateresponsetypedef)
- [GetTemporaryGluePartitionCredentialsResponseTypeDef](./type_defs.md#gettemporarygluepartitioncredentialsresponsetypedef)
- [GetTemporaryGlueTableCredentialsResponseTypeDef](./type_defs.md#gettemporarygluetablecredentialsresponsetypedef)
- [GetWorkUnitResultsResponseTypeDef](./type_defs.md#getworkunitresultsresponsetypedef)
- [StartQueryPlanningResponseTypeDef](./type_defs.md#startqueryplanningresponsetypedef)
- [StartTransactionResponseTypeDef](./type_defs.md#starttransactionresponsetypedef)
- [UpdateTableStorageOptimizerResponseTypeDef](./type_defs.md#updatetablestorageoptimizerresponsetypedef)
- [PrincipalPermissionsOutputTypeDef](./type_defs.md#principalpermissionsoutputtypedef)
- [PrincipalPermissionsTypeDef](./type_defs.md#principalpermissionstypedef)
- [ColumnLFTagTypeDef](./type_defs.md#columnlftagtypedef)
- [LFTagErrorTypeDef](./type_defs.md#lftagerrortypedef)
- [ListLFTagsResponseTypeDef](./type_defs.md#listlftagsresponsetypedef)
- [TableWithColumnsResourceOutputTypeDef](./type_defs.md#tablewithcolumnsresourceoutputtypedef)
- [ColumnWildcardUnionTypeDef](./type_defs.md#columnwildcarduniontypedef)
- [CreateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef](./type_defs.md#createlakeformationidentitycenterconfigurationrequestrequesttypedef)
- [UpdateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef](./type_defs.md#updatelakeformationidentitycenterconfigurationrequestrequesttypedef)
- [DataCellsFilterOutputTypeDef](./type_defs.md#datacellsfilteroutputtypedef)
- [TaggedDatabaseTypeDef](./type_defs.md#taggeddatabasetypedef)
- [WriteOperationTypeDef](./type_defs.md#writeoperationtypedef)
- [DeleteObjectsOnCancelRequestRequestTypeDef](./type_defs.md#deleteobjectsoncancelrequestrequesttypedef)
- [DescribeLakeFormationIdentityCenterConfigurationResponseTypeDef](./type_defs.md#describelakeformationidentitycenterconfigurationresponsetypedef)
- [DescribeResourceResponseTypeDef](./type_defs.md#describeresourceresponsetypedef)
- [ListResourcesResponseTypeDef](./type_defs.md#listresourcesresponsetypedef)
- [DescribeTransactionResponseTypeDef](./type_defs.md#describetransactionresponsetypedef)
- [ListTransactionsResponseTypeDef](./type_defs.md#listtransactionsresponsetypedef)
- [ListResourcesRequestRequestTypeDef](./type_defs.md#listresourcesrequestrequesttypedef)
- [GetLFTagExpressionResponseTypeDef](./type_defs.md#getlftagexpressionresponsetypedef)
- [LFTagExpressionTypeDef](./type_defs.md#lftagexpressiontypedef)
- [LFTagPolicyResourceOutputTypeDef](./type_defs.md#lftagpolicyresourceoutputtypedef)
- [GetQueryStatisticsResponseTypeDef](./type_defs.md#getquerystatisticsresponsetypedef)
- [GetTableObjectsRequestRequestTypeDef](./type_defs.md#gettableobjectsrequestrequesttypedef)
- [QueryPlanningContextTypeDef](./type_defs.md#queryplanningcontexttypedef)
- [QuerySessionContextTypeDef](./type_defs.md#querysessioncontexttypedef)
- [GetTemporaryGluePartitionCredentialsRequestRequestTypeDef](./type_defs.md#gettemporarygluepartitioncredentialsrequestrequesttypedef)
- [GetWorkUnitsRequestPaginateTypeDef](./type_defs.md#getworkunitsrequestpaginatetypedef)
- [ListLFTagExpressionsRequestPaginateTypeDef](./type_defs.md#listlftagexpressionsrequestpaginatetypedef)
- [ListLFTagsRequestPaginateTypeDef](./type_defs.md#listlftagsrequestpaginatetypedef)
- [GetWorkUnitsResponseTypeDef](./type_defs.md#getworkunitsresponsetypedef)
- [LFTagKeyResourceUnionTypeDef](./type_defs.md#lftagkeyresourceuniontypedef)
- [LFTagPairUnionTypeDef](./type_defs.md#lftagpairuniontypedef)
- [LFTagUnionTypeDef](./type_defs.md#lftaguniontypedef)
- [SearchDatabasesByLFTagsRequestPaginateTypeDef](./type_defs.md#searchdatabasesbylftagsrequestpaginatetypedef)
- [SearchDatabasesByLFTagsRequestRequestTypeDef](./type_defs.md#searchdatabasesbylftagsrequestrequesttypedef)
- [SearchTablesByLFTagsRequestPaginateTypeDef](./type_defs.md#searchtablesbylftagsrequestpaginatetypedef)
- [SearchTablesByLFTagsRequestRequestTypeDef](./type_defs.md#searchtablesbylftagsrequestrequesttypedef)
- [UpdateLFTagExpressionRequestRequestTypeDef](./type_defs.md#updatelftagexpressionrequestrequesttypedef)
- [ListDataCellsFilterRequestPaginateTypeDef](./type_defs.md#listdatacellsfilterrequestpaginatetypedef)
- [ListDataCellsFilterRequestRequestTypeDef](./type_defs.md#listdatacellsfilterrequestrequesttypedef)
- [ListTableStorageOptimizersResponseTypeDef](./type_defs.md#listtablestorageoptimizersresponsetypedef)
- [PartitionObjectsTypeDef](./type_defs.md#partitionobjectstypedef)
- [TableResourceUnionTypeDef](./type_defs.md#tableresourceuniontypedef)
- [RowFilterUnionTypeDef](./type_defs.md#rowfilteruniontypedef)
- [DataLakeSettingsOutputTypeDef](./type_defs.md#datalakesettingsoutputtypedef)
- [PrincipalPermissionsUnionTypeDef](./type_defs.md#principalpermissionsuniontypedef)
- [GetResourceLFTagsResponseTypeDef](./type_defs.md#getresourcelftagsresponsetypedef)
- [TaggedTableTypeDef](./type_defs.md#taggedtabletypedef)
- [AddLFTagsToResourceResponseTypeDef](./type_defs.md#addlftagstoresourceresponsetypedef)
- [RemoveLFTagsFromResourceResponseTypeDef](./type_defs.md#removelftagsfromresourceresponsetypedef)
- [TableWithColumnsResourceTypeDef](./type_defs.md#tablewithcolumnsresourcetypedef)
- [GetDataCellsFilterResponseTypeDef](./type_defs.md#getdatacellsfilterresponsetypedef)
- [ListDataCellsFilterResponseTypeDef](./type_defs.md#listdatacellsfilterresponsetypedef)
- [SearchDatabasesByLFTagsResponseTypeDef](./type_defs.md#searchdatabasesbylftagsresponsetypedef)
- [UpdateTableObjectsRequestRequestTypeDef](./type_defs.md#updatetableobjectsrequestrequesttypedef)
- [ListLFTagExpressionsResponseTypeDef](./type_defs.md#listlftagexpressionsresponsetypedef)
- [ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef)
- [StartQueryPlanningRequestRequestTypeDef](./type_defs.md#startqueryplanningrequestrequesttypedef)
- [GetTemporaryGlueTableCredentialsRequestRequestTypeDef](./type_defs.md#gettemporarygluetablecredentialsrequestrequesttypedef)
- [CreateLFTagExpressionRequestRequestTypeDef](./type_defs.md#createlftagexpressionrequestrequesttypedef)
- [LFTagPolicyResourceTypeDef](./type_defs.md#lftagpolicyresourcetypedef)
- [GetTableObjectsResponseTypeDef](./type_defs.md#gettableobjectsresponsetypedef)
- [DataCellsFilterTypeDef](./type_defs.md#datacellsfiltertypedef)
- [GetDataLakeSettingsResponseTypeDef](./type_defs.md#getdatalakesettingsresponsetypedef)
- [DataLakeSettingsTypeDef](./type_defs.md#datalakesettingstypedef)
- [SearchTablesByLFTagsResponseTypeDef](./type_defs.md#searchtablesbylftagsresponsetypedef)
- [TableWithColumnsResourceUnionTypeDef](./type_defs.md#tablewithcolumnsresourceuniontypedef)
- [BatchPermissionsRequestEntryOutputTypeDef](./type_defs.md#batchpermissionsrequestentryoutputtypedef)
- [LakeFormationOptInsInfoTypeDef](./type_defs.md#lakeformationoptinsinfotypedef)
- [PrincipalResourcePermissionsTypeDef](./type_defs.md#principalresourcepermissionstypedef)
- [LFTagPolicyResourceUnionTypeDef](./type_defs.md#lftagpolicyresourceuniontypedef)
- [CreateDataCellsFilterRequestRequestTypeDef](./type_defs.md#createdatacellsfilterrequestrequesttypedef)
- [UpdateDataCellsFilterRequestRequestTypeDef](./type_defs.md#updatedatacellsfilterrequestrequesttypedef)
- [PutDataLakeSettingsRequestRequestTypeDef](./type_defs.md#putdatalakesettingsrequestrequesttypedef)
- [BatchPermissionsFailureEntryTypeDef](./type_defs.md#batchpermissionsfailureentrytypedef)
- [ListLakeFormationOptInsResponseTypeDef](./type_defs.md#listlakeformationoptinsresponsetypedef)
- [GetEffectivePermissionsForPathResponseTypeDef](./type_defs.md#geteffectivepermissionsforpathresponsetypedef)
- [ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [BatchGrantPermissionsResponseTypeDef](./type_defs.md#batchgrantpermissionsresponsetypedef)
- [BatchRevokePermissionsResponseTypeDef](./type_defs.md#batchrevokepermissionsresponsetypedef)
- [AddLFTagsToResourceRequestRequestTypeDef](./type_defs.md#addlftagstoresourcerequestrequesttypedef)
- [CreateLakeFormationOptInRequestRequestTypeDef](./type_defs.md#createlakeformationoptinrequestrequesttypedef)
- [DeleteLakeFormationOptInRequestRequestTypeDef](./type_defs.md#deletelakeformationoptinrequestrequesttypedef)
- [GetResourceLFTagsRequestRequestTypeDef](./type_defs.md#getresourcelftagsrequestrequesttypedef)
- [GrantPermissionsRequestRequestTypeDef](./type_defs.md#grantpermissionsrequestrequesttypedef)
- [ListLakeFormationOptInsRequestRequestTypeDef](./type_defs.md#listlakeformationoptinsrequestrequesttypedef)
- [ListPermissionsRequestRequestTypeDef](./type_defs.md#listpermissionsrequestrequesttypedef)
- [RemoveLFTagsFromResourceRequestRequestTypeDef](./type_defs.md#removelftagsfromresourcerequestrequesttypedef)
- [ResourceUnionTypeDef](./type_defs.md#resourceuniontypedef)
- [RevokePermissionsRequestRequestTypeDef](./type_defs.md#revokepermissionsrequestrequesttypedef)
- [BatchPermissionsRequestEntryTypeDef](./type_defs.md#batchpermissionsrequestentrytypedef)
- [BatchPermissionsRequestEntryUnionTypeDef](./type_defs.md#batchpermissionsrequestentryuniontypedef)
- [BatchRevokePermissionsRequestRequestTypeDef](./type_defs.md#batchrevokepermissionsrequestrequesttypedef)
- [BatchGrantPermissionsRequestRequestTypeDef](./type_defs.md#batchgrantpermissionsrequestrequesttypedef)

