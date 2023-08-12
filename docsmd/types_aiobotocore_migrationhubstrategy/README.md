# MigrationHubStrategyRecommendations module

> [Index](../README.md) > MigrationHubStrategyRecommendations


!!! note ""

    Auto-generated documentation for [MigrationHubStrategyRecommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
    type annotations stubs module [types-aiobotocore-migrationhubstrategy](https://pypi.org/project/types-aiobotocore-migrationhubstrategy/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `MigrationHubStrategyRecommendations` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[migrationhubstrategy]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[migrationhubstrategy]'


# standalone installation
python -m pip install types-aiobotocore-migrationhubstrategy
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-migrationhubstrategy
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MigrationHubStrategyRecommendationsClient

Type annotations and code completion for  `#!python session.create_client("migrationhubstrategy")` as [MigrationHubStrategyRecommendationsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# MigrationHubStrategyRecommendationsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.client import MigrationHubStrategyRecommendationsClient


session = get_session()
async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("migrationhubstrategy").get_paginator("...")`.

```python
# GetServerDetailsPaginator usage example

from types_aiobotocore_migrationhubstrategy.paginator import GetServerDetailsPaginator

def get_get_server_details_paginator() -> GetServerDetailsPaginator:
    return client.get_paginator("get_server_details"))
```

- [GetServerDetailsPaginator](./paginators.md#getserverdetailspaginator)
- [ListApplicationComponentsPaginator](./paginators.md#listapplicationcomponentspaginator)
- [ListCollectorsPaginator](./paginators.md#listcollectorspaginator)
- [ListImportFileTaskPaginator](./paginators.md#listimportfiletaskpaginator)
- [ListServersPaginator](./paginators.md#listserverspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AnalysisTypeType usage example

from types_aiobotocore_migrationhubstrategy.literals import AnalysisTypeType

def get_value() -> AnalysisTypeType:
    return "BINARY_ANALYSIS"
```

- [AnalysisTypeType](./literals.md#analysistypetype)
- [AntipatternReportStatusType](./literals.md#antipatternreportstatustype)
- [AppTypeType](./literals.md#apptypetype)
- [AppUnitErrorCategoryType](./literals.md#appuniterrorcategorytype)
- [ApplicationComponentCriteriaType](./literals.md#applicationcomponentcriteriatype)
- [ApplicationModeType](./literals.md#applicationmodetype)
- [AssessmentStatusType](./literals.md#assessmentstatustype)
- [AuthTypeType](./literals.md#authtypetype)
- [AwsManagedTargetDestinationType](./literals.md#awsmanagedtargetdestinationtype)
- [BinaryAnalyzerNameType](./literals.md#binaryanalyzernametype)
- [CollectorHealthType](./literals.md#collectorhealthtype)
- [ConditionType](./literals.md#conditiontype)
- [DataSourceTypeType](./literals.md#datasourcetypetype)
- [DatabaseManagementPreferenceType](./literals.md#databasemanagementpreferencetype)
- [GetServerDetailsPaginatorName](./literals.md#getserverdetailspaginatorname)
- [GroupNameType](./literals.md#groupnametype)
- [HeterogeneousTargetDatabaseEngineType](./literals.md#heterogeneoustargetdatabaseenginetype)
- [HomogeneousTargetDatabaseEngineType](./literals.md#homogeneoustargetdatabaseenginetype)
- [ImportFileTaskStatusType](./literals.md#importfiletaskstatustype)
- [InclusionStatusType](./literals.md#inclusionstatustype)
- [ListApplicationComponentsPaginatorName](./literals.md#listapplicationcomponentspaginatorname)
- [ListCollectorsPaginatorName](./literals.md#listcollectorspaginatorname)
- [ListImportFileTaskPaginatorName](./literals.md#listimportfiletaskpaginatorname)
- [ListServersPaginatorName](./literals.md#listserverspaginatorname)
- [NoPreferenceTargetDestinationType](./literals.md#nopreferencetargetdestinationtype)
- [OSTypeType](./literals.md#ostypetype)
- [OutputFormatType](./literals.md#outputformattype)
- [PipelineTypeType](./literals.md#pipelinetypetype)
- [RecommendationReportStatusType](./literals.md#recommendationreportstatustype)
- [ResourceSubTypeType](./literals.md#resourcesubtypetype)
- [RunTimeAnalyzerNameType](./literals.md#runtimeanalyzernametype)
- [RunTimeAssessmentStatusType](./literals.md#runtimeassessmentstatustype)
- [RuntimeAnalysisStatusType](./literals.md#runtimeanalysisstatustype)
- [SelfManageTargetDestinationType](./literals.md#selfmanagetargetdestinationtype)
- [ServerCriteriaType](./literals.md#servercriteriatype)
- [ServerErrorCategoryType](./literals.md#servererrorcategorytype)
- [ServerOsTypeType](./literals.md#serverostypetype)
- [SeverityType](./literals.md#severitytype)
- [SortOrderType](./literals.md#sortordertype)
- [SourceCodeAnalyzerNameType](./literals.md#sourcecodeanalyzernametype)
- [SrcCodeOrDbAnalysisStatusType](./literals.md#srccodeordbanalysisstatustype)
- [StrategyRecommendationType](./literals.md#strategyrecommendationtype)
- [StrategyType](./literals.md#strategytype)
- [TargetDatabaseEngineType](./literals.md#targetdatabaseenginetype)
- [TargetDestinationType](./literals.md#targetdestinationtype)
- [TransformationToolNameType](./literals.md#transformationtoolnametype)
- [VersionControlType](./literals.md#versioncontroltype)
- [VersionControlTypeType](./literals.md#versioncontroltypetype)
- [MigrationHubStrategyRecommendationsServiceName](./literals.md#migrationhubstrategyrecommendationsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AnalysisStatusUnionTypeDef](./type_defs.md#analysisstatusuniontypedef)
- [AnalyzerNameUnionTypeDef](./type_defs.md#analyzernameuniontypedef)
- [S3ObjectTypeDef](./type_defs.md#s3objecttypedef)
- [AntipatternSeveritySummaryTypeDef](./type_defs.md#antipatternseveritysummarytypedef)
- [AppUnitErrorTypeDef](./type_defs.md#appuniterrortypedef)
- [DatabaseConfigDetailTypeDef](./type_defs.md#databaseconfigdetailtypedef)
- [SourceCodeRepositoryTypeDef](./type_defs.md#sourcecoderepositorytypedef)
- [ApplicationComponentStatusSummaryTypeDef](./type_defs.md#applicationcomponentstatussummarytypedef)
- [ApplicationComponentSummaryTypeDef](./type_defs.md#applicationcomponentsummarytypedef)
- [ServerStatusSummaryTypeDef](./type_defs.md#serverstatussummarytypedef)
- [ServerSummaryTypeDef](./type_defs.md#serversummarytypedef)
- [StrategySummaryTypeDef](./type_defs.md#strategysummarytypedef)
- [AssessmentTargetTypeDef](./type_defs.md#assessmenttargettypedef)
- [AssociatedApplicationTypeDef](./type_defs.md#associatedapplicationtypedef)
- [AwsManagedResourcesTypeDef](./type_defs.md#awsmanagedresourcestypedef)
- [BusinessGoalsTypeDef](./type_defs.md#businessgoalstypedef)
- [IPAddressBasedRemoteInfoTypeDef](./type_defs.md#ipaddressbasedremoteinfotypedef)
- [PipelineInfoTypeDef](./type_defs.md#pipelineinfotypedef)
- [RemoteSourceCodeAnalysisServerInfoTypeDef](./type_defs.md#remotesourcecodeanalysisserverinfotypedef)
- [VcenterBasedRemoteInfoTypeDef](./type_defs.md#vcenterbasedremoteinfotypedef)
- [VersionControlInfoTypeDef](./type_defs.md#versioncontrolinfotypedef)
- [DataCollectionDetailsTypeDef](./type_defs.md#datacollectiondetailstypedef)
- [HeterogeneousTypeDef](./type_defs.md#heterogeneoustypedef)
- [HomogeneousTypeDef](./type_defs.md#homogeneoustypedef)
- [NoDatabaseMigrationPreferenceTypeDef](./type_defs.md#nodatabasemigrationpreferencetypedef)
- [GetApplicationComponentDetailsRequestRequestTypeDef](./type_defs.md#getapplicationcomponentdetailsrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetApplicationComponentStrategiesRequestRequestTypeDef](./type_defs.md#getapplicationcomponentstrategiesrequestrequesttypedef)
- [GetAssessmentRequestRequestTypeDef](./type_defs.md#getassessmentrequestrequesttypedef)
- [GetImportFileTaskRequestRequestTypeDef](./type_defs.md#getimportfiletaskrequestrequesttypedef)
- [GetRecommendationReportDetailsRequestRequestTypeDef](./type_defs.md#getrecommendationreportdetailsrequestrequesttypedef)
- [RecommendationReportDetailsTypeDef](./type_defs.md#recommendationreportdetailstypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetServerDetailsRequestRequestTypeDef](./type_defs.md#getserverdetailsrequestrequesttypedef)
- [GetServerStrategiesRequestRequestTypeDef](./type_defs.md#getserverstrategiesrequestrequesttypedef)
- [GroupTypeDef](./type_defs.md#grouptypedef)
- [ImportFileTaskInformationTypeDef](./type_defs.md#importfiletaskinformationtypedef)
- [ListCollectorsRequestRequestTypeDef](./type_defs.md#listcollectorsrequestrequesttypedef)
- [ListImportFileTaskRequestRequestTypeDef](./type_defs.md#listimportfiletaskrequestrequesttypedef)
- [NoManagementPreferenceTypeDef](./type_defs.md#nomanagementpreferencetypedef)
- [SelfManageResourcesTypeDef](./type_defs.md#selfmanageresourcestypedef)
- [NetworkInfoTypeDef](./type_defs.md#networkinfotypedef)
- [OSInfoTypeDef](./type_defs.md#osinfotypedef)
- [TransformationToolTypeDef](./type_defs.md#transformationtooltypedef)
- [ServerErrorTypeDef](./type_defs.md#servererrortypedef)
- [SourceCodeTypeDef](./type_defs.md#sourcecodetypedef)
- [StopAssessmentRequestRequestTypeDef](./type_defs.md#stopassessmentrequestrequesttypedef)
- [StrategyOptionTypeDef](./type_defs.md#strategyoptiontypedef)
- [AntipatternReportResultTypeDef](./type_defs.md#antipatternreportresulttypedef)
- [AssessmentSummaryTypeDef](./type_defs.md#assessmentsummarytypedef)
- [StartAssessmentRequestRequestTypeDef](./type_defs.md#startassessmentrequestrequesttypedef)
- [PrioritizeBusinessGoalsTypeDef](./type_defs.md#prioritizebusinessgoalstypedef)
- [ConfigurationSummaryTypeDef](./type_defs.md#configurationsummarytypedef)
- [DatabaseMigrationPreferenceTypeDef](./type_defs.md#databasemigrationpreferencetypedef)
- [GetAssessmentResponseTypeDef](./type_defs.md#getassessmentresponsetypedef)
- [GetImportFileTaskResponseTypeDef](./type_defs.md#getimportfiletaskresponsetypedef)
- [GetLatestAssessmentIdResponseTypeDef](./type_defs.md#getlatestassessmentidresponsetypedef)
- [StartAssessmentResponseTypeDef](./type_defs.md#startassessmentresponsetypedef)
- [StartImportFileTaskResponseTypeDef](./type_defs.md#startimportfiletaskresponsetypedef)
- [StartRecommendationReportGenerationResponseTypeDef](./type_defs.md#startrecommendationreportgenerationresponsetypedef)
- [GetRecommendationReportDetailsResponseTypeDef](./type_defs.md#getrecommendationreportdetailsresponsetypedef)
- [GetServerDetailsRequestGetServerDetailsPaginateTypeDef](./type_defs.md#getserverdetailsrequestgetserverdetailspaginatetypedef)
- [ListCollectorsRequestListCollectorsPaginateTypeDef](./type_defs.md#listcollectorsrequestlistcollectorspaginatetypedef)
- [ListImportFileTaskRequestListImportFileTaskPaginateTypeDef](./type_defs.md#listimportfiletaskrequestlistimportfiletaskpaginatetypedef)
- [ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef](./type_defs.md#listapplicationcomponentsrequestlistapplicationcomponentspaginatetypedef)
- [ListApplicationComponentsRequestRequestTypeDef](./type_defs.md#listapplicationcomponentsrequestrequesttypedef)
- [ListServersRequestListServersPaginateTypeDef](./type_defs.md#listserversrequestlistserverspaginatetypedef)
- [ListServersRequestRequestTypeDef](./type_defs.md#listserversrequestrequesttypedef)
- [StartImportFileTaskRequestRequestTypeDef](./type_defs.md#startimportfiletaskrequestrequesttypedef)
- [StartRecommendationReportGenerationRequestRequestTypeDef](./type_defs.md#startrecommendationreportgenerationrequestrequesttypedef)
- [ListImportFileTaskResponseTypeDef](./type_defs.md#listimportfiletaskresponsetypedef)
- [ManagementPreferenceTypeDef](./type_defs.md#managementpreferencetypedef)
- [SystemInfoTypeDef](./type_defs.md#systeminfotypedef)
- [RecommendationSetTypeDef](./type_defs.md#recommendationsettypedef)
- [UpdateApplicationComponentConfigRequestRequestTypeDef](./type_defs.md#updateapplicationcomponentconfigrequestrequesttypedef)
- [UpdateServerConfigRequestRequestTypeDef](./type_defs.md#updateserverconfigrequestrequesttypedef)
- [ResultTypeDef](./type_defs.md#resulttypedef)
- [GetPortfolioSummaryResponseTypeDef](./type_defs.md#getportfoliosummaryresponsetypedef)
- [CollectorTypeDef](./type_defs.md#collectortypedef)
- [DatabasePreferencesTypeDef](./type_defs.md#databasepreferencestypedef)
- [ApplicationPreferencesTypeDef](./type_defs.md#applicationpreferencestypedef)
- [ApplicationComponentStrategyTypeDef](./type_defs.md#applicationcomponentstrategytypedef)
- [ServerDetailTypeDef](./type_defs.md#serverdetailtypedef)
- [ServerStrategyTypeDef](./type_defs.md#serverstrategytypedef)
- [ApplicationComponentDetailTypeDef](./type_defs.md#applicationcomponentdetailtypedef)
- [ListCollectorsResponseTypeDef](./type_defs.md#listcollectorsresponsetypedef)
- [GetPortfolioPreferencesResponseTypeDef](./type_defs.md#getportfoliopreferencesresponsetypedef)
- [PutPortfolioPreferencesRequestRequestTypeDef](./type_defs.md#putportfoliopreferencesrequestrequesttypedef)
- [GetApplicationComponentStrategiesResponseTypeDef](./type_defs.md#getapplicationcomponentstrategiesresponsetypedef)
- [GetServerDetailsResponseTypeDef](./type_defs.md#getserverdetailsresponsetypedef)
- [ListServersResponseTypeDef](./type_defs.md#listserversresponsetypedef)
- [GetServerStrategiesResponseTypeDef](./type_defs.md#getserverstrategiesresponsetypedef)
- [GetApplicationComponentDetailsResponseTypeDef](./type_defs.md#getapplicationcomponentdetailsresponsetypedef)
- [ListApplicationComponentsResponseTypeDef](./type_defs.md#listapplicationcomponentsresponsetypedef)

