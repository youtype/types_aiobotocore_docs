# Athena module

> [Index](../README.md) > Athena


!!! note ""

    Auto-generated documentation for [Athena](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
    type annotations stubs module [types-aiobotocore-athena](https://pypi.org/project/types-aiobotocore-athena/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Athena` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[athena]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[athena]'


# standalone installation
python -m pip install types-aiobotocore-athena
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-athena
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AthenaClient

Type annotations and code completion for  `#!python session.create_client("athena")` as [AthenaClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client)

```python
# AthenaClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_athena.client import AthenaClient


session = get_session()
async with session.create_client("athena") as client:
    client: AthenaClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("athena").get_paginator("...")`.

```python
# GetQueryResultsPaginator usage example

from types_aiobotocore_athena.paginator import GetQueryResultsPaginator

def get_get_query_results_paginator() -> GetQueryResultsPaginator:
    return client.get_paginator("get_query_results"))
```

- [GetQueryResultsPaginator](./paginators.md#getqueryresultspaginator)
- [ListDataCatalogsPaginator](./paginators.md#listdatacatalogspaginator)
- [ListDatabasesPaginator](./paginators.md#listdatabasespaginator)
- [ListNamedQueriesPaginator](./paginators.md#listnamedqueriespaginator)
- [ListQueryExecutionsPaginator](./paginators.md#listqueryexecutionspaginator)
- [ListTableMetadataPaginator](./paginators.md#listtablemetadatapaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CalculationExecutionStateType usage example

from types_aiobotocore_athena.literals import CalculationExecutionStateType

def get_value() -> CalculationExecutionStateType:
    return "CANCELED"
```

- [CalculationExecutionStateType](./literals.md#calculationexecutionstatetype)
- [CapacityAllocationStatusType](./literals.md#capacityallocationstatustype)
- [CapacityReservationStatusType](./literals.md#capacityreservationstatustype)
- [ColumnNullableType](./literals.md#columnnullabletype)
- [DataCatalogTypeType](./literals.md#datacatalogtypetype)
- [EncryptionOptionType](./literals.md#encryptionoptiontype)
- [ExecutorStateType](./literals.md#executorstatetype)
- [ExecutorTypeType](./literals.md#executortypetype)
- [GetQueryResultsPaginatorName](./literals.md#getqueryresultspaginatorname)
- [ListDataCatalogsPaginatorName](./literals.md#listdatacatalogspaginatorname)
- [ListDatabasesPaginatorName](./literals.md#listdatabasespaginatorname)
- [ListNamedQueriesPaginatorName](./literals.md#listnamedqueriespaginatorname)
- [ListQueryExecutionsPaginatorName](./literals.md#listqueryexecutionspaginatorname)
- [ListTableMetadataPaginatorName](./literals.md#listtablemetadatapaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [NotebookTypeType](./literals.md#notebooktypetype)
- [QueryExecutionStateType](./literals.md#queryexecutionstatetype)
- [S3AclOptionType](./literals.md#s3acloptiontype)
- [SessionStateType](./literals.md#sessionstatetype)
- [StatementTypeType](./literals.md#statementtypetype)
- [WorkGroupStateType](./literals.md#workgroupstatetype)
- [AthenaServiceName](./literals.md#athenaservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AclConfigurationTypeDef](./type_defs.md#aclconfigurationtypedef)
- [ApplicationDPUSizesTypeDef](./type_defs.md#applicationdpusizestypedef)
- [AthenaErrorTypeDef](./type_defs.md#athenaerrortypedef)
- [BatchGetNamedQueryInputRequestTypeDef](./type_defs.md#batchgetnamedqueryinputrequesttypedef)
- [NamedQueryTypeDef](./type_defs.md#namedquerytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [UnprocessedNamedQueryIdTypeDef](./type_defs.md#unprocessednamedqueryidtypedef)
- [BatchGetPreparedStatementInputRequestTypeDef](./type_defs.md#batchgetpreparedstatementinputrequesttypedef)
- [PreparedStatementTypeDef](./type_defs.md#preparedstatementtypedef)
- [UnprocessedPreparedStatementNameTypeDef](./type_defs.md#unprocessedpreparedstatementnametypedef)
- [BatchGetQueryExecutionInputRequestTypeDef](./type_defs.md#batchgetqueryexecutioninputrequesttypedef)
- [UnprocessedQueryExecutionIdTypeDef](./type_defs.md#unprocessedqueryexecutionidtypedef)
- [CalculationConfigurationTypeDef](./type_defs.md#calculationconfigurationtypedef)
- [CalculationResultTypeDef](./type_defs.md#calculationresulttypedef)
- [CalculationStatisticsTypeDef](./type_defs.md#calculationstatisticstypedef)
- [CalculationStatusTypeDef](./type_defs.md#calculationstatustypedef)
- [CancelCapacityReservationInputRequestTypeDef](./type_defs.md#cancelcapacityreservationinputrequesttypedef)
- [CapacityAllocationTypeDef](./type_defs.md#capacityallocationtypedef)
- [CapacityAssignmentTypeDef](./type_defs.md#capacityassignmenttypedef)
- [ColumnInfoTypeDef](./type_defs.md#columninfotypedef)
- [ColumnTypeDef](./type_defs.md#columntypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CreateNamedQueryInputRequestTypeDef](./type_defs.md#createnamedqueryinputrequesttypedef)
- [CreateNotebookInputRequestTypeDef](./type_defs.md#createnotebookinputrequesttypedef)
- [CreatePreparedStatementInputRequestTypeDef](./type_defs.md#createpreparedstatementinputrequesttypedef)
- [CreatePresignedNotebookUrlRequestRequestTypeDef](./type_defs.md#createpresignednotebookurlrequestrequesttypedef)
- [CustomerContentEncryptionConfigurationTypeDef](./type_defs.md#customercontentencryptionconfigurationtypedef)
- [DataCatalogSummaryTypeDef](./type_defs.md#datacatalogsummarytypedef)
- [DataCatalogTypeDef](./type_defs.md#datacatalogtypedef)
- [DatabaseTypeDef](./type_defs.md#databasetypedef)
- [DatumTypeDef](./type_defs.md#datumtypedef)
- [DeleteCapacityReservationInputRequestTypeDef](./type_defs.md#deletecapacityreservationinputrequesttypedef)
- [DeleteDataCatalogInputRequestTypeDef](./type_defs.md#deletedatacataloginputrequesttypedef)
- [DeleteNamedQueryInputRequestTypeDef](./type_defs.md#deletenamedqueryinputrequesttypedef)
- [DeleteNotebookInputRequestTypeDef](./type_defs.md#deletenotebookinputrequesttypedef)
- [DeletePreparedStatementInputRequestTypeDef](./type_defs.md#deletepreparedstatementinputrequesttypedef)
- [DeleteWorkGroupInputRequestTypeDef](./type_defs.md#deleteworkgroupinputrequesttypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [EngineConfigurationTypeDef](./type_defs.md#engineconfigurationtypedef)
- [EngineVersionTypeDef](./type_defs.md#engineversiontypedef)
- [ExecutorsSummaryTypeDef](./type_defs.md#executorssummarytypedef)
- [ExportNotebookInputRequestTypeDef](./type_defs.md#exportnotebookinputrequesttypedef)
- [NotebookMetadataTypeDef](./type_defs.md#notebookmetadatatypedef)
- [FilterDefinitionTypeDef](./type_defs.md#filterdefinitiontypedef)
- [GetCalculationExecutionCodeRequestRequestTypeDef](./type_defs.md#getcalculationexecutioncoderequestrequesttypedef)
- [GetCalculationExecutionRequestRequestTypeDef](./type_defs.md#getcalculationexecutionrequestrequesttypedef)
- [GetCalculationExecutionStatusRequestRequestTypeDef](./type_defs.md#getcalculationexecutionstatusrequestrequesttypedef)
- [GetCapacityAssignmentConfigurationInputRequestTypeDef](./type_defs.md#getcapacityassignmentconfigurationinputrequesttypedef)
- [GetCapacityReservationInputRequestTypeDef](./type_defs.md#getcapacityreservationinputrequesttypedef)
- [GetDataCatalogInputRequestTypeDef](./type_defs.md#getdatacataloginputrequesttypedef)
- [GetDatabaseInputRequestTypeDef](./type_defs.md#getdatabaseinputrequesttypedef)
- [GetNamedQueryInputRequestTypeDef](./type_defs.md#getnamedqueryinputrequesttypedef)
- [GetNotebookMetadataInputRequestTypeDef](./type_defs.md#getnotebookmetadatainputrequesttypedef)
- [GetPreparedStatementInputRequestTypeDef](./type_defs.md#getpreparedstatementinputrequesttypedef)
- [GetQueryExecutionInputRequestTypeDef](./type_defs.md#getqueryexecutioninputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetQueryResultsInputRequestTypeDef](./type_defs.md#getqueryresultsinputrequesttypedef)
- [GetQueryRuntimeStatisticsInputRequestTypeDef](./type_defs.md#getqueryruntimestatisticsinputrequesttypedef)
- [GetSessionRequestRequestTypeDef](./type_defs.md#getsessionrequestrequesttypedef)
- [SessionStatisticsTypeDef](./type_defs.md#sessionstatisticstypedef)
- [SessionStatusTypeDef](./type_defs.md#sessionstatustypedef)
- [GetSessionStatusRequestRequestTypeDef](./type_defs.md#getsessionstatusrequestrequesttypedef)
- [GetTableMetadataInputRequestTypeDef](./type_defs.md#gettablemetadatainputrequesttypedef)
- [GetWorkGroupInputRequestTypeDef](./type_defs.md#getworkgroupinputrequesttypedef)
- [ImportNotebookInputRequestTypeDef](./type_defs.md#importnotebookinputrequesttypedef)
- [ListApplicationDPUSizesInputRequestTypeDef](./type_defs.md#listapplicationdpusizesinputrequesttypedef)
- [ListCalculationExecutionsRequestRequestTypeDef](./type_defs.md#listcalculationexecutionsrequestrequesttypedef)
- [ListCapacityReservationsInputRequestTypeDef](./type_defs.md#listcapacityreservationsinputrequesttypedef)
- [ListDataCatalogsInputRequestTypeDef](./type_defs.md#listdatacatalogsinputrequesttypedef)
- [ListDatabasesInputRequestTypeDef](./type_defs.md#listdatabasesinputrequesttypedef)
- [ListEngineVersionsInputRequestTypeDef](./type_defs.md#listengineversionsinputrequesttypedef)
- [ListExecutorsRequestRequestTypeDef](./type_defs.md#listexecutorsrequestrequesttypedef)
- [ListNamedQueriesInputRequestTypeDef](./type_defs.md#listnamedqueriesinputrequesttypedef)
- [ListNotebookSessionsRequestRequestTypeDef](./type_defs.md#listnotebooksessionsrequestrequesttypedef)
- [NotebookSessionSummaryTypeDef](./type_defs.md#notebooksessionsummarytypedef)
- [ListPreparedStatementsInputRequestTypeDef](./type_defs.md#listpreparedstatementsinputrequesttypedef)
- [PreparedStatementSummaryTypeDef](./type_defs.md#preparedstatementsummarytypedef)
- [ListQueryExecutionsInputRequestTypeDef](./type_defs.md#listqueryexecutionsinputrequesttypedef)
- [ListSessionsRequestRequestTypeDef](./type_defs.md#listsessionsrequestrequesttypedef)
- [ListTableMetadataInputRequestTypeDef](./type_defs.md#listtablemetadatainputrequesttypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ListWorkGroupsInputRequestTypeDef](./type_defs.md#listworkgroupsinputrequesttypedef)
- [QueryExecutionContextTypeDef](./type_defs.md#queryexecutioncontexttypedef)
- [ResultReuseInformationTypeDef](./type_defs.md#resultreuseinformationtypedef)
- [QueryRuntimeStatisticsRowsTypeDef](./type_defs.md#queryruntimestatisticsrowstypedef)
- [QueryRuntimeStatisticsTimelineTypeDef](./type_defs.md#queryruntimestatisticstimelinetypedef)
- [QueryStagePlanNodeTypeDef](./type_defs.md#querystageplannodetypedef)
- [QueryStageTypeDef](./type_defs.md#querystagetypedef)
- [ResultReuseByAgeConfigurationTypeDef](./type_defs.md#resultreusebyageconfigurationtypedef)
- [StopCalculationExecutionRequestRequestTypeDef](./type_defs.md#stopcalculationexecutionrequestrequesttypedef)
- [StopQueryExecutionInputRequestTypeDef](./type_defs.md#stopqueryexecutioninputrequesttypedef)
- [TerminateSessionRequestRequestTypeDef](./type_defs.md#terminatesessionrequestrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateCapacityReservationInputRequestTypeDef](./type_defs.md#updatecapacityreservationinputrequesttypedef)
- [UpdateDataCatalogInputRequestTypeDef](./type_defs.md#updatedatacataloginputrequesttypedef)
- [UpdateNamedQueryInputRequestTypeDef](./type_defs.md#updatenamedqueryinputrequesttypedef)
- [UpdateNotebookInputRequestTypeDef](./type_defs.md#updatenotebookinputrequesttypedef)
- [UpdateNotebookMetadataInputRequestTypeDef](./type_defs.md#updatenotebookmetadatainputrequesttypedef)
- [UpdatePreparedStatementInputRequestTypeDef](./type_defs.md#updatepreparedstatementinputrequesttypedef)
- [QueryExecutionStatusTypeDef](./type_defs.md#queryexecutionstatustypedef)
- [CreateNamedQueryOutputTypeDef](./type_defs.md#createnamedqueryoutputtypedef)
- [CreateNotebookOutputTypeDef](./type_defs.md#createnotebookoutputtypedef)
- [CreatePresignedNotebookUrlResponseTypeDef](./type_defs.md#createpresignednotebookurlresponsetypedef)
- [GetCalculationExecutionCodeResponseTypeDef](./type_defs.md#getcalculationexecutioncoderesponsetypedef)
- [GetNamedQueryOutputTypeDef](./type_defs.md#getnamedqueryoutputtypedef)
- [ImportNotebookOutputTypeDef](./type_defs.md#importnotebookoutputtypedef)
- [ListApplicationDPUSizesOutputTypeDef](./type_defs.md#listapplicationdpusizesoutputtypedef)
- [ListNamedQueriesOutputTypeDef](./type_defs.md#listnamedqueriesoutputtypedef)
- [ListQueryExecutionsOutputTypeDef](./type_defs.md#listqueryexecutionsoutputtypedef)
- [StartCalculationExecutionResponseTypeDef](./type_defs.md#startcalculationexecutionresponsetypedef)
- [StartQueryExecutionOutputTypeDef](./type_defs.md#startqueryexecutionoutputtypedef)
- [StartSessionResponseTypeDef](./type_defs.md#startsessionresponsetypedef)
- [StopCalculationExecutionResponseTypeDef](./type_defs.md#stopcalculationexecutionresponsetypedef)
- [TerminateSessionResponseTypeDef](./type_defs.md#terminatesessionresponsetypedef)
- [BatchGetNamedQueryOutputTypeDef](./type_defs.md#batchgetnamedqueryoutputtypedef)
- [GetPreparedStatementOutputTypeDef](./type_defs.md#getpreparedstatementoutputtypedef)
- [BatchGetPreparedStatementOutputTypeDef](./type_defs.md#batchgetpreparedstatementoutputtypedef)
- [StartCalculationExecutionRequestRequestTypeDef](./type_defs.md#startcalculationexecutionrequestrequesttypedef)
- [CalculationSummaryTypeDef](./type_defs.md#calculationsummarytypedef)
- [GetCalculationExecutionResponseTypeDef](./type_defs.md#getcalculationexecutionresponsetypedef)
- [GetCalculationExecutionStatusResponseTypeDef](./type_defs.md#getcalculationexecutionstatusresponsetypedef)
- [CapacityReservationTypeDef](./type_defs.md#capacityreservationtypedef)
- [CapacityAssignmentConfigurationTypeDef](./type_defs.md#capacityassignmentconfigurationtypedef)
- [PutCapacityAssignmentConfigurationInputRequestTypeDef](./type_defs.md#putcapacityassignmentconfigurationinputrequesttypedef)
- [ResultSetMetadataTypeDef](./type_defs.md#resultsetmetadatatypedef)
- [TableMetadataTypeDef](./type_defs.md#tablemetadatatypedef)
- [CreateCapacityReservationInputRequestTypeDef](./type_defs.md#createcapacityreservationinputrequesttypedef)
- [CreateDataCatalogInputRequestTypeDef](./type_defs.md#createdatacataloginputrequesttypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [ListDataCatalogsOutputTypeDef](./type_defs.md#listdatacatalogsoutputtypedef)
- [GetDataCatalogOutputTypeDef](./type_defs.md#getdatacatalogoutputtypedef)
- [GetDatabaseOutputTypeDef](./type_defs.md#getdatabaseoutputtypedef)
- [ListDatabasesOutputTypeDef](./type_defs.md#listdatabasesoutputtypedef)
- [RowTypeDef](./type_defs.md#rowtypedef)
- [ResultConfigurationTypeDef](./type_defs.md#resultconfigurationtypedef)
- [ResultConfigurationUpdatesTypeDef](./type_defs.md#resultconfigurationupdatestypedef)
- [SessionConfigurationTypeDef](./type_defs.md#sessionconfigurationtypedef)
- [StartSessionRequestRequestTypeDef](./type_defs.md#startsessionrequestrequesttypedef)
- [ListEngineVersionsOutputTypeDef](./type_defs.md#listengineversionsoutputtypedef)
- [WorkGroupSummaryTypeDef](./type_defs.md#workgroupsummarytypedef)
- [ListExecutorsResponseTypeDef](./type_defs.md#listexecutorsresponsetypedef)
- [ExportNotebookOutputTypeDef](./type_defs.md#exportnotebookoutputtypedef)
- [GetNotebookMetadataOutputTypeDef](./type_defs.md#getnotebookmetadataoutputtypedef)
- [ListNotebookMetadataOutputTypeDef](./type_defs.md#listnotebookmetadataoutputtypedef)
- [ListNotebookMetadataInputRequestTypeDef](./type_defs.md#listnotebookmetadatainputrequesttypedef)
- [GetQueryResultsInputGetQueryResultsPaginateTypeDef](./type_defs.md#getqueryresultsinputgetqueryresultspaginatetypedef)
- [ListDataCatalogsInputListDataCatalogsPaginateTypeDef](./type_defs.md#listdatacatalogsinputlistdatacatalogspaginatetypedef)
- [ListDatabasesInputListDatabasesPaginateTypeDef](./type_defs.md#listdatabasesinputlistdatabasespaginatetypedef)
- [ListNamedQueriesInputListNamedQueriesPaginateTypeDef](./type_defs.md#listnamedqueriesinputlistnamedqueriespaginatetypedef)
- [ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef](./type_defs.md#listqueryexecutionsinputlistqueryexecutionspaginatetypedef)
- [ListTableMetadataInputListTableMetadataPaginateTypeDef](./type_defs.md#listtablemetadatainputlisttablemetadatapaginatetypedef)
- [ListTagsForResourceInputListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourceinputlisttagsforresourcepaginatetypedef)
- [GetSessionStatusResponseTypeDef](./type_defs.md#getsessionstatusresponsetypedef)
- [SessionSummaryTypeDef](./type_defs.md#sessionsummarytypedef)
- [ListNotebookSessionsResponseTypeDef](./type_defs.md#listnotebooksessionsresponsetypedef)
- [ListPreparedStatementsOutputTypeDef](./type_defs.md#listpreparedstatementsoutputtypedef)
- [QueryExecutionStatisticsTypeDef](./type_defs.md#queryexecutionstatisticstypedef)
- [QueryRuntimeStatisticsTypeDef](./type_defs.md#queryruntimestatisticstypedef)
- [ResultReuseConfigurationTypeDef](./type_defs.md#resultreuseconfigurationtypedef)
- [ListCalculationExecutionsResponseTypeDef](./type_defs.md#listcalculationexecutionsresponsetypedef)
- [GetCapacityReservationOutputTypeDef](./type_defs.md#getcapacityreservationoutputtypedef)
- [ListCapacityReservationsOutputTypeDef](./type_defs.md#listcapacityreservationsoutputtypedef)
- [GetCapacityAssignmentConfigurationOutputTypeDef](./type_defs.md#getcapacityassignmentconfigurationoutputtypedef)
- [GetTableMetadataOutputTypeDef](./type_defs.md#gettablemetadataoutputtypedef)
- [ListTableMetadataOutputTypeDef](./type_defs.md#listtablemetadataoutputtypedef)
- [ResultSetTypeDef](./type_defs.md#resultsettypedef)
- [WorkGroupConfigurationTypeDef](./type_defs.md#workgroupconfigurationtypedef)
- [WorkGroupConfigurationUpdatesTypeDef](./type_defs.md#workgroupconfigurationupdatestypedef)
- [GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef)
- [ListWorkGroupsOutputTypeDef](./type_defs.md#listworkgroupsoutputtypedef)
- [ListSessionsResponseTypeDef](./type_defs.md#listsessionsresponsetypedef)
- [GetQueryRuntimeStatisticsOutputTypeDef](./type_defs.md#getqueryruntimestatisticsoutputtypedef)
- [QueryExecutionTypeDef](./type_defs.md#queryexecutiontypedef)
- [StartQueryExecutionInputRequestTypeDef](./type_defs.md#startqueryexecutioninputrequesttypedef)
- [GetQueryResultsOutputTypeDef](./type_defs.md#getqueryresultsoutputtypedef)
- [CreateWorkGroupInputRequestTypeDef](./type_defs.md#createworkgroupinputrequesttypedef)
- [WorkGroupTypeDef](./type_defs.md#workgrouptypedef)
- [UpdateWorkGroupInputRequestTypeDef](./type_defs.md#updateworkgroupinputrequesttypedef)
- [BatchGetQueryExecutionOutputTypeDef](./type_defs.md#batchgetqueryexecutionoutputtypedef)
- [GetQueryExecutionOutputTypeDef](./type_defs.md#getqueryexecutionoutputtypedef)
- [GetWorkGroupOutputTypeDef](./type_defs.md#getworkgroupoutputtypedef)

