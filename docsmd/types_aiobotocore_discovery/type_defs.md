# Type definitions

> [Index](../README.md) > [ApplicationDiscoveryService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ApplicationDiscoveryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#applicationdiscoveryservice)
    type annotations stubs module [types-aiobotocore-discovery](https://pypi.org/project/types-aiobotocore-discovery/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AgentConfigurationStatusTypeDef

```python
# AgentConfigurationStatusTypeDef definition

class AgentConfigurationStatusTypeDef(TypedDict):
    agentId: NotRequired[str],
    operationSucceeded: NotRequired[bool],
    description: NotRequired[str],
```

## AgentNetworkInfoTypeDef

```python
# AgentNetworkInfoTypeDef definition

class AgentNetworkInfoTypeDef(TypedDict):
    ipAddress: NotRequired[str],
    macAddress: NotRequired[str],
```

## AssociateConfigurationItemsToApplicationRequestRequestTypeDef

```python
# AssociateConfigurationItemsToApplicationRequestRequestTypeDef definition

class AssociateConfigurationItemsToApplicationRequestRequestTypeDef(TypedDict):
    applicationConfigurationId: str,
    configurationIds: Sequence[str],
```

## BatchDeleteAgentErrorTypeDef

```python
# BatchDeleteAgentErrorTypeDef definition

class BatchDeleteAgentErrorTypeDef(TypedDict):
    agentId: str,
    errorMessage: str,
    errorCode: DeleteAgentErrorCodeType,  # (1)
```

1. See [:material-code-brackets: DeleteAgentErrorCodeType](./literals.md#deleteagenterrorcodetype) 
## DeleteAgentTypeDef

```python
# DeleteAgentTypeDef definition

class DeleteAgentTypeDef(TypedDict):
    agentId: str,
    force: NotRequired[bool],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## DeletionWarningTypeDef

```python
# DeletionWarningTypeDef definition

class DeletionWarningTypeDef(TypedDict):
    configurationId: NotRequired[str],
    warningCode: NotRequired[int],
    warningText: NotRequired[str],
```

## FailedConfigurationTypeDef

```python
# FailedConfigurationTypeDef definition

class FailedConfigurationTypeDef(TypedDict):
    configurationId: NotRequired[str],
    errorStatusCode: NotRequired[int],
    errorMessage: NotRequired[str],
```

## BatchDeleteImportDataErrorTypeDef

```python
# BatchDeleteImportDataErrorTypeDef definition

class BatchDeleteImportDataErrorTypeDef(TypedDict):
    importTaskId: NotRequired[str],
    errorCode: NotRequired[BatchDeleteImportDataErrorCodeType],  # (1)
    errorDescription: NotRequired[str],
```

1. See [:material-code-brackets: BatchDeleteImportDataErrorCodeType](./literals.md#batchdeleteimportdataerrorcodetype) 
## BatchDeleteImportDataRequestRequestTypeDef

```python
# BatchDeleteImportDataRequestRequestTypeDef definition

class BatchDeleteImportDataRequestRequestTypeDef(TypedDict):
    importTaskIds: Sequence[str],
    deleteHistory: NotRequired[bool],
```

## ConfigurationTagTypeDef

```python
# ConfigurationTagTypeDef definition

class ConfigurationTagTypeDef(TypedDict):
    configurationType: NotRequired[ConfigurationItemTypeType],  # (1)
    configurationId: NotRequired[str],
    key: NotRequired[str],
    value: NotRequired[str],
    timeOfCreation: NotRequired[datetime],
```

1. See [:material-code-brackets: ConfigurationItemTypeType](./literals.md#configurationitemtypetype) 
## ContinuousExportDescriptionTypeDef

```python
# ContinuousExportDescriptionTypeDef definition

class ContinuousExportDescriptionTypeDef(TypedDict):
    exportId: NotRequired[str],
    status: NotRequired[ContinuousExportStatusType],  # (1)
    statusDetail: NotRequired[str],
    s3Bucket: NotRequired[str],
    startTime: NotRequired[datetime],
    stopTime: NotRequired[datetime],
    dataSource: NotRequired[DataSourceType],  # (2)
    schemaStorageConfig: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ContinuousExportStatusType](./literals.md#continuousexportstatustype) 
2. See [:material-code-brackets: DataSourceType](./literals.md#datasourcetype) 
## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    wave: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## CustomerAgentInfoTypeDef

```python
# CustomerAgentInfoTypeDef definition

class CustomerAgentInfoTypeDef(TypedDict):
    activeAgents: int,
    healthyAgents: int,
    blackListedAgents: int,
    shutdownAgents: int,
    unhealthyAgents: int,
    totalAgents: int,
    unknownAgents: int,
```

## CustomerAgentlessCollectorInfoTypeDef

```python
# CustomerAgentlessCollectorInfoTypeDef definition

class CustomerAgentlessCollectorInfoTypeDef(TypedDict):
    activeAgentlessCollectors: int,
    healthyAgentlessCollectors: int,
    denyListedAgentlessCollectors: int,
    shutdownAgentlessCollectors: int,
    unhealthyAgentlessCollectors: int,
    totalAgentlessCollectors: int,
    unknownAgentlessCollectors: int,
```

## CustomerConnectorInfoTypeDef

```python
# CustomerConnectorInfoTypeDef definition

class CustomerConnectorInfoTypeDef(TypedDict):
    activeConnectors: int,
    healthyConnectors: int,
    blackListedConnectors: int,
    shutdownConnectors: int,
    unhealthyConnectors: int,
    totalConnectors: int,
    unknownConnectors: int,
```

## CustomerMeCollectorInfoTypeDef

```python
# CustomerMeCollectorInfoTypeDef definition

class CustomerMeCollectorInfoTypeDef(TypedDict):
    activeMeCollectors: int,
    healthyMeCollectors: int,
    denyListedMeCollectors: int,
    shutdownMeCollectors: int,
    unhealthyMeCollectors: int,
    totalMeCollectors: int,
    unknownMeCollectors: int,
```

## DeleteApplicationsRequestRequestTypeDef

```python
# DeleteApplicationsRequestRequestTypeDef definition

class DeleteApplicationsRequestRequestTypeDef(TypedDict):
    configurationIds: Sequence[str],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    name: str,
    values: Sequence[str],
    condition: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeBatchDeleteConfigurationTaskRequestRequestTypeDef

```python
# DescribeBatchDeleteConfigurationTaskRequestRequestTypeDef definition

class DescribeBatchDeleteConfigurationTaskRequestRequestTypeDef(TypedDict):
    taskId: str,
```

## DescribeConfigurationsRequestRequestTypeDef

```python
# DescribeConfigurationsRequestRequestTypeDef definition

class DescribeConfigurationsRequestRequestTypeDef(TypedDict):
    configurationIds: Sequence[str],
```

## DescribeContinuousExportsRequestRequestTypeDef

```python
# DescribeContinuousExportsRequestRequestTypeDef definition

class DescribeContinuousExportsRequestRequestTypeDef(TypedDict):
    exportIds: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## DescribeExportConfigurationsRequestRequestTypeDef

```python
# DescribeExportConfigurationsRequestRequestTypeDef definition

class DescribeExportConfigurationsRequestRequestTypeDef(TypedDict):
    exportIds: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ExportInfoTypeDef

```python
# ExportInfoTypeDef definition

class ExportInfoTypeDef(TypedDict):
    exportId: str,
    exportStatus: ExportStatusType,  # (1)
    statusMessage: str,
    exportRequestTime: datetime,
    configurationsDownloadUrl: NotRequired[str],
    isTruncated: NotRequired[bool],
    requestedStartTime: NotRequired[datetime],
    requestedEndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
## ExportFilterTypeDef

```python
# ExportFilterTypeDef definition

class ExportFilterTypeDef(TypedDict):
    name: str,
    values: Sequence[str],
    condition: str,
```

## ImportTaskFilterTypeDef

```python
# ImportTaskFilterTypeDef definition

class ImportTaskFilterTypeDef(TypedDict):
    name: NotRequired[ImportTaskFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ImportTaskFilterNameType](./literals.md#importtaskfilternametype) 
## ImportTaskTypeDef

```python
# ImportTaskTypeDef definition

class ImportTaskTypeDef(TypedDict):
    importTaskId: NotRequired[str],
    clientRequestToken: NotRequired[str],
    name: NotRequired[str],
    importUrl: NotRequired[str],
    status: NotRequired[ImportStatusType],  # (1)
    importRequestTime: NotRequired[datetime],
    importCompletionTime: NotRequired[datetime],
    importDeletedTime: NotRequired[datetime],
    fileClassification: NotRequired[FileClassificationType],  # (2)
    serverImportSuccess: NotRequired[int],
    serverImportFailure: NotRequired[int],
    applicationImportSuccess: NotRequired[int],
    applicationImportFailure: NotRequired[int],
    errorsAndFailedEntriesZip: NotRequired[str],
```

1. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
2. See [:material-code-brackets: FileClassificationType](./literals.md#fileclassificationtype) 
## TagFilterTypeDef

```python
# TagFilterTypeDef definition

class TagFilterTypeDef(TypedDict):
    name: str,
    values: Sequence[str],
```

## DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef

```python
# DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef definition

class DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef(TypedDict):
    applicationConfigurationId: str,
    configurationIds: Sequence[str],
```

## ReservedInstanceOptionsTypeDef

```python
# ReservedInstanceOptionsTypeDef definition

class ReservedInstanceOptionsTypeDef(TypedDict):
    purchasingOption: PurchasingOptionType,  # (1)
    offeringClass: OfferingClassType,  # (2)
    termLength: TermLengthType,  # (3)
```

1. See [:material-code-brackets: PurchasingOptionType](./literals.md#purchasingoptiontype) 
2. See [:material-code-brackets: OfferingClassType](./literals.md#offeringclasstype) 
3. See [:material-code-brackets: TermLengthType](./literals.md#termlengthtype) 
## UsageMetricBasisTypeDef

```python
# UsageMetricBasisTypeDef definition

class UsageMetricBasisTypeDef(TypedDict):
    name: NotRequired[str],
    percentageAdjust: NotRequired[float],
```

## OrderByElementTypeDef

```python
# OrderByElementTypeDef definition

class OrderByElementTypeDef(TypedDict):
    fieldName: str,
    sortOrder: NotRequired[OrderStringType],  # (1)
```

1. See [:material-code-brackets: OrderStringType](./literals.md#orderstringtype) 
## ListServerNeighborsRequestRequestTypeDef

```python
# ListServerNeighborsRequestRequestTypeDef definition

class ListServerNeighborsRequestRequestTypeDef(TypedDict):
    configurationId: str,
    portInformationNeeded: NotRequired[bool],
    neighborConfigurationIds: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## NeighborConnectionDetailTypeDef

```python
# NeighborConnectionDetailTypeDef definition

class NeighborConnectionDetailTypeDef(TypedDict):
    sourceServerId: str,
    destinationServerId: str,
    connectionsCount: int,
    destinationPort: NotRequired[int],
    transportProtocol: NotRequired[str],
```

## StartBatchDeleteConfigurationTaskRequestRequestTypeDef

```python
# StartBatchDeleteConfigurationTaskRequestRequestTypeDef definition

class StartBatchDeleteConfigurationTaskRequestRequestTypeDef(TypedDict):
    configurationType: DeletionConfigurationItemTypeType,  # (1)
    configurationIds: Sequence[str],
```

1. See [:material-code-brackets: DeletionConfigurationItemTypeType](./literals.md#deletionconfigurationitemtypetype) 
## StartDataCollectionByAgentIdsRequestRequestTypeDef

```python
# StartDataCollectionByAgentIdsRequestRequestTypeDef definition

class StartDataCollectionByAgentIdsRequestRequestTypeDef(TypedDict):
    agentIds: Sequence[str],
```

## StartImportTaskRequestRequestTypeDef

```python
# StartImportTaskRequestRequestTypeDef definition

class StartImportTaskRequestRequestTypeDef(TypedDict):
    name: str,
    importUrl: str,
    clientRequestToken: NotRequired[str],
```

## StopContinuousExportRequestRequestTypeDef

```python
# StopContinuousExportRequestRequestTypeDef definition

class StopContinuousExportRequestRequestTypeDef(TypedDict):
    exportId: str,
```

## StopDataCollectionByAgentIdsRequestRequestTypeDef

```python
# StopDataCollectionByAgentIdsRequestRequestTypeDef definition

class StopDataCollectionByAgentIdsRequestRequestTypeDef(TypedDict):
    agentIds: Sequence[str],
```

## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    configurationId: str,
    name: NotRequired[str],
    description: NotRequired[str],
    wave: NotRequired[str],
```

## AgentInfoTypeDef

```python
# AgentInfoTypeDef definition

class AgentInfoTypeDef(TypedDict):
    agentId: NotRequired[str],
    hostName: NotRequired[str],
    agentNetworkInfoList: NotRequired[List[AgentNetworkInfoTypeDef]],  # (1)
    connectorId: NotRequired[str],
    version: NotRequired[str],
    health: NotRequired[AgentStatusType],  # (2)
    lastHealthPingTime: NotRequired[str],
    collectionStatus: NotRequired[str],
    agentType: NotRequired[str],
    registeredTime: NotRequired[str],
```

1. See [:material-code-braces: AgentNetworkInfoTypeDef](./type_defs.md#agentnetworkinfotypedef) 
2. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
## BatchDeleteAgentsRequestRequestTypeDef

```python
# BatchDeleteAgentsRequestRequestTypeDef definition

class BatchDeleteAgentsRequestRequestTypeDef(TypedDict):
    deleteAgents: Sequence[DeleteAgentTypeDef],  # (1)
```

1. See [:material-code-braces: DeleteAgentTypeDef](./type_defs.md#deleteagenttypedef) 
## BatchDeleteAgentsResponseTypeDef

```python
# BatchDeleteAgentsResponseTypeDef definition

class BatchDeleteAgentsResponseTypeDef(TypedDict):
    errors: List[BatchDeleteAgentErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteAgentErrorTypeDef](./type_defs.md#batchdeleteagenterrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationResponseTypeDef

```python
# CreateApplicationResponseTypeDef definition

class CreateApplicationResponseTypeDef(TypedDict):
    configurationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConfigurationsResponseTypeDef

```python
# DescribeConfigurationsResponseTypeDef definition

class DescribeConfigurationsResponseTypeDef(TypedDict):
    configurations: List[Dict[str, str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportConfigurationsResponseTypeDef

```python
# ExportConfigurationsResponseTypeDef definition

class ExportConfigurationsResponseTypeDef(TypedDict):
    exportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationsResponseTypeDef

```python
# ListConfigurationsResponseTypeDef definition

class ListConfigurationsResponseTypeDef(TypedDict):
    configurations: List[Dict[str, str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartBatchDeleteConfigurationTaskResponseTypeDef

```python
# StartBatchDeleteConfigurationTaskResponseTypeDef definition

class StartBatchDeleteConfigurationTaskResponseTypeDef(TypedDict):
    taskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartContinuousExportResponseTypeDef

```python
# StartContinuousExportResponseTypeDef definition

class StartContinuousExportResponseTypeDef(TypedDict):
    exportId: str,
    s3Bucket: str,
    startTime: datetime,
    dataSource: DataSourceType,  # (1)
    schemaStorageConfig: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DataSourceType](./literals.md#datasourcetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDataCollectionByAgentIdsResponseTypeDef

```python
# StartDataCollectionByAgentIdsResponseTypeDef definition

class StartDataCollectionByAgentIdsResponseTypeDef(TypedDict):
    agentsConfigurationStatus: List[AgentConfigurationStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentConfigurationStatusTypeDef](./type_defs.md#agentconfigurationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartExportTaskResponseTypeDef

```python
# StartExportTaskResponseTypeDef definition

class StartExportTaskResponseTypeDef(TypedDict):
    exportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopContinuousExportResponseTypeDef

```python
# StopContinuousExportResponseTypeDef definition

class StopContinuousExportResponseTypeDef(TypedDict):
    startTime: datetime,
    stopTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopDataCollectionByAgentIdsResponseTypeDef

```python
# StopDataCollectionByAgentIdsResponseTypeDef definition

class StopDataCollectionByAgentIdsResponseTypeDef(TypedDict):
    agentsConfigurationStatus: List[AgentConfigurationStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentConfigurationStatusTypeDef](./type_defs.md#agentconfigurationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteConfigurationTaskTypeDef

```python
# BatchDeleteConfigurationTaskTypeDef definition

class BatchDeleteConfigurationTaskTypeDef(TypedDict):
    taskId: NotRequired[str],
    status: NotRequired[BatchDeleteConfigurationTaskStatusType],  # (1)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    configurationType: NotRequired[DeletionConfigurationItemTypeType],  # (2)
    requestedConfigurations: NotRequired[List[str]],
    deletedConfigurations: NotRequired[List[str]],
    failedConfigurations: NotRequired[List[FailedConfigurationTypeDef]],  # (3)
    deletionWarnings: NotRequired[List[DeletionWarningTypeDef]],  # (4)
```

1. See [:material-code-brackets: BatchDeleteConfigurationTaskStatusType](./literals.md#batchdeleteconfigurationtaskstatustype) 
2. See [:material-code-brackets: DeletionConfigurationItemTypeType](./literals.md#deletionconfigurationitemtypetype) 
3. See [:material-code-braces: FailedConfigurationTypeDef](./type_defs.md#failedconfigurationtypedef) 
4. See [:material-code-braces: DeletionWarningTypeDef](./type_defs.md#deletionwarningtypedef) 
## BatchDeleteImportDataResponseTypeDef

```python
# BatchDeleteImportDataResponseTypeDef definition

class BatchDeleteImportDataResponseTypeDef(TypedDict):
    errors: List[BatchDeleteImportDataErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteImportDataErrorTypeDef](./type_defs.md#batchdeleteimportdataerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTagsResponseTypeDef

```python
# DescribeTagsResponseTypeDef definition

class DescribeTagsResponseTypeDef(TypedDict):
    tags: List[ConfigurationTagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationTagTypeDef](./type_defs.md#configurationtagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContinuousExportsResponseTypeDef

```python
# DescribeContinuousExportsResponseTypeDef definition

class DescribeContinuousExportsResponseTypeDef(TypedDict):
    descriptions: List[ContinuousExportDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ContinuousExportDescriptionTypeDef](./type_defs.md#continuousexportdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTagsRequestRequestTypeDef

```python
# CreateTagsRequestRequestTypeDef definition

class CreateTagsRequestRequestTypeDef(TypedDict):
    configurationIds: Sequence[str],
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DeleteTagsRequestRequestTypeDef

```python
# DeleteTagsRequestRequestTypeDef definition

class DeleteTagsRequestRequestTypeDef(TypedDict):
    configurationIds: Sequence[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetDiscoverySummaryResponseTypeDef

```python
# GetDiscoverySummaryResponseTypeDef definition

class GetDiscoverySummaryResponseTypeDef(TypedDict):
    servers: int,
    applications: int,
    serversMappedToApplications: int,
    serversMappedtoTags: int,
    agentSummary: CustomerAgentInfoTypeDef,  # (1)
    connectorSummary: CustomerConnectorInfoTypeDef,  # (2)
    meCollectorSummary: CustomerMeCollectorInfoTypeDef,  # (3)
    agentlessCollectorSummary: CustomerAgentlessCollectorInfoTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: CustomerAgentInfoTypeDef](./type_defs.md#customeragentinfotypedef) 
2. See [:material-code-braces: CustomerConnectorInfoTypeDef](./type_defs.md#customerconnectorinfotypedef) 
3. See [:material-code-braces: CustomerMeCollectorInfoTypeDef](./type_defs.md#customermecollectorinfotypedef) 
4. See [:material-code-braces: CustomerAgentlessCollectorInfoTypeDef](./type_defs.md#customeragentlesscollectorinfotypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAgentsRequestRequestTypeDef

```python
# DescribeAgentsRequestRequestTypeDef definition

class DescribeAgentsRequestRequestTypeDef(TypedDict):
    agentIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeAgentsRequestPaginateTypeDef

```python
# DescribeAgentsRequestPaginateTypeDef definition

class DescribeAgentsRequestPaginateTypeDef(TypedDict):
    agentIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeContinuousExportsRequestPaginateTypeDef

```python
# DescribeContinuousExportsRequestPaginateTypeDef definition

class DescribeContinuousExportsRequestPaginateTypeDef(TypedDict):
    exportIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeExportConfigurationsRequestPaginateTypeDef

```python
# DescribeExportConfigurationsRequestPaginateTypeDef definition

class DescribeExportConfigurationsRequestPaginateTypeDef(TypedDict):
    exportIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeExportConfigurationsResponseTypeDef

```python
# DescribeExportConfigurationsResponseTypeDef definition

class DescribeExportConfigurationsResponseTypeDef(TypedDict):
    exportsInfo: List[ExportInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportInfoTypeDef](./type_defs.md#exportinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeExportTasksResponseTypeDef

```python
# DescribeExportTasksResponseTypeDef definition

class DescribeExportTasksResponseTypeDef(TypedDict):
    exportsInfo: List[ExportInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportInfoTypeDef](./type_defs.md#exportinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeExportTasksRequestPaginateTypeDef

```python
# DescribeExportTasksRequestPaginateTypeDef definition

class DescribeExportTasksRequestPaginateTypeDef(TypedDict):
    exportIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[ExportFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ExportFilterTypeDef](./type_defs.md#exportfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeExportTasksRequestRequestTypeDef

```python
# DescribeExportTasksRequestRequestTypeDef definition

class DescribeExportTasksRequestRequestTypeDef(TypedDict):
    exportIds: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[ExportFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportFilterTypeDef](./type_defs.md#exportfiltertypedef) 
## DescribeImportTasksRequestPaginateTypeDef

```python
# DescribeImportTasksRequestPaginateTypeDef definition

class DescribeImportTasksRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[ImportTaskFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ImportTaskFilterTypeDef](./type_defs.md#importtaskfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeImportTasksRequestRequestTypeDef

```python
# DescribeImportTasksRequestRequestTypeDef definition

class DescribeImportTasksRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[ImportTaskFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportTaskFilterTypeDef](./type_defs.md#importtaskfiltertypedef) 
## DescribeImportTasksResponseTypeDef

```python
# DescribeImportTasksResponseTypeDef definition

class DescribeImportTasksResponseTypeDef(TypedDict):
    tasks: List[ImportTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportTaskTypeDef](./type_defs.md#importtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartImportTaskResponseTypeDef

```python
# StartImportTaskResponseTypeDef definition

class StartImportTaskResponseTypeDef(TypedDict):
    task: ImportTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportTaskTypeDef](./type_defs.md#importtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTagsRequestPaginateTypeDef

```python
# DescribeTagsRequestPaginateTypeDef definition

class DescribeTagsRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[TagFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeTagsRequestRequestTypeDef

```python
# DescribeTagsRequestRequestTypeDef definition

class DescribeTagsRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[TagFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
## Ec2RecommendationsExportPreferencesTypeDef

```python
# Ec2RecommendationsExportPreferencesTypeDef definition

class Ec2RecommendationsExportPreferencesTypeDef(TypedDict):
    enabled: NotRequired[bool],
    cpuPerformanceMetricBasis: NotRequired[UsageMetricBasisTypeDef],  # (1)
    ramPerformanceMetricBasis: NotRequired[UsageMetricBasisTypeDef],  # (1)
    tenancy: NotRequired[TenancyType],  # (3)
    excludedInstanceTypes: NotRequired[Sequence[str]],
    preferredRegion: NotRequired[str],
    reservedInstanceOptions: NotRequired[ReservedInstanceOptionsTypeDef],  # (4)
```

1. See [:material-code-braces: UsageMetricBasisTypeDef](./type_defs.md#usagemetricbasistypedef) 
2. See [:material-code-braces: UsageMetricBasisTypeDef](./type_defs.md#usagemetricbasistypedef) 
3. See [:material-code-brackets: TenancyType](./literals.md#tenancytype) 
4. See [:material-code-braces: ReservedInstanceOptionsTypeDef](./type_defs.md#reservedinstanceoptionstypedef) 
## ListConfigurationsRequestPaginateTypeDef

```python
# ListConfigurationsRequestPaginateTypeDef definition

class ListConfigurationsRequestPaginateTypeDef(TypedDict):
    configurationType: ConfigurationItemTypeType,  # (1)
    filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    orderBy: NotRequired[Sequence[OrderByElementTypeDef]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ConfigurationItemTypeType](./literals.md#configurationitemtypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: OrderByElementTypeDef](./type_defs.md#orderbyelementtypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfigurationsRequestRequestTypeDef

```python
# ListConfigurationsRequestRequestTypeDef definition

class ListConfigurationsRequestRequestTypeDef(TypedDict):
    configurationType: ConfigurationItemTypeType,  # (1)
    filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    orderBy: NotRequired[Sequence[OrderByElementTypeDef]],  # (3)
```

1. See [:material-code-brackets: ConfigurationItemTypeType](./literals.md#configurationitemtypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: OrderByElementTypeDef](./type_defs.md#orderbyelementtypedef) 
## ListServerNeighborsResponseTypeDef

```python
# ListServerNeighborsResponseTypeDef definition

class ListServerNeighborsResponseTypeDef(TypedDict):
    neighbors: List[NeighborConnectionDetailTypeDef],  # (1)
    knownDependencyCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NeighborConnectionDetailTypeDef](./type_defs.md#neighborconnectiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAgentsResponseTypeDef

```python
# DescribeAgentsResponseTypeDef definition

class DescribeAgentsResponseTypeDef(TypedDict):
    agentsInfo: List[AgentInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AgentInfoTypeDef](./type_defs.md#agentinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBatchDeleteConfigurationTaskResponseTypeDef

```python
# DescribeBatchDeleteConfigurationTaskResponseTypeDef definition

class DescribeBatchDeleteConfigurationTaskResponseTypeDef(TypedDict):
    task: BatchDeleteConfigurationTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteConfigurationTaskTypeDef](./type_defs.md#batchdeleteconfigurationtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportPreferencesTypeDef

```python
# ExportPreferencesTypeDef definition

class ExportPreferencesTypeDef(TypedDict):
    ec2RecommendationsPreferences: NotRequired[Ec2RecommendationsExportPreferencesTypeDef],  # (1)
```

1. See [:material-code-braces: Ec2RecommendationsExportPreferencesTypeDef](./type_defs.md#ec2recommendationsexportpreferencestypedef) 
## StartExportTaskRequestRequestTypeDef

```python
# StartExportTaskRequestRequestTypeDef definition

class StartExportTaskRequestRequestTypeDef(TypedDict):
    exportDataFormat: NotRequired[Sequence[ExportDataFormatType]],  # (1)
    filters: NotRequired[Sequence[ExportFilterTypeDef]],  # (2)
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    preferences: NotRequired[ExportPreferencesTypeDef],  # (3)
```

1. See [:material-code-brackets: ExportDataFormatType](./literals.md#exportdataformattype) 
2. See [:material-code-braces: ExportFilterTypeDef](./type_defs.md#exportfiltertypedef) 
3. See [:material-code-braces: ExportPreferencesTypeDef](./type_defs.md#exportpreferencestypedef) 
