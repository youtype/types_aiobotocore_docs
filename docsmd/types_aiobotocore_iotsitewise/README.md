# IoTSiteWise module

> [Index](../README.md) > IoTSiteWise


!!! note ""

    Auto-generated documentation for [IoTSiteWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#iotsitewise)
    type annotations stubs module [types-aiobotocore-iotsitewise](https://pypi.org/project/types-aiobotocore-iotsitewise/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `IoTSiteWise` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `IoTSiteWise` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iotsitewise]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iotsitewise]'

# standalone installation
python -m pip install types-aiobotocore-iotsitewise
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iotsitewise
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTSiteWiseClient

Type annotations and code completion for  `#!python session.create_client("iotsitewise")` as [IoTSiteWiseClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client)

```python
# IoTSiteWiseClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.client import IoTSiteWiseClient


session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("iotsitewise").get_paginator("...")`.

```python
# ExecuteQueryPaginator usage example

from types_aiobotocore_iotsitewise.paginator import ExecuteQueryPaginator

def get_execute_query_paginator() -> ExecuteQueryPaginator:
    return client.get_paginator("execute_query"))
```

- [ExecuteQueryPaginator](./paginators.md#executequerypaginator)
- [GetAssetPropertyAggregatesPaginator](./paginators.md#getassetpropertyaggregatespaginator)
- [GetAssetPropertyValueHistoryPaginator](./paginators.md#getassetpropertyvaluehistorypaginator)
- [GetInterpolatedAssetPropertyValuesPaginator](./paginators.md#getinterpolatedassetpropertyvaluespaginator)
- [ListAccessPoliciesPaginator](./paginators.md#listaccesspoliciespaginator)
- [ListActionsPaginator](./paginators.md#listactionspaginator)
- [ListAssetModelCompositeModelsPaginator](./paginators.md#listassetmodelcompositemodelspaginator)
- [ListAssetModelPropertiesPaginator](./paginators.md#listassetmodelpropertiespaginator)
- [ListAssetModelsPaginator](./paginators.md#listassetmodelspaginator)
- [ListAssetPropertiesPaginator](./paginators.md#listassetpropertiespaginator)
- [ListAssetRelationshipsPaginator](./paginators.md#listassetrelationshipspaginator)
- [ListAssetsPaginator](./paginators.md#listassetspaginator)
- [ListAssociatedAssetsPaginator](./paginators.md#listassociatedassetspaginator)
- [ListBulkImportJobsPaginator](./paginators.md#listbulkimportjobspaginator)
- [ListCompositionRelationshipsPaginator](./paginators.md#listcompositionrelationshipspaginator)
- [ListDashboardsPaginator](./paginators.md#listdashboardspaginator)
- [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
- [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
- [ListPortalsPaginator](./paginators.md#listportalspaginator)
- [ListProjectAssetsPaginator](./paginators.md#listprojectassetspaginator)
- [ListProjectsPaginator](./paginators.md#listprojectspaginator)
- [ListTimeSeriesPaginator](./paginators.md#listtimeseriespaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("iotsitewise").get_waiter("...")`.

```python
# AssetActiveWaiter usage example

from types_aiobotocore_iotsitewise.waiter import AssetActiveWaiter

def get_asset_active_waiter() -> AssetActiveWaiter:
    return Session().client("iotsitewise").get_waiter("asset_active")
```

- [AssetActiveWaiter](./waiters.md#assetactivewaiter)
- [AssetModelActiveWaiter](./waiters.md#assetmodelactivewaiter)
- [AssetModelNotExistsWaiter](./waiters.md#assetmodelnotexistswaiter)
- [AssetNotExistsWaiter](./waiters.md#assetnotexistswaiter)
- [PortalActiveWaiter](./waiters.md#portalactivewaiter)
- [PortalNotExistsWaiter](./waiters.md#portalnotexistswaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AggregateTypeType usage example

from types_aiobotocore_iotsitewise.literals import AggregateTypeType

def get_value() -> AggregateTypeType:
    return "AVERAGE"
```

- [AggregateTypeType](./literals.md#aggregatetypetype)
- [AssetActiveWaiterName](./literals.md#assetactivewaitername)
- [AssetErrorCodeType](./literals.md#asseterrorcodetype)
- [AssetModelActiveWaiterName](./literals.md#assetmodelactivewaitername)
- [AssetModelNotExistsWaiterName](./literals.md#assetmodelnotexistswaitername)
- [AssetModelStateType](./literals.md#assetmodelstatetype)
- [AssetModelTypeType](./literals.md#assetmodeltypetype)
- [AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype)
- [AssetNotExistsWaiterName](./literals.md#assetnotexistswaitername)
- [AssetRelationshipTypeType](./literals.md#assetrelationshiptypetype)
- [AssetStateType](./literals.md#assetstatetype)
- [AuthModeType](./literals.md#authmodetype)
- [BatchEntryCompletionStatusType](./literals.md#batchentrycompletionstatustype)
- [BatchGetAssetPropertyAggregatesErrorCodeType](./literals.md#batchgetassetpropertyaggregateserrorcodetype)
- [BatchGetAssetPropertyValueErrorCodeType](./literals.md#batchgetassetpropertyvalueerrorcodetype)
- [BatchGetAssetPropertyValueHistoryErrorCodeType](./literals.md#batchgetassetpropertyvaluehistoryerrorcodetype)
- [BatchPutAssetPropertyValueErrorCodeType](./literals.md#batchputassetpropertyvalueerrorcodetype)
- [CapabilitySyncStatusType](./literals.md#capabilitysyncstatustype)
- [ColumnNameType](./literals.md#columnnametype)
- [ComputeLocationType](./literals.md#computelocationtype)
- [ConfigurationStateType](./literals.md#configurationstatetype)
- [DatasetSourceFormatType](./literals.md#datasetsourceformattype)
- [DatasetSourceTypeType](./literals.md#datasetsourcetypetype)
- [DatasetStateType](./literals.md#datasetstatetype)
- [DetailedErrorCodeType](./literals.md#detailederrorcodetype)
- [DisassociatedDataStorageStateType](./literals.md#disassociateddatastoragestatetype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [ErrorCodeType](./literals.md#errorcodetype)
- [ExecuteQueryPaginatorName](./literals.md#executequerypaginatorname)
- [ForwardingConfigStateType](./literals.md#forwardingconfigstatetype)
- [GetAssetPropertyAggregatesPaginatorName](./literals.md#getassetpropertyaggregatespaginatorname)
- [GetAssetPropertyValueHistoryPaginatorName](./literals.md#getassetpropertyvaluehistorypaginatorname)
- [GetInterpolatedAssetPropertyValuesPaginatorName](./literals.md#getinterpolatedassetpropertyvaluespaginatorname)
- [IdentityTypeType](./literals.md#identitytypetype)
- [ImageFileTypeType](./literals.md#imagefiletypetype)
- [JobStatusType](./literals.md#jobstatustype)
- [ListAccessPoliciesPaginatorName](./literals.md#listaccesspoliciespaginatorname)
- [ListActionsPaginatorName](./literals.md#listactionspaginatorname)
- [ListAssetModelCompositeModelsPaginatorName](./literals.md#listassetmodelcompositemodelspaginatorname)
- [ListAssetModelPropertiesFilterType](./literals.md#listassetmodelpropertiesfiltertype)
- [ListAssetModelPropertiesPaginatorName](./literals.md#listassetmodelpropertiespaginatorname)
- [ListAssetModelsPaginatorName](./literals.md#listassetmodelspaginatorname)
- [ListAssetPropertiesFilterType](./literals.md#listassetpropertiesfiltertype)
- [ListAssetPropertiesPaginatorName](./literals.md#listassetpropertiespaginatorname)
- [ListAssetRelationshipsPaginatorName](./literals.md#listassetrelationshipspaginatorname)
- [ListAssetsFilterType](./literals.md#listassetsfiltertype)
- [ListAssetsPaginatorName](./literals.md#listassetspaginatorname)
- [ListAssociatedAssetsPaginatorName](./literals.md#listassociatedassetspaginatorname)
- [ListBulkImportJobsFilterType](./literals.md#listbulkimportjobsfiltertype)
- [ListBulkImportJobsPaginatorName](./literals.md#listbulkimportjobspaginatorname)
- [ListCompositionRelationshipsPaginatorName](./literals.md#listcompositionrelationshipspaginatorname)
- [ListDashboardsPaginatorName](./literals.md#listdashboardspaginatorname)
- [ListDatasetsPaginatorName](./literals.md#listdatasetspaginatorname)
- [ListGatewaysPaginatorName](./literals.md#listgatewayspaginatorname)
- [ListPortalsPaginatorName](./literals.md#listportalspaginatorname)
- [ListProjectAssetsPaginatorName](./literals.md#listprojectassetspaginatorname)
- [ListProjectsPaginatorName](./literals.md#listprojectspaginatorname)
- [ListTimeSeriesPaginatorName](./literals.md#listtimeseriespaginatorname)
- [ListTimeSeriesTypeType](./literals.md#listtimeseriestypetype)
- [LoggingLevelType](./literals.md#loggingleveltype)
- [MonitorErrorCodeType](./literals.md#monitorerrorcodetype)
- [PermissionType](./literals.md#permissiontype)
- [PortalActiveWaiterName](./literals.md#portalactivewaitername)
- [PortalNotExistsWaiterName](./literals.md#portalnotexistswaitername)
- [PortalStateType](./literals.md#portalstatetype)
- [PortalTypeType](./literals.md#portaltypetype)
- [PropertyDataTypeType](./literals.md#propertydatatypetype)
- [PropertyNotificationStateType](./literals.md#propertynotificationstatetype)
- [QualityType](./literals.md#qualitytype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [ScalarTypeType](./literals.md#scalartypetype)
- [StorageTypeType](./literals.md#storagetypetype)
- [TargetResourceTypeType](./literals.md#targetresourcetypetype)
- [TimeOrderingType](./literals.md#timeorderingtype)
- [TraversalDirectionType](./literals.md#traversaldirectiontype)
- [TraversalTypeType](./literals.md#traversaltypetype)
- [WarmTierStateType](./literals.md#warmtierstatetype)
- [IoTSiteWiseServiceName](./literals.md#iotsitewiseservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef)
- [ActionDefinitionTypeDef](./type_defs.md#actiondefinitiontypedef)
- [ActionPayloadTypeDef](./type_defs.md#actionpayloadtypedef)
- [TargetResourceTypeDef](./type_defs.md#targetresourcetypedef)
- [AggregatesTypeDef](./type_defs.md#aggregatestypedef)
- [AlarmsTypeDef](./type_defs.md#alarmstypedef)
- [AssetCompositeModelPathSegmentTypeDef](./type_defs.md#assetcompositemodelpathsegmenttypedef)
- [AssetErrorDetailsTypeDef](./type_defs.md#asseterrordetailstypedef)
- [AssetHierarchyInfoTypeDef](./type_defs.md#assethierarchyinfotypedef)
- [AssetHierarchyTypeDef](./type_defs.md#assethierarchytypedef)
- [AssetModelCompositeModelPathSegmentTypeDef](./type_defs.md#assetmodelcompositemodelpathsegmenttypedef)
- [AssetModelHierarchyDefinitionTypeDef](./type_defs.md#assetmodelhierarchydefinitiontypedef)
- [AssetModelHierarchyTypeDef](./type_defs.md#assetmodelhierarchytypedef)
- [AssetModelPropertyPathSegmentTypeDef](./type_defs.md#assetmodelpropertypathsegmenttypedef)
- [AssetPropertyPathSegmentTypeDef](./type_defs.md#assetpropertypathsegmenttypedef)
- [PropertyNotificationTypeDef](./type_defs.md#propertynotificationtypedef)
- [TimeInNanosTypeDef](./type_defs.md#timeinnanostypedef)
- [VariantTypeDef](./type_defs.md#varianttypedef)
- [AssociateAssetsRequestRequestTypeDef](./type_defs.md#associateassetsrequestrequesttypedef)
- [AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef](./type_defs.md#associatetimeseriestoassetpropertyrequestrequesttypedef)
- [AttributeTypeDef](./type_defs.md#attributetypedef)
- [BatchAssociateProjectAssetsRequestRequestTypeDef](./type_defs.md#batchassociateprojectassetsrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchDisassociateProjectAssetsRequestRequestTypeDef](./type_defs.md#batchdisassociateprojectassetsrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [BatchGetAssetPropertyAggregatesErrorEntryTypeDef](./type_defs.md#batchgetassetpropertyaggregateserrorentrytypedef)
- [BatchGetAssetPropertyAggregatesErrorInfoTypeDef](./type_defs.md#batchgetassetpropertyaggregateserrorinfotypedef)
- [BatchGetAssetPropertyValueEntryTypeDef](./type_defs.md#batchgetassetpropertyvalueentrytypedef)
- [BatchGetAssetPropertyValueErrorEntryTypeDef](./type_defs.md#batchgetassetpropertyvalueerrorentrytypedef)
- [BatchGetAssetPropertyValueErrorInfoTypeDef](./type_defs.md#batchgetassetpropertyvalueerrorinfotypedef)
- [BatchGetAssetPropertyValueHistoryErrorEntryTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryerrorentrytypedef)
- [BatchGetAssetPropertyValueHistoryErrorInfoTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryerrorinfotypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ContentTypeDef](./type_defs.md#contenttypedef)
- [ColumnTypeTypeDef](./type_defs.md#columntypetypedef)
- [CompositionRelationshipItemTypeDef](./type_defs.md#compositionrelationshipitemtypedef)
- [CompositionRelationshipSummaryTypeDef](./type_defs.md#compositionrelationshipsummarytypedef)
- [ConfigurationErrorDetailsTypeDef](./type_defs.md#configurationerrordetailstypedef)
- [ConflictingOperationExceptionTypeDef](./type_defs.md#conflictingoperationexceptiontypedef)
- [CreateAssetRequestRequestTypeDef](./type_defs.md#createassetrequestrequesttypedef)
- [ErrorReportLocationTypeDef](./type_defs.md#errorreportlocationtypedef)
- [FileTypeDef](./type_defs.md#filetypedef)
- [CreateDashboardRequestRequestTypeDef](./type_defs.md#createdashboardrequestrequesttypedef)
- [CreateProjectRequestRequestTypeDef](./type_defs.md#createprojectrequestrequesttypedef)
- [CsvOutputTypeDef](./type_defs.md#csvoutputtypedef)
- [CsvTypeDef](./type_defs.md#csvtypedef)
- [CustomerManagedS3StorageTypeDef](./type_defs.md#customermanageds3storagetypedef)
- [DashboardSummaryTypeDef](./type_defs.md#dashboardsummarytypedef)
- [DatumPaginatorTypeDef](./type_defs.md#datumpaginatortypedef)
- [DatumTypeDef](./type_defs.md#datumtypedef)
- [DeleteAccessPolicyRequestRequestTypeDef](./type_defs.md#deleteaccesspolicyrequestrequesttypedef)
- [DeleteAssetModelCompositeModelRequestRequestTypeDef](./type_defs.md#deleteassetmodelcompositemodelrequestrequesttypedef)
- [DeleteAssetModelRequestRequestTypeDef](./type_defs.md#deleteassetmodelrequestrequesttypedef)
- [DeleteAssetRequestRequestTypeDef](./type_defs.md#deleteassetrequestrequesttypedef)
- [DeleteDashboardRequestRequestTypeDef](./type_defs.md#deletedashboardrequestrequesttypedef)
- [DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef)
- [DeleteGatewayRequestRequestTypeDef](./type_defs.md#deletegatewayrequestrequesttypedef)
- [DeletePortalRequestRequestTypeDef](./type_defs.md#deleteportalrequestrequesttypedef)
- [DeleteProjectRequestRequestTypeDef](./type_defs.md#deleteprojectrequestrequesttypedef)
- [DeleteTimeSeriesRequestRequestTypeDef](./type_defs.md#deletetimeseriesrequestrequesttypedef)
- [DescribeAccessPolicyRequestRequestTypeDef](./type_defs.md#describeaccesspolicyrequestrequesttypedef)
- [DescribeActionRequestRequestTypeDef](./type_defs.md#describeactionrequestrequesttypedef)
- [DescribeAssetCompositeModelRequestRequestTypeDef](./type_defs.md#describeassetcompositemodelrequestrequesttypedef)
- [DescribeAssetModelCompositeModelRequestRequestTypeDef](./type_defs.md#describeassetmodelcompositemodelrequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeAssetModelRequestRequestTypeDef](./type_defs.md#describeassetmodelrequestrequesttypedef)
- [DescribeAssetPropertyRequestRequestTypeDef](./type_defs.md#describeassetpropertyrequestrequesttypedef)
- [DescribeAssetRequestRequestTypeDef](./type_defs.md#describeassetrequestrequesttypedef)
- [DescribeBulkImportJobRequestRequestTypeDef](./type_defs.md#describebulkimportjobrequestrequesttypedef)
- [DescribeDashboardRequestRequestTypeDef](./type_defs.md#describedashboardrequestrequesttypedef)
- [DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef)
- [DescribeGatewayCapabilityConfigurationRequestRequestTypeDef](./type_defs.md#describegatewaycapabilityconfigurationrequestrequesttypedef)
- [DescribeGatewayRequestRequestTypeDef](./type_defs.md#describegatewayrequestrequesttypedef)
- [GatewayCapabilitySummaryTypeDef](./type_defs.md#gatewaycapabilitysummarytypedef)
- [LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef)
- [DescribePortalRequestRequestTypeDef](./type_defs.md#describeportalrequestrequesttypedef)
- [ImageLocationTypeDef](./type_defs.md#imagelocationtypedef)
- [PortalTypeEntryOutputTypeDef](./type_defs.md#portaltypeentryoutputtypedef)
- [DescribeProjectRequestRequestTypeDef](./type_defs.md#describeprojectrequestrequesttypedef)
- [RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef)
- [WarmTierRetentionPeriodTypeDef](./type_defs.md#warmtierretentionperiodtypedef)
- [DescribeTimeSeriesRequestRequestTypeDef](./type_defs.md#describetimeseriesrequestrequesttypedef)
- [DetailedErrorTypeDef](./type_defs.md#detailederrortypedef)
- [DisassociateAssetsRequestRequestTypeDef](./type_defs.md#disassociateassetsrequestrequesttypedef)
- [DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef](./type_defs.md#disassociatetimeseriesfromassetpropertyrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ExecuteQueryRequestRequestTypeDef](./type_defs.md#executequeryrequestrequesttypedef)
- [ForwardingConfigTypeDef](./type_defs.md#forwardingconfigtypedef)
- [GreengrassTypeDef](./type_defs.md#greengrasstypedef)
- [GreengrassV2TypeDef](./type_defs.md#greengrassv2typedef)
- [SiemensIETypeDef](./type_defs.md#siemensietypedef)
- [GetAssetPropertyValueRequestRequestTypeDef](./type_defs.md#getassetpropertyvaluerequestrequesttypedef)
- [GetInterpolatedAssetPropertyValuesRequestRequestTypeDef](./type_defs.md#getinterpolatedassetpropertyvaluesrequestrequesttypedef)
- [GroupIdentityTypeDef](./type_defs.md#groupidentitytypedef)
- [IAMRoleIdentityTypeDef](./type_defs.md#iamroleidentitytypedef)
- [IAMUserIdentityTypeDef](./type_defs.md#iamuseridentitytypedef)
- [UserIdentityTypeDef](./type_defs.md#useridentitytypedef)
- [InternalFailureExceptionTypeDef](./type_defs.md#internalfailureexceptiontypedef)
- [InvalidRequestExceptionTypeDef](./type_defs.md#invalidrequestexceptiontypedef)
- [InvokeAssistantRequestRequestTypeDef](./type_defs.md#invokeassistantrequestrequesttypedef)
- [JobSummaryTypeDef](./type_defs.md#jobsummarytypedef)
- [KendraSourceDetailTypeDef](./type_defs.md#kendrasourcedetailtypedef)
- [LimitExceededExceptionTypeDef](./type_defs.md#limitexceededexceptiontypedef)
- [ListAccessPoliciesRequestRequestTypeDef](./type_defs.md#listaccesspoliciesrequestrequesttypedef)
- [ListActionsRequestRequestTypeDef](./type_defs.md#listactionsrequestrequesttypedef)
- [ListAssetModelCompositeModelsRequestRequestTypeDef](./type_defs.md#listassetmodelcompositemodelsrequestrequesttypedef)
- [ListAssetModelPropertiesRequestRequestTypeDef](./type_defs.md#listassetmodelpropertiesrequestrequesttypedef)
- [ListAssetModelsRequestRequestTypeDef](./type_defs.md#listassetmodelsrequestrequesttypedef)
- [ListAssetPropertiesRequestRequestTypeDef](./type_defs.md#listassetpropertiesrequestrequesttypedef)
- [ListAssetRelationshipsRequestRequestTypeDef](./type_defs.md#listassetrelationshipsrequestrequesttypedef)
- [ListAssetsRequestRequestTypeDef](./type_defs.md#listassetsrequestrequesttypedef)
- [ListAssociatedAssetsRequestRequestTypeDef](./type_defs.md#listassociatedassetsrequestrequesttypedef)
- [ListBulkImportJobsRequestRequestTypeDef](./type_defs.md#listbulkimportjobsrequestrequesttypedef)
- [ListCompositionRelationshipsRequestRequestTypeDef](./type_defs.md#listcompositionrelationshipsrequestrequesttypedef)
- [ListDashboardsRequestRequestTypeDef](./type_defs.md#listdashboardsrequestrequesttypedef)
- [ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef)
- [ListGatewaysRequestRequestTypeDef](./type_defs.md#listgatewaysrequestrequesttypedef)
- [ListPortalsRequestRequestTypeDef](./type_defs.md#listportalsrequestrequesttypedef)
- [ListProjectAssetsRequestRequestTypeDef](./type_defs.md#listprojectassetsrequestrequesttypedef)
- [ListProjectsRequestRequestTypeDef](./type_defs.md#listprojectsrequestrequesttypedef)
- [ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTimeSeriesRequestRequestTypeDef](./type_defs.md#listtimeseriesrequestrequesttypedef)
- [TimeSeriesSummaryTypeDef](./type_defs.md#timeseriessummarytypedef)
- [LocationTypeDef](./type_defs.md#locationtypedef)
- [MetricProcessingConfigTypeDef](./type_defs.md#metricprocessingconfigtypedef)
- [TumblingWindowTypeDef](./type_defs.md#tumblingwindowtypedef)
- [MonitorErrorDetailsTypeDef](./type_defs.md#monitorerrordetailstypedef)
- [PortalResourceTypeDef](./type_defs.md#portalresourcetypedef)
- [PortalTypeEntryTypeDef](./type_defs.md#portaltypeentrytypedef)
- [ProjectResourceTypeDef](./type_defs.md#projectresourcetypedef)
- [PutDefaultEncryptionConfigurationRequestRequestTypeDef](./type_defs.md#putdefaultencryptionconfigurationrequestrequesttypedef)
- [ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef)
- [ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef)
- [TraceTypeDef](./type_defs.md#tracetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAssetPropertyRequestRequestTypeDef](./type_defs.md#updateassetpropertyrequestrequesttypedef)
- [UpdateAssetRequestRequestTypeDef](./type_defs.md#updateassetrequestrequesttypedef)
- [UpdateDashboardRequestRequestTypeDef](./type_defs.md#updatedashboardrequestrequesttypedef)
- [UpdateGatewayCapabilityConfigurationRequestRequestTypeDef](./type_defs.md#updategatewaycapabilityconfigurationrequestrequesttypedef)
- [UpdateGatewayRequestRequestTypeDef](./type_defs.md#updategatewayrequestrequesttypedef)
- [UpdateProjectRequestRequestTypeDef](./type_defs.md#updateprojectrequestrequesttypedef)
- [ActionSummaryTypeDef](./type_defs.md#actionsummarytypedef)
- [ExecuteActionRequestRequestTypeDef](./type_defs.md#executeactionrequestrequesttypedef)
- [AggregatedValueTypeDef](./type_defs.md#aggregatedvaluetypedef)
- [AssetCompositeModelSummaryTypeDef](./type_defs.md#assetcompositemodelsummarytypedef)
- [AssetRelationshipSummaryTypeDef](./type_defs.md#assetrelationshipsummarytypedef)
- [AssetModelCompositeModelSummaryTypeDef](./type_defs.md#assetmodelcompositemodelsummarytypedef)
- [VariableValueOutputTypeDef](./type_defs.md#variablevalueoutputtypedef)
- [VariableValueTypeDef](./type_defs.md#variablevaluetypedef)
- [AssetPropertySummaryTypeDef](./type_defs.md#assetpropertysummarytypedef)
- [AssetPropertyTypeDef](./type_defs.md#assetpropertytypedef)
- [BatchPutAssetPropertyErrorTypeDef](./type_defs.md#batchputassetpropertyerrortypedef)
- [AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef)
- [InterpolatedAssetPropertyValueTypeDef](./type_defs.md#interpolatedassetpropertyvaluetypedef)
- [BatchAssociateProjectAssetsResponseTypeDef](./type_defs.md#batchassociateprojectassetsresponsetypedef)
- [BatchDisassociateProjectAssetsResponseTypeDef](./type_defs.md#batchdisassociateprojectassetsresponsetypedef)
- [CreateAccessPolicyResponseTypeDef](./type_defs.md#createaccesspolicyresponsetypedef)
- [CreateBulkImportJobResponseTypeDef](./type_defs.md#createbulkimportjobresponsetypedef)
- [CreateDashboardResponseTypeDef](./type_defs.md#createdashboardresponsetypedef)
- [CreateGatewayResponseTypeDef](./type_defs.md#creategatewayresponsetypedef)
- [CreateProjectResponseTypeDef](./type_defs.md#createprojectresponsetypedef)
- [DescribeActionResponseTypeDef](./type_defs.md#describeactionresponsetypedef)
- [DescribeDashboardResponseTypeDef](./type_defs.md#describedashboardresponsetypedef)
- [DescribeGatewayCapabilityConfigurationResponseTypeDef](./type_defs.md#describegatewaycapabilityconfigurationresponsetypedef)
- [DescribeProjectResponseTypeDef](./type_defs.md#describeprojectresponsetypedef)
- [DescribeTimeSeriesResponseTypeDef](./type_defs.md#describetimeseriesresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExecuteActionResponseTypeDef](./type_defs.md#executeactionresponsetypedef)
- [ListProjectAssetsResponseTypeDef](./type_defs.md#listprojectassetsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateGatewayCapabilityConfigurationResponseTypeDef](./type_defs.md#updategatewaycapabilityconfigurationresponsetypedef)
- [BatchGetAssetPropertyAggregatesEntryTypeDef](./type_defs.md#batchgetassetpropertyaggregatesentrytypedef)
- [BatchGetAssetPropertyValueHistoryEntryTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryentrytypedef)
- [GetAssetPropertyAggregatesRequestRequestTypeDef](./type_defs.md#getassetpropertyaggregatesrequestrequesttypedef)
- [GetAssetPropertyValueHistoryRequestRequestTypeDef](./type_defs.md#getassetpropertyvaluehistoryrequestrequesttypedef)
- [BatchGetAssetPropertyAggregatesSkippedEntryTypeDef](./type_defs.md#batchgetassetpropertyaggregatesskippedentrytypedef)
- [BatchGetAssetPropertyValueRequestRequestTypeDef](./type_defs.md#batchgetassetpropertyvaluerequestrequesttypedef)
- [BatchGetAssetPropertyValueSkippedEntryTypeDef](./type_defs.md#batchgetassetpropertyvalueskippedentrytypedef)
- [BatchGetAssetPropertyValueHistorySkippedEntryTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryskippedentrytypedef)
- [ImageFileTypeDef](./type_defs.md#imagefiletypedef)
- [ColumnInfoTypeDef](./type_defs.md#columninfotypedef)
- [CompositionDetailsTypeDef](./type_defs.md#compositiondetailstypedef)
- [ListCompositionRelationshipsResponseTypeDef](./type_defs.md#listcompositionrelationshipsresponsetypedef)
- [ConfigurationStatusTypeDef](./type_defs.md#configurationstatustypedef)
- [FileFormatOutputTypeDef](./type_defs.md#fileformatoutputtypedef)
- [CsvUnionTypeDef](./type_defs.md#csvuniontypedef)
- [MultiLayerStorageTypeDef](./type_defs.md#multilayerstoragetypedef)
- [ListDashboardsResponseTypeDef](./type_defs.md#listdashboardsresponsetypedef)
- [RowPaginatorTypeDef](./type_defs.md#rowpaginatortypedef)
- [RowTypeDef](./type_defs.md#rowtypedef)
- [DescribeAssetModelRequestAssetModelActiveWaitTypeDef](./type_defs.md#describeassetmodelrequestassetmodelactivewaittypedef)
- [DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef](./type_defs.md#describeassetmodelrequestassetmodelnotexistswaittypedef)
- [DescribeAssetRequestAssetActiveWaitTypeDef](./type_defs.md#describeassetrequestassetactivewaittypedef)
- [DescribeAssetRequestAssetNotExistsWaitTypeDef](./type_defs.md#describeassetrequestassetnotexistswaittypedef)
- [DescribePortalRequestPortalActiveWaitTypeDef](./type_defs.md#describeportalrequestportalactivewaittypedef)
- [DescribePortalRequestPortalNotExistsWaitTypeDef](./type_defs.md#describeportalrequestportalnotexistswaittypedef)
- [DescribeLoggingOptionsResponseTypeDef](./type_defs.md#describeloggingoptionsresponsetypedef)
- [PutLoggingOptionsRequestRequestTypeDef](./type_defs.md#putloggingoptionsrequestrequesttypedef)
- [ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef)
- [ExecuteQueryRequestExecuteQueryPaginateTypeDef](./type_defs.md#executequeryrequestexecutequerypaginatetypedef)
- [GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef](./type_defs.md#getassetpropertyaggregatesrequestgetassetpropertyaggregatespaginatetypedef)
- [GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef](./type_defs.md#getassetpropertyvaluehistoryrequestgetassetpropertyvaluehistorypaginatetypedef)
- [GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef](./type_defs.md#getinterpolatedassetpropertyvaluesrequestgetinterpolatedassetpropertyvaluespaginatetypedef)
- [ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef](./type_defs.md#listaccesspoliciesrequestlistaccesspoliciespaginatetypedef)
- [ListActionsRequestListActionsPaginateTypeDef](./type_defs.md#listactionsrequestlistactionspaginatetypedef)
- [ListAssetModelCompositeModelsRequestListAssetModelCompositeModelsPaginateTypeDef](./type_defs.md#listassetmodelcompositemodelsrequestlistassetmodelcompositemodelspaginatetypedef)
- [ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef](./type_defs.md#listassetmodelpropertiesrequestlistassetmodelpropertiespaginatetypedef)
- [ListAssetModelsRequestListAssetModelsPaginateTypeDef](./type_defs.md#listassetmodelsrequestlistassetmodelspaginatetypedef)
- [ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef](./type_defs.md#listassetpropertiesrequestlistassetpropertiespaginatetypedef)
- [ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef](./type_defs.md#listassetrelationshipsrequestlistassetrelationshipspaginatetypedef)
- [ListAssetsRequestListAssetsPaginateTypeDef](./type_defs.md#listassetsrequestlistassetspaginatetypedef)
- [ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef](./type_defs.md#listassociatedassetsrequestlistassociatedassetspaginatetypedef)
- [ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef](./type_defs.md#listbulkimportjobsrequestlistbulkimportjobspaginatetypedef)
- [ListCompositionRelationshipsRequestListCompositionRelationshipsPaginateTypeDef](./type_defs.md#listcompositionrelationshipsrequestlistcompositionrelationshipspaginatetypedef)
- [ListDashboardsRequestListDashboardsPaginateTypeDef](./type_defs.md#listdashboardsrequestlistdashboardspaginatetypedef)
- [ListDatasetsRequestListDatasetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef)
- [ListGatewaysRequestListGatewaysPaginateTypeDef](./type_defs.md#listgatewaysrequestlistgatewayspaginatetypedef)
- [ListPortalsRequestListPortalsPaginateTypeDef](./type_defs.md#listportalsrequestlistportalspaginatetypedef)
- [ListProjectAssetsRequestListProjectAssetsPaginateTypeDef](./type_defs.md#listprojectassetsrequestlistprojectassetspaginatetypedef)
- [ListProjectsRequestListProjectsPaginateTypeDef](./type_defs.md#listprojectsrequestlistprojectspaginatetypedef)
- [ListTimeSeriesRequestListTimeSeriesPaginateTypeDef](./type_defs.md#listtimeseriesrequestlisttimeseriespaginatetypedef)
- [MeasurementProcessingConfigTypeDef](./type_defs.md#measurementprocessingconfigtypedef)
- [TransformProcessingConfigTypeDef](./type_defs.md#transformprocessingconfigtypedef)
- [GatewayPlatformTypeDef](./type_defs.md#gatewayplatformtypedef)
- [IdentityTypeDef](./type_defs.md#identitytypedef)
- [ListBulkImportJobsResponseTypeDef](./type_defs.md#listbulkimportjobsresponsetypedef)
- [SourceDetailTypeDef](./type_defs.md#sourcedetailtypedef)
- [ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef)
- [ListTimeSeriesResponseTypeDef](./type_defs.md#listtimeseriesresponsetypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [MetricWindowTypeDef](./type_defs.md#metricwindowtypedef)
- [PortalStatusTypeDef](./type_defs.md#portalstatustypedef)
- [PortalTypeEntryUnionTypeDef](./type_defs.md#portaltypeentryuniontypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [ListActionsResponseTypeDef](./type_defs.md#listactionsresponsetypedef)
- [BatchGetAssetPropertyAggregatesSuccessEntryTypeDef](./type_defs.md#batchgetassetpropertyaggregatessuccessentrytypedef)
- [GetAssetPropertyAggregatesResponseTypeDef](./type_defs.md#getassetpropertyaggregatesresponsetypedef)
- [ListAssetRelationshipsResponseTypeDef](./type_defs.md#listassetrelationshipsresponsetypedef)
- [ListAssetModelCompositeModelsResponseTypeDef](./type_defs.md#listassetmodelcompositemodelsresponsetypedef)
- [ExpressionVariableOutputTypeDef](./type_defs.md#expressionvariableoutputtypedef)
- [VariableValueUnionTypeDef](./type_defs.md#variablevalueuniontypedef)
- [ListAssetPropertiesResponseTypeDef](./type_defs.md#listassetpropertiesresponsetypedef)
- [AssetCompositeModelTypeDef](./type_defs.md#assetcompositemodeltypedef)
- [DescribeAssetCompositeModelResponseTypeDef](./type_defs.md#describeassetcompositemodelresponsetypedef)
- [BatchPutAssetPropertyErrorEntryTypeDef](./type_defs.md#batchputassetpropertyerrorentrytypedef)
- [BatchGetAssetPropertyValueHistorySuccessEntryTypeDef](./type_defs.md#batchgetassetpropertyvaluehistorysuccessentrytypedef)
- [BatchGetAssetPropertyValueSuccessEntryTypeDef](./type_defs.md#batchgetassetpropertyvaluesuccessentrytypedef)
- [GetAssetPropertyValueHistoryResponseTypeDef](./type_defs.md#getassetpropertyvaluehistoryresponsetypedef)
- [GetAssetPropertyValueResponseTypeDef](./type_defs.md#getassetpropertyvalueresponsetypedef)
- [PutAssetPropertyValueEntryTypeDef](./type_defs.md#putassetpropertyvalueentrytypedef)
- [GetInterpolatedAssetPropertyValuesResponseTypeDef](./type_defs.md#getinterpolatedassetpropertyvaluesresponsetypedef)
- [BatchGetAssetPropertyAggregatesRequestRequestTypeDef](./type_defs.md#batchgetassetpropertyaggregatesrequestrequesttypedef)
- [BatchGetAssetPropertyValueHistoryRequestRequestTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryrequestrequesttypedef)
- [ImageTypeDef](./type_defs.md#imagetypedef)
- [DescribeDefaultEncryptionConfigurationResponseTypeDef](./type_defs.md#describedefaultencryptionconfigurationresponsetypedef)
- [PutDefaultEncryptionConfigurationResponseTypeDef](./type_defs.md#putdefaultencryptionconfigurationresponsetypedef)
- [JobConfigurationOutputTypeDef](./type_defs.md#jobconfigurationoutputtypedef)
- [FileFormatTypeDef](./type_defs.md#fileformattypedef)
- [DescribeStorageConfigurationResponseTypeDef](./type_defs.md#describestorageconfigurationresponsetypedef)
- [PutStorageConfigurationRequestRequestTypeDef](./type_defs.md#putstorageconfigurationrequestrequesttypedef)
- [PutStorageConfigurationResponseTypeDef](./type_defs.md#putstorageconfigurationresponsetypedef)
- [ExecuteQueryResponsePaginatorTypeDef](./type_defs.md#executequeryresponsepaginatortypedef)
- [ExecuteQueryResponseTypeDef](./type_defs.md#executequeryresponsetypedef)
- [AssetModelStatusTypeDef](./type_defs.md#assetmodelstatustypedef)
- [AssetStatusTypeDef](./type_defs.md#assetstatustypedef)
- [DatasetStatusTypeDef](./type_defs.md#datasetstatustypedef)
- [MeasurementTypeDef](./type_defs.md#measurementtypedef)
- [CreateGatewayRequestRequestTypeDef](./type_defs.md#creategatewayrequestrequesttypedef)
- [DescribeGatewayResponseTypeDef](./type_defs.md#describegatewayresponsetypedef)
- [GatewaySummaryTypeDef](./type_defs.md#gatewaysummarytypedef)
- [DatasetSourceTypeDef](./type_defs.md#datasetsourcetypedef)
- [DataSetReferenceTypeDef](./type_defs.md#datasetreferencetypedef)
- [CreatePortalResponseTypeDef](./type_defs.md#createportalresponsetypedef)
- [DeletePortalResponseTypeDef](./type_defs.md#deleteportalresponsetypedef)
- [DescribePortalResponseTypeDef](./type_defs.md#describeportalresponsetypedef)
- [PortalSummaryTypeDef](./type_defs.md#portalsummarytypedef)
- [UpdatePortalResponseTypeDef](./type_defs.md#updateportalresponsetypedef)
- [CreatePortalRequestRequestTypeDef](./type_defs.md#createportalrequestrequesttypedef)
- [AccessPolicySummaryTypeDef](./type_defs.md#accesspolicysummarytypedef)
- [CreateAccessPolicyRequestRequestTypeDef](./type_defs.md#createaccesspolicyrequestrequesttypedef)
- [DescribeAccessPolicyResponseTypeDef](./type_defs.md#describeaccesspolicyresponsetypedef)
- [UpdateAccessPolicyRequestRequestTypeDef](./type_defs.md#updateaccesspolicyrequestrequesttypedef)
- [BatchGetAssetPropertyAggregatesResponseTypeDef](./type_defs.md#batchgetassetpropertyaggregatesresponsetypedef)
- [MetricOutputTypeDef](./type_defs.md#metricoutputtypedef)
- [TransformOutputTypeDef](./type_defs.md#transformoutputtypedef)
- [ExpressionVariableTypeDef](./type_defs.md#expressionvariabletypedef)
- [BatchPutAssetPropertyValueResponseTypeDef](./type_defs.md#batchputassetpropertyvalueresponsetypedef)
- [BatchGetAssetPropertyValueHistoryResponseTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryresponsetypedef)
- [BatchGetAssetPropertyValueResponseTypeDef](./type_defs.md#batchgetassetpropertyvalueresponsetypedef)
- [BatchPutAssetPropertyValueRequestRequestTypeDef](./type_defs.md#batchputassetpropertyvaluerequestrequesttypedef)
- [UpdatePortalRequestRequestTypeDef](./type_defs.md#updateportalrequestrequesttypedef)
- [DescribeBulkImportJobResponseTypeDef](./type_defs.md#describebulkimportjobresponsetypedef)
- [FileFormatUnionTypeDef](./type_defs.md#fileformatuniontypedef)
- [AssetModelSummaryTypeDef](./type_defs.md#assetmodelsummarytypedef)
- [CreateAssetModelCompositeModelResponseTypeDef](./type_defs.md#createassetmodelcompositemodelresponsetypedef)
- [CreateAssetModelResponseTypeDef](./type_defs.md#createassetmodelresponsetypedef)
- [DeleteAssetModelCompositeModelResponseTypeDef](./type_defs.md#deleteassetmodelcompositemodelresponsetypedef)
- [DeleteAssetModelResponseTypeDef](./type_defs.md#deleteassetmodelresponsetypedef)
- [UpdateAssetModelCompositeModelResponseTypeDef](./type_defs.md#updateassetmodelcompositemodelresponsetypedef)
- [UpdateAssetModelResponseTypeDef](./type_defs.md#updateassetmodelresponsetypedef)
- [AssetSummaryTypeDef](./type_defs.md#assetsummarytypedef)
- [AssociatedAssetsSummaryTypeDef](./type_defs.md#associatedassetssummarytypedef)
- [CreateAssetResponseTypeDef](./type_defs.md#createassetresponsetypedef)
- [DeleteAssetResponseTypeDef](./type_defs.md#deleteassetresponsetypedef)
- [DescribeAssetResponseTypeDef](./type_defs.md#describeassetresponsetypedef)
- [UpdateAssetResponseTypeDef](./type_defs.md#updateassetresponsetypedef)
- [CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef)
- [DatasetSummaryTypeDef](./type_defs.md#datasetsummarytypedef)
- [DeleteDatasetResponseTypeDef](./type_defs.md#deletedatasetresponsetypedef)
- [UpdateDatasetResponseTypeDef](./type_defs.md#updatedatasetresponsetypedef)
- [ListGatewaysResponseTypeDef](./type_defs.md#listgatewaysresponsetypedef)
- [CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef)
- [DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef)
- [UpdateDatasetRequestRequestTypeDef](./type_defs.md#updatedatasetrequestrequesttypedef)
- [ReferenceTypeDef](./type_defs.md#referencetypedef)
- [ListPortalsResponseTypeDef](./type_defs.md#listportalsresponsetypedef)
- [ListAccessPoliciesResponseTypeDef](./type_defs.md#listaccesspoliciesresponsetypedef)
- [PropertyTypeOutputTypeDef](./type_defs.md#propertytypeoutputtypedef)
- [ExpressionVariableUnionTypeDef](./type_defs.md#expressionvariableuniontypedef)
- [JobConfigurationTypeDef](./type_defs.md#jobconfigurationtypedef)
- [ListAssetModelsResponseTypeDef](./type_defs.md#listassetmodelsresponsetypedef)
- [ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef)
- [ListAssociatedAssetsResponseTypeDef](./type_defs.md#listassociatedassetsresponsetypedef)
- [ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)
- [CitationTypeDef](./type_defs.md#citationtypedef)
- [AssetModelPropertyOutputTypeDef](./type_defs.md#assetmodelpropertyoutputtypedef)
- [AssetModelPropertySummaryTypeDef](./type_defs.md#assetmodelpropertysummarytypedef)
- [PropertyTypeDef](./type_defs.md#propertytypedef)
- [MetricTypeDef](./type_defs.md#metrictypedef)
- [TransformTypeDef](./type_defs.md#transformtypedef)
- [CreateBulkImportJobRequestRequestTypeDef](./type_defs.md#createbulkimportjobrequestrequesttypedef)
- [InvocationOutputTypeDef](./type_defs.md#invocationoutputtypedef)
- [AssetModelCompositeModelOutputTypeDef](./type_defs.md#assetmodelcompositemodeloutputtypedef)
- [DescribeAssetModelCompositeModelResponseTypeDef](./type_defs.md#describeassetmodelcompositemodelresponsetypedef)
- [ListAssetModelPropertiesResponseTypeDef](./type_defs.md#listassetmodelpropertiesresponsetypedef)
- [CompositeModelPropertyTypeDef](./type_defs.md#compositemodelpropertytypedef)
- [MetricUnionTypeDef](./type_defs.md#metricuniontypedef)
- [TransformUnionTypeDef](./type_defs.md#transformuniontypedef)
- [ResponseStreamTypeDef](./type_defs.md#responsestreamtypedef)
- [DescribeAssetModelResponseTypeDef](./type_defs.md#describeassetmodelresponsetypedef)
- [DescribeAssetPropertyResponseTypeDef](./type_defs.md#describeassetpropertyresponsetypedef)
- [PropertyTypeTypeDef](./type_defs.md#propertytypetypedef)
- [InvokeAssistantResponseTypeDef](./type_defs.md#invokeassistantresponsetypedef)
- [PropertyTypeUnionTypeDef](./type_defs.md#propertytypeuniontypedef)
- [AssetModelPropertyDefinitionTypeDef](./type_defs.md#assetmodelpropertydefinitiontypedef)
- [AssetModelPropertyTypeDef](./type_defs.md#assetmodelpropertytypedef)
- [AssetModelCompositeModelDefinitionTypeDef](./type_defs.md#assetmodelcompositemodeldefinitiontypedef)
- [CreateAssetModelCompositeModelRequestRequestTypeDef](./type_defs.md#createassetmodelcompositemodelrequestrequesttypedef)
- [AssetModelPropertyUnionTypeDef](./type_defs.md#assetmodelpropertyuniontypedef)
- [UpdateAssetModelCompositeModelRequestRequestTypeDef](./type_defs.md#updateassetmodelcompositemodelrequestrequesttypedef)
- [CreateAssetModelRequestRequestTypeDef](./type_defs.md#createassetmodelrequestrequesttypedef)
- [AssetModelCompositeModelTypeDef](./type_defs.md#assetmodelcompositemodeltypedef)
- [AssetModelCompositeModelUnionTypeDef](./type_defs.md#assetmodelcompositemodeluniontypedef)
- [UpdateAssetModelRequestRequestTypeDef](./type_defs.md#updateassetmodelrequestrequesttypedef)

