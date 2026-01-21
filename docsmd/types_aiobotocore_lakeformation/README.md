# LakeFormation module

> [Index](../README.md) > LakeFormation


!!! note ""

    Auto-generated documentation for [LakeFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#lakeformation)
    type annotations stubs module [types-aiobotocore-lakeformation](https://pypi.org/project/types-aiobotocore-lakeformation/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
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
- [CredentialsScopeType](./literals.md#credentialsscopetype)
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
- [ServiceAuthorizationType](./literals.md#serviceauthorizationtype)
- [TransactionStatusFilterType](./literals.md#transactionstatusfiltertype)
- [TransactionStatusType](./literals.md#transactionstatustype)
- [TransactionTypeType](./literals.md#transactiontypetype)
- [VerificationStatusType](./literals.md#verificationstatustype)
- [LakeFormationServiceName](./literals.md#lakeformationservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AddObjectInputTypeDef](./type_defs.md#addobjectinputtypedef)
- [AssumeDecoratedRoleWithSAMLRequestTypeDef](./type_defs.md#assumedecoratedrolewithsamlrequesttypedef)
- [AuditContextTypeDef](./type_defs.md#auditcontexttypedef)
- [ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)
- [ConditionTypeDef](./type_defs.md#conditiontypedef)
- [DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef)
- [CancelTransactionRequestTypeDef](./type_defs.md#canceltransactionrequesttypedef)
- [CatalogResourceTypeDef](./type_defs.md#catalogresourcetypedef)
- [LFTagPairOutputTypeDef](./type_defs.md#lftagpairoutputtypedef)
- [ColumnWildcardOutputTypeDef](./type_defs.md#columnwildcardoutputtypedef)
- [ColumnWildcardTypeDef](./type_defs.md#columnwildcardtypedef)
- [CommitTransactionRequestTypeDef](./type_defs.md#committransactionrequesttypedef)
- [CreateLFTagRequestTypeDef](./type_defs.md#createlftagrequesttypedef)
- [RowFilterOutputTypeDef](./type_defs.md#rowfilteroutputtypedef)
- [DataCellsFilterResourceTypeDef](./type_defs.md#datacellsfilterresourcetypedef)
- [RowFilterTypeDef](./type_defs.md#rowfiltertypedef)
- [DataLocationResourceTypeDef](./type_defs.md#datalocationresourcetypedef)
- [DatabaseResourceTypeDef](./type_defs.md#databaseresourcetypedef)
- [DeleteDataCellsFilterRequestTypeDef](./type_defs.md#deletedatacellsfilterrequesttypedef)
- [DeleteLFTagExpressionRequestTypeDef](./type_defs.md#deletelftagexpressionrequesttypedef)
- [DeleteLFTagRequestTypeDef](./type_defs.md#deletelftagrequesttypedef)
- [DeleteLakeFormationIdentityCenterConfigurationRequestTypeDef](./type_defs.md#deletelakeformationidentitycenterconfigurationrequesttypedef)
- [DeleteObjectInputTypeDef](./type_defs.md#deleteobjectinputtypedef)
- [VirtualObjectTypeDef](./type_defs.md#virtualobjecttypedef)
- [DeregisterResourceRequestTypeDef](./type_defs.md#deregisterresourcerequesttypedef)
- [DescribeLakeFormationIdentityCenterConfigurationRequestTypeDef](./type_defs.md#describelakeformationidentitycenterconfigurationrequesttypedef)
- [ExternalFilteringConfigurationOutputTypeDef](./type_defs.md#externalfilteringconfigurationoutputtypedef)
- [DescribeResourceRequestTypeDef](./type_defs.md#describeresourcerequesttypedef)
- [ResourceInfoTypeDef](./type_defs.md#resourceinfotypedef)
- [DescribeTransactionRequestTypeDef](./type_defs.md#describetransactionrequesttypedef)
- [TransactionDescriptionTypeDef](./type_defs.md#transactiondescriptiontypedef)
- [DetailsMapTypeDef](./type_defs.md#detailsmaptypedef)
- [ExecutionStatisticsTypeDef](./type_defs.md#executionstatisticstypedef)
- [ExtendTransactionRequestTypeDef](./type_defs.md#extendtransactionrequesttypedef)
- [ExternalFilteringConfigurationTypeDef](./type_defs.md#externalfilteringconfigurationtypedef)
- [FilterConditionTypeDef](./type_defs.md#filterconditiontypedef)
- [GetDataCellsFilterRequestTypeDef](./type_defs.md#getdatacellsfilterrequesttypedef)
- [GetDataLakeSettingsRequestTypeDef](./type_defs.md#getdatalakesettingsrequesttypedef)
- [GetEffectivePermissionsForPathRequestTypeDef](./type_defs.md#geteffectivepermissionsforpathrequesttypedef)
- [GetLFTagExpressionRequestTypeDef](./type_defs.md#getlftagexpressionrequesttypedef)
- [LFTagOutputTypeDef](./type_defs.md#lftagoutputtypedef)
- [GetLFTagRequestTypeDef](./type_defs.md#getlftagrequesttypedef)
- [GetQueryStateRequestTypeDef](./type_defs.md#getquerystaterequesttypedef)
- [GetQueryStatisticsRequestTypeDef](./type_defs.md#getquerystatisticsrequesttypedef)
- [PlanningStatisticsTypeDef](./type_defs.md#planningstatisticstypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [TemporaryCredentialsTypeDef](./type_defs.md#temporarycredentialstypedef)
- [PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef)
- [GetWorkUnitResultsRequestTypeDef](./type_defs.md#getworkunitresultsrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetWorkUnitsRequestTypeDef](./type_defs.md#getworkunitsrequesttypedef)
- [WorkUnitRangeTypeDef](./type_defs.md#workunitrangetypedef)
- [LFTagExpressionResourceTypeDef](./type_defs.md#lftagexpressionresourcetypedef)
- [LFTagKeyResourceOutputTypeDef](./type_defs.md#lftagkeyresourceoutputtypedef)
- [LFTagKeyResourceTypeDef](./type_defs.md#lftagkeyresourcetypedef)
- [LFTagPairTypeDef](./type_defs.md#lftagpairtypedef)
- [LFTagTypeDef](./type_defs.md#lftagtypedef)
- [ListLFTagExpressionsRequestTypeDef](./type_defs.md#listlftagexpressionsrequesttypedef)
- [ListLFTagsRequestTypeDef](./type_defs.md#listlftagsrequesttypedef)
- [ListTableStorageOptimizersRequestTypeDef](./type_defs.md#listtablestorageoptimizersrequesttypedef)
- [StorageOptimizerTypeDef](./type_defs.md#storageoptimizertypedef)
- [ListTransactionsRequestTypeDef](./type_defs.md#listtransactionsrequesttypedef)
- [TableObjectTypeDef](./type_defs.md#tableobjecttypedef)
- [RedshiftConnectTypeDef](./type_defs.md#redshiftconnecttypedef)
- [RegisterResourceRequestTypeDef](./type_defs.md#registerresourcerequesttypedef)
- [TableResourceOutputTypeDef](./type_defs.md#tableresourceoutputtypedef)
- [StartTransactionRequestTypeDef](./type_defs.md#starttransactionrequesttypedef)
- [TableResourceTypeDef](./type_defs.md#tableresourcetypedef)
- [UpdateLFTagRequestTypeDef](./type_defs.md#updatelftagrequesttypedef)
- [UpdateResourceRequestTypeDef](./type_defs.md#updateresourcerequesttypedef)
- [UpdateTableStorageOptimizerRequestTypeDef](./type_defs.md#updatetablestorageoptimizerrequesttypedef)
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
- [GetTemporaryDataLocationCredentialsRequestTypeDef](./type_defs.md#gettemporarydatalocationcredentialsrequesttypedef)
- [PrincipalPermissionsOutputTypeDef](./type_defs.md#principalpermissionsoutputtypedef)
- [PrincipalPermissionsTypeDef](./type_defs.md#principalpermissionstypedef)
- [ColumnLFTagTypeDef](./type_defs.md#columnlftagtypedef)
- [LFTagErrorTypeDef](./type_defs.md#lftagerrortypedef)
- [ListLFTagsResponseTypeDef](./type_defs.md#listlftagsresponsetypedef)
- [TableWithColumnsResourceOutputTypeDef](./type_defs.md#tablewithcolumnsresourceoutputtypedef)
- [ColumnWildcardUnionTypeDef](./type_defs.md#columnwildcarduniontypedef)
- [DataCellsFilterOutputTypeDef](./type_defs.md#datacellsfilteroutputtypedef)
- [DataCellsFilterTypeDef](./type_defs.md#datacellsfiltertypedef)
- [TaggedDatabaseTypeDef](./type_defs.md#taggeddatabasetypedef)
- [WriteOperationTypeDef](./type_defs.md#writeoperationtypedef)
- [DeleteObjectsOnCancelRequestTypeDef](./type_defs.md#deleteobjectsoncancelrequesttypedef)
- [DescribeResourceResponseTypeDef](./type_defs.md#describeresourceresponsetypedef)
- [ListResourcesResponseTypeDef](./type_defs.md#listresourcesresponsetypedef)
- [DescribeTransactionResponseTypeDef](./type_defs.md#describetransactionresponsetypedef)
- [ListTransactionsResponseTypeDef](./type_defs.md#listtransactionsresponsetypedef)
- [ExternalFilteringConfigurationUnionTypeDef](./type_defs.md#externalfilteringconfigurationuniontypedef)
- [ListResourcesRequestTypeDef](./type_defs.md#listresourcesrequesttypedef)
- [GetLFTagExpressionResponseTypeDef](./type_defs.md#getlftagexpressionresponsetypedef)
- [LFTagExpressionTypeDef](./type_defs.md#lftagexpressiontypedef)
- [LFTagPolicyResourceOutputTypeDef](./type_defs.md#lftagpolicyresourceoutputtypedef)
- [GetQueryStatisticsResponseTypeDef](./type_defs.md#getquerystatisticsresponsetypedef)
- [GetTableObjectsRequestTypeDef](./type_defs.md#gettableobjectsrequesttypedef)
- [QueryPlanningContextTypeDef](./type_defs.md#queryplanningcontexttypedef)
- [QuerySessionContextTypeDef](./type_defs.md#querysessioncontexttypedef)
- [GetTemporaryDataLocationCredentialsResponseTypeDef](./type_defs.md#gettemporarydatalocationcredentialsresponsetypedef)
- [GetTemporaryGluePartitionCredentialsRequestTypeDef](./type_defs.md#gettemporarygluepartitioncredentialsrequesttypedef)
- [GetWorkUnitsRequestPaginateTypeDef](./type_defs.md#getworkunitsrequestpaginatetypedef)
- [ListLFTagExpressionsRequestPaginateTypeDef](./type_defs.md#listlftagexpressionsrequestpaginatetypedef)
- [ListLFTagsRequestPaginateTypeDef](./type_defs.md#listlftagsrequestpaginatetypedef)
- [GetWorkUnitsResponseTypeDef](./type_defs.md#getworkunitsresponsetypedef)
- [LFTagKeyResourceUnionTypeDef](./type_defs.md#lftagkeyresourceuniontypedef)
- [LFTagPairUnionTypeDef](./type_defs.md#lftagpairuniontypedef)
- [LFTagUnionTypeDef](./type_defs.md#lftaguniontypedef)
- [ListTableStorageOptimizersResponseTypeDef](./type_defs.md#listtablestorageoptimizersresponsetypedef)
- [PartitionObjectsTypeDef](./type_defs.md#partitionobjectstypedef)
- [RedshiftScopeUnionTypeDef](./type_defs.md#redshiftscopeuniontypedef)
- [TableResourceUnionTypeDef](./type_defs.md#tableresourceuniontypedef)
- [DataLakeSettingsOutputTypeDef](./type_defs.md#datalakesettingsoutputtypedef)
- [DataLakeSettingsTypeDef](./type_defs.md#datalakesettingstypedef)
- [GetResourceLFTagsResponseTypeDef](./type_defs.md#getresourcelftagsresponsetypedef)
- [TaggedTableTypeDef](./type_defs.md#taggedtabletypedef)
- [AddLFTagsToResourceResponseTypeDef](./type_defs.md#addlftagstoresourceresponsetypedef)
- [RemoveLFTagsFromResourceResponseTypeDef](./type_defs.md#removelftagsfromresourceresponsetypedef)
- [TableWithColumnsResourceTypeDef](./type_defs.md#tablewithcolumnsresourcetypedef)
- [GetDataCellsFilterResponseTypeDef](./type_defs.md#getdatacellsfilterresponsetypedef)
- [ListDataCellsFilterResponseTypeDef](./type_defs.md#listdatacellsfilterresponsetypedef)
- [DataCellsFilterUnionTypeDef](./type_defs.md#datacellsfilteruniontypedef)
- [SearchDatabasesByLFTagsResponseTypeDef](./type_defs.md#searchdatabasesbylftagsresponsetypedef)
- [UpdateTableObjectsRequestTypeDef](./type_defs.md#updatetableobjectsrequesttypedef)
- [ListLFTagExpressionsResponseTypeDef](./type_defs.md#listlftagexpressionsresponsetypedef)
- [ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef)
- [StartQueryPlanningRequestTypeDef](./type_defs.md#startqueryplanningrequesttypedef)
- [GetTemporaryGlueTableCredentialsRequestTypeDef](./type_defs.md#gettemporarygluetablecredentialsrequesttypedef)
- [CreateLFTagExpressionRequestTypeDef](./type_defs.md#createlftagexpressionrequesttypedef)
- [LFTagPolicyResourceTypeDef](./type_defs.md#lftagpolicyresourcetypedef)
- [SearchDatabasesByLFTagsRequestPaginateTypeDef](./type_defs.md#searchdatabasesbylftagsrequestpaginatetypedef)
- [SearchDatabasesByLFTagsRequestTypeDef](./type_defs.md#searchdatabasesbylftagsrequesttypedef)
- [SearchTablesByLFTagsRequestPaginateTypeDef](./type_defs.md#searchtablesbylftagsrequestpaginatetypedef)
- [SearchTablesByLFTagsRequestTypeDef](./type_defs.md#searchtablesbylftagsrequesttypedef)
- [UpdateLFTagExpressionRequestTypeDef](./type_defs.md#updatelftagexpressionrequesttypedef)
- [GetTableObjectsResponseTypeDef](./type_defs.md#gettableobjectsresponsetypedef)
- [ServiceIntegrationUnionOutputTypeDef](./type_defs.md#serviceintegrationunionoutputtypedef)
- [ServiceIntegrationUnionTypeDef](./type_defs.md#serviceintegrationuniontypedef)
- [ListDataCellsFilterRequestPaginateTypeDef](./type_defs.md#listdatacellsfilterrequestpaginatetypedef)
- [ListDataCellsFilterRequestTypeDef](./type_defs.md#listdatacellsfilterrequesttypedef)
- [GetDataLakeSettingsResponseTypeDef](./type_defs.md#getdatalakesettingsresponsetypedef)
- [DataLakeSettingsUnionTypeDef](./type_defs.md#datalakesettingsuniontypedef)
- [SearchTablesByLFTagsResponseTypeDef](./type_defs.md#searchtablesbylftagsresponsetypedef)
- [TableWithColumnsResourceUnionTypeDef](./type_defs.md#tablewithcolumnsresourceuniontypedef)
- [CreateDataCellsFilterRequestTypeDef](./type_defs.md#createdatacellsfilterrequesttypedef)
- [UpdateDataCellsFilterRequestTypeDef](./type_defs.md#updatedatacellsfilterrequesttypedef)
- [BatchPermissionsRequestEntryOutputTypeDef](./type_defs.md#batchpermissionsrequestentryoutputtypedef)
- [LakeFormationOptInsInfoTypeDef](./type_defs.md#lakeformationoptinsinfotypedef)
- [PrincipalResourcePermissionsTypeDef](./type_defs.md#principalresourcepermissionstypedef)
- [LFTagPolicyResourceUnionTypeDef](./type_defs.md#lftagpolicyresourceuniontypedef)
- [DescribeLakeFormationIdentityCenterConfigurationResponseTypeDef](./type_defs.md#describelakeformationidentitycenterconfigurationresponsetypedef)
- [ServiceIntegrationUnionUnionTypeDef](./type_defs.md#serviceintegrationunionuniontypedef)
- [PutDataLakeSettingsRequestTypeDef](./type_defs.md#putdatalakesettingsrequesttypedef)
- [BatchPermissionsFailureEntryTypeDef](./type_defs.md#batchpermissionsfailureentrytypedef)
- [ListLakeFormationOptInsResponseTypeDef](./type_defs.md#listlakeformationoptinsresponsetypedef)
- [GetEffectivePermissionsForPathResponseTypeDef](./type_defs.md#geteffectivepermissionsforpathresponsetypedef)
- [ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [CreateLakeFormationIdentityCenterConfigurationRequestTypeDef](./type_defs.md#createlakeformationidentitycenterconfigurationrequesttypedef)
- [UpdateLakeFormationIdentityCenterConfigurationRequestTypeDef](./type_defs.md#updatelakeformationidentitycenterconfigurationrequesttypedef)
- [BatchGrantPermissionsResponseTypeDef](./type_defs.md#batchgrantpermissionsresponsetypedef)
- [BatchRevokePermissionsResponseTypeDef](./type_defs.md#batchrevokepermissionsresponsetypedef)
- [ResourceUnionTypeDef](./type_defs.md#resourceuniontypedef)
- [AddLFTagsToResourceRequestTypeDef](./type_defs.md#addlftagstoresourcerequesttypedef)
- [BatchPermissionsRequestEntryTypeDef](./type_defs.md#batchpermissionsrequestentrytypedef)
- [CreateLakeFormationOptInRequestTypeDef](./type_defs.md#createlakeformationoptinrequesttypedef)
- [DeleteLakeFormationOptInRequestTypeDef](./type_defs.md#deletelakeformationoptinrequesttypedef)
- [GetResourceLFTagsRequestTypeDef](./type_defs.md#getresourcelftagsrequesttypedef)
- [GrantPermissionsRequestTypeDef](./type_defs.md#grantpermissionsrequesttypedef)
- [ListLakeFormationOptInsRequestTypeDef](./type_defs.md#listlakeformationoptinsrequesttypedef)
- [ListPermissionsRequestTypeDef](./type_defs.md#listpermissionsrequesttypedef)
- [RemoveLFTagsFromResourceRequestTypeDef](./type_defs.md#removelftagsfromresourcerequesttypedef)
- [RevokePermissionsRequestTypeDef](./type_defs.md#revokepermissionsrequesttypedef)
- [BatchPermissionsRequestEntryUnionTypeDef](./type_defs.md#batchpermissionsrequestentryuniontypedef)
- [BatchGrantPermissionsRequestTypeDef](./type_defs.md#batchgrantpermissionsrequesttypedef)
- [BatchRevokePermissionsRequestTypeDef](./type_defs.md#batchrevokepermissionsrequesttypedef)

