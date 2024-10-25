# Type definitions

> [Index](../README.md) > [NeptuneGraph](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [NeptuneGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph)
    type annotations stubs module [types-aiobotocore-neptune-graph](https://pypi.org/project/types-aiobotocore-neptune-graph/).



## CancelImportTaskInputRequestTypeDef

```python
# CancelImportTaskInputRequestTypeDef definition

class CancelImportTaskInputRequestTypeDef(TypedDict):
    taskIdentifier: str,
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

## CancelQueryInputRequestTypeDef

```python
# CancelQueryInputRequestTypeDef definition

class CancelQueryInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
    queryId: str,
```

## VectorSearchConfigurationTypeDef

```python
# VectorSearchConfigurationTypeDef definition

class VectorSearchConfigurationTypeDef(TypedDict):
    dimension: int,
```

## CreateGraphSnapshotInputRequestTypeDef

```python
# CreateGraphSnapshotInputRequestTypeDef definition

class CreateGraphSnapshotInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
    snapshotName: str,
    tags: NotRequired[Mapping[str, str]],
```

## CreatePrivateGraphEndpointInputRequestTypeDef

```python
# CreatePrivateGraphEndpointInputRequestTypeDef definition

class CreatePrivateGraphEndpointInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
    vpcId: NotRequired[str],
    subnetIds: NotRequired[Sequence[str]],
    vpcSecurityGroupIds: NotRequired[Sequence[str]],
```

## DeleteGraphInputRequestTypeDef

```python
# DeleteGraphInputRequestTypeDef definition

class DeleteGraphInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
    skipSnapshot: bool,
```

## DeleteGraphSnapshotInputRequestTypeDef

```python
# DeleteGraphSnapshotInputRequestTypeDef definition

class DeleteGraphSnapshotInputRequestTypeDef(TypedDict):
    snapshotIdentifier: str,
```

## DeletePrivateGraphEndpointInputRequestTypeDef

```python
# DeletePrivateGraphEndpointInputRequestTypeDef definition

class DeletePrivateGraphEndpointInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
    vpcId: str,
```

## EdgeStructureTypeDef

```python
# EdgeStructureTypeDef definition

class EdgeStructureTypeDef(TypedDict):
    count: NotRequired[int],
    edgeProperties: NotRequired[List[str]],
```

## ExecuteQueryInputRequestTypeDef

```python
# ExecuteQueryInputRequestTypeDef definition

class ExecuteQueryInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
    queryString: str,
    language: QueryLanguageType,  # (1)
    parameters: NotRequired[Mapping[str, Mapping[str, Any]]],
    planCache: NotRequired[PlanCacheTypeType],  # (2)
    explainMode: NotRequired[ExplainModeType],  # (3)
    queryTimeoutMilliseconds: NotRequired[int],
```

1. See [:material-code-brackets: QueryLanguageType](./literals.md#querylanguagetype) 
2. See [:material-code-brackets: PlanCacheTypeType](./literals.md#plancachetypetype) 
3. See [:material-code-brackets: ExplainModeType](./literals.md#explainmodetype) 
## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## GetGraphInputRequestTypeDef

```python
# GetGraphInputRequestTypeDef definition

class GetGraphInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
```

## GetGraphSnapshotInputRequestTypeDef

```python
# GetGraphSnapshotInputRequestTypeDef definition

class GetGraphSnapshotInputRequestTypeDef(TypedDict):
    snapshotIdentifier: str,
```

## GetGraphSummaryInputRequestTypeDef

```python
# GetGraphSummaryInputRequestTypeDef definition

class GetGraphSummaryInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
    mode: NotRequired[GraphSummaryModeType],  # (1)
```

1. See [:material-code-brackets: GraphSummaryModeType](./literals.md#graphsummarymodetype) 
## GetImportTaskInputRequestTypeDef

```python
# GetImportTaskInputRequestTypeDef definition

class GetImportTaskInputRequestTypeDef(TypedDict):
    taskIdentifier: str,
```

## ImportTaskDetailsTypeDef

```python
# ImportTaskDetailsTypeDef definition

class ImportTaskDetailsTypeDef(TypedDict):
    status: str,
    startTime: datetime,
    timeElapsedSeconds: int,
    progressPercentage: int,
    errorCount: int,
    statementCount: int,
    dictionaryEntryCount: int,
    errorDetails: NotRequired[str],
```

## GetPrivateGraphEndpointInputRequestTypeDef

```python
# GetPrivateGraphEndpointInputRequestTypeDef definition

class GetPrivateGraphEndpointInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
    vpcId: str,
```

## GetQueryInputRequestTypeDef

```python
# GetQueryInputRequestTypeDef definition

class GetQueryInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
    queryId: str,
```

## NodeStructureTypeDef

```python
# NodeStructureTypeDef definition

class NodeStructureTypeDef(TypedDict):
    count: NotRequired[int],
    nodeProperties: NotRequired[List[str]],
    distinctOutgoingEdgeLabels: NotRequired[List[str]],
```

## GraphSnapshotSummaryTypeDef

```python
# GraphSnapshotSummaryTypeDef definition

class GraphSnapshotSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    sourceGraphId: NotRequired[str],
    snapshotCreateTime: NotRequired[datetime],
    status: NotRequired[SnapshotStatusType],  # (1)
    kmsKeyIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: SnapshotStatusType](./literals.md#snapshotstatustype) 
## GraphSummaryTypeDef

```python
# GraphSummaryTypeDef definition

class GraphSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: NotRequired[GraphStatusType],  # (1)
    provisionedMemory: NotRequired[int],
    publicConnectivity: NotRequired[bool],
    endpoint: NotRequired[str],
    replicaCount: NotRequired[int],
    kmsKeyIdentifier: NotRequired[str],
    deletionProtection: NotRequired[bool],
```

1. See [:material-code-brackets: GraphStatusType](./literals.md#graphstatustype) 
## NeptuneImportOptionsTypeDef

```python
# NeptuneImportOptionsTypeDef definition

class NeptuneImportOptionsTypeDef(TypedDict):
    s3ExportPath: str,
    s3ExportKmsKeyId: str,
    preserveDefaultVertexLabels: NotRequired[bool],
    preserveEdgeIds: NotRequired[bool],
```

## ImportTaskSummaryTypeDef

```python
# ImportTaskSummaryTypeDef definition

class ImportTaskSummaryTypeDef(TypedDict):
    taskId: str,
    source: str,
    roleArn: str,
    status: ImportTaskStatusType,  # (2)
    graphId: NotRequired[str],
    format: NotRequired[FormatType],  # (1)
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
2. See [:material-code-brackets: ImportTaskStatusType](./literals.md#importtaskstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListGraphSnapshotsInputRequestTypeDef

```python
# ListGraphSnapshotsInputRequestTypeDef definition

class ListGraphSnapshotsInputRequestTypeDef(TypedDict):
    graphIdentifier: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListGraphsInputRequestTypeDef

```python
# ListGraphsInputRequestTypeDef definition

class ListGraphsInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListImportTasksInputRequestTypeDef

```python
# ListImportTasksInputRequestTypeDef definition

class ListImportTasksInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListPrivateGraphEndpointsInputRequestTypeDef

```python
# ListPrivateGraphEndpointsInputRequestTypeDef definition

class ListPrivateGraphEndpointsInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PrivateGraphEndpointSummaryTypeDef

```python
# PrivateGraphEndpointSummaryTypeDef definition

class PrivateGraphEndpointSummaryTypeDef(TypedDict):
    vpcId: str,
    subnetIds: List[str],
    status: PrivateGraphEndpointStatusType,  # (1)
    vpcEndpointId: NotRequired[str],
```

1. See [:material-code-brackets: PrivateGraphEndpointStatusType](./literals.md#privategraphendpointstatustype) 
## ListQueriesInputRequestTypeDef

```python
# ListQueriesInputRequestTypeDef definition

class ListQueriesInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
    maxResults: int,
    state: NotRequired[QueryStateInputType],  # (1)
```

1. See [:material-code-brackets: QueryStateInputType](./literals.md#querystateinputtype) 
## QuerySummaryTypeDef

```python
# QuerySummaryTypeDef definition

class QuerySummaryTypeDef(TypedDict):
    id: NotRequired[str],
    queryString: NotRequired[str],
    waited: NotRequired[int],
    elapsed: NotRequired[int],
    state: NotRequired[QueryStateType],  # (1)
```

1. See [:material-code-brackets: QueryStateType](./literals.md#querystatetype) 
## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ResetGraphInputRequestTypeDef

```python
# ResetGraphInputRequestTypeDef definition

class ResetGraphInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
    skipSnapshot: bool,
```

## RestoreGraphFromSnapshotInputRequestTypeDef

```python
# RestoreGraphFromSnapshotInputRequestTypeDef definition

class RestoreGraphFromSnapshotInputRequestTypeDef(TypedDict):
    snapshotIdentifier: str,
    graphName: str,
    provisionedMemory: NotRequired[int],
    deletionProtection: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
    replicaCount: NotRequired[int],
    publicConnectivity: NotRequired[bool],
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateGraphInputRequestTypeDef

```python
# UpdateGraphInputRequestTypeDef definition

class UpdateGraphInputRequestTypeDef(TypedDict):
    graphIdentifier: str,
    publicConnectivity: NotRequired[bool],
    provisionedMemory: NotRequired[int],
    deletionProtection: NotRequired[bool],
```

## CancelImportTaskOutputTypeDef

```python
# CancelImportTaskOutputTypeDef definition

class CancelImportTaskOutputTypeDef(TypedDict):
    graphId: str,
    taskId: str,
    source: str,
    format: FormatType,  # (1)
    roleArn: str,
    status: ImportTaskStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
2. See [:material-code-brackets: ImportTaskStatusType](./literals.md#importtaskstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGraphSnapshotOutputTypeDef

```python
# CreateGraphSnapshotOutputTypeDef definition

class CreateGraphSnapshotOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    sourceGraphId: str,
    snapshotCreateTime: datetime,
    status: SnapshotStatusType,  # (1)
    kmsKeyIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SnapshotStatusType](./literals.md#snapshotstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePrivateGraphEndpointOutputTypeDef

```python
# CreatePrivateGraphEndpointOutputTypeDef definition

class CreatePrivateGraphEndpointOutputTypeDef(TypedDict):
    vpcId: str,
    subnetIds: List[str],
    status: PrivateGraphEndpointStatusType,  # (1)
    vpcEndpointId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PrivateGraphEndpointStatusType](./literals.md#privategraphendpointstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGraphSnapshotOutputTypeDef

```python
# DeleteGraphSnapshotOutputTypeDef definition

class DeleteGraphSnapshotOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    sourceGraphId: str,
    snapshotCreateTime: datetime,
    status: SnapshotStatusType,  # (1)
    kmsKeyIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SnapshotStatusType](./literals.md#snapshotstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePrivateGraphEndpointOutputTypeDef

```python
# DeletePrivateGraphEndpointOutputTypeDef definition

class DeletePrivateGraphEndpointOutputTypeDef(TypedDict):
    vpcId: str,
    subnetIds: List[str],
    status: PrivateGraphEndpointStatusType,  # (1)
    vpcEndpointId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PrivateGraphEndpointStatusType](./literals.md#privategraphendpointstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteQueryOutputTypeDef

```python
# ExecuteQueryOutputTypeDef definition

class ExecuteQueryOutputTypeDef(TypedDict):
    payload: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGraphSnapshotOutputTypeDef

```python
# GetGraphSnapshotOutputTypeDef definition

class GetGraphSnapshotOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    sourceGraphId: str,
    snapshotCreateTime: datetime,
    status: SnapshotStatusType,  # (1)
    kmsKeyIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SnapshotStatusType](./literals.md#snapshotstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPrivateGraphEndpointOutputTypeDef

```python
# GetPrivateGraphEndpointOutputTypeDef definition

class GetPrivateGraphEndpointOutputTypeDef(TypedDict):
    vpcId: str,
    subnetIds: List[str],
    status: PrivateGraphEndpointStatusType,  # (1)
    vpcEndpointId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PrivateGraphEndpointStatusType](./literals.md#privategraphendpointstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueryOutputTypeDef

```python
# GetQueryOutputTypeDef definition

class GetQueryOutputTypeDef(TypedDict):
    id: str,
    queryString: str,
    waited: int,
    elapsed: int,
    state: QueryStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: QueryStateType](./literals.md#querystatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGraphInputRequestTypeDef

```python
# CreateGraphInputRequestTypeDef definition

class CreateGraphInputRequestTypeDef(TypedDict):
    graphName: str,
    provisionedMemory: int,
    tags: NotRequired[Mapping[str, str]],
    publicConnectivity: NotRequired[bool],
    kmsKeyIdentifier: NotRequired[str],
    vectorSearchConfiguration: NotRequired[VectorSearchConfigurationTypeDef],  # (1)
    replicaCount: NotRequired[int],
    deletionProtection: NotRequired[bool],
```

1. See [:material-code-braces: VectorSearchConfigurationTypeDef](./type_defs.md#vectorsearchconfigurationtypedef) 
## CreateGraphOutputTypeDef

```python
# CreateGraphOutputTypeDef definition

class CreateGraphOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: GraphStatusType,  # (1)
    statusReason: str,
    createTime: datetime,
    provisionedMemory: int,
    endpoint: str,
    publicConnectivity: bool,
    vectorSearchConfiguration: VectorSearchConfigurationTypeDef,  # (2)
    replicaCount: int,
    kmsKeyIdentifier: str,
    sourceSnapshotId: str,
    deletionProtection: bool,
    buildNumber: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: GraphStatusType](./literals.md#graphstatustype) 
2. See [:material-code-braces: VectorSearchConfigurationTypeDef](./type_defs.md#vectorsearchconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGraphOutputTypeDef

```python
# DeleteGraphOutputTypeDef definition

class DeleteGraphOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: GraphStatusType,  # (1)
    statusReason: str,
    createTime: datetime,
    provisionedMemory: int,
    endpoint: str,
    publicConnectivity: bool,
    vectorSearchConfiguration: VectorSearchConfigurationTypeDef,  # (2)
    replicaCount: int,
    kmsKeyIdentifier: str,
    sourceSnapshotId: str,
    deletionProtection: bool,
    buildNumber: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: GraphStatusType](./literals.md#graphstatustype) 
2. See [:material-code-braces: VectorSearchConfigurationTypeDef](./type_defs.md#vectorsearchconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGraphOutputTypeDef

```python
# GetGraphOutputTypeDef definition

class GetGraphOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: GraphStatusType,  # (1)
    statusReason: str,
    createTime: datetime,
    provisionedMemory: int,
    endpoint: str,
    publicConnectivity: bool,
    vectorSearchConfiguration: VectorSearchConfigurationTypeDef,  # (2)
    replicaCount: int,
    kmsKeyIdentifier: str,
    sourceSnapshotId: str,
    deletionProtection: bool,
    buildNumber: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: GraphStatusType](./literals.md#graphstatustype) 
2. See [:material-code-braces: VectorSearchConfigurationTypeDef](./type_defs.md#vectorsearchconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetGraphOutputTypeDef

```python
# ResetGraphOutputTypeDef definition

class ResetGraphOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: GraphStatusType,  # (1)
    statusReason: str,
    createTime: datetime,
    provisionedMemory: int,
    endpoint: str,
    publicConnectivity: bool,
    vectorSearchConfiguration: VectorSearchConfigurationTypeDef,  # (2)
    replicaCount: int,
    kmsKeyIdentifier: str,
    sourceSnapshotId: str,
    deletionProtection: bool,
    buildNumber: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: GraphStatusType](./literals.md#graphstatustype) 
2. See [:material-code-braces: VectorSearchConfigurationTypeDef](./type_defs.md#vectorsearchconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreGraphFromSnapshotOutputTypeDef

```python
# RestoreGraphFromSnapshotOutputTypeDef definition

class RestoreGraphFromSnapshotOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: GraphStatusType,  # (1)
    statusReason: str,
    createTime: datetime,
    provisionedMemory: int,
    endpoint: str,
    publicConnectivity: bool,
    vectorSearchConfiguration: VectorSearchConfigurationTypeDef,  # (2)
    replicaCount: int,
    kmsKeyIdentifier: str,
    sourceSnapshotId: str,
    deletionProtection: bool,
    buildNumber: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: GraphStatusType](./literals.md#graphstatustype) 
2. See [:material-code-braces: VectorSearchConfigurationTypeDef](./type_defs.md#vectorsearchconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGraphOutputTypeDef

```python
# UpdateGraphOutputTypeDef definition

class UpdateGraphOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: GraphStatusType,  # (1)
    statusReason: str,
    createTime: datetime,
    provisionedMemory: int,
    endpoint: str,
    publicConnectivity: bool,
    vectorSearchConfiguration: VectorSearchConfigurationTypeDef,  # (2)
    replicaCount: int,
    kmsKeyIdentifier: str,
    sourceSnapshotId: str,
    deletionProtection: bool,
    buildNumber: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: GraphStatusType](./literals.md#graphstatustype) 
2. See [:material-code-braces: VectorSearchConfigurationTypeDef](./type_defs.md#vectorsearchconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGraphInputGraphAvailableWaitTypeDef

```python
# GetGraphInputGraphAvailableWaitTypeDef definition

class GetGraphInputGraphAvailableWaitTypeDef(TypedDict):
    graphIdentifier: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetGraphInputGraphDeletedWaitTypeDef

```python
# GetGraphInputGraphDeletedWaitTypeDef definition

class GetGraphInputGraphDeletedWaitTypeDef(TypedDict):
    graphIdentifier: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetGraphSnapshotInputGraphSnapshotAvailableWaitTypeDef

```python
# GetGraphSnapshotInputGraphSnapshotAvailableWaitTypeDef definition

class GetGraphSnapshotInputGraphSnapshotAvailableWaitTypeDef(TypedDict):
    snapshotIdentifier: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetGraphSnapshotInputGraphSnapshotDeletedWaitTypeDef

```python
# GetGraphSnapshotInputGraphSnapshotDeletedWaitTypeDef definition

class GetGraphSnapshotInputGraphSnapshotDeletedWaitTypeDef(TypedDict):
    snapshotIdentifier: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetImportTaskInputImportTaskCancelledWaitTypeDef

```python
# GetImportTaskInputImportTaskCancelledWaitTypeDef definition

class GetImportTaskInputImportTaskCancelledWaitTypeDef(TypedDict):
    taskIdentifier: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetImportTaskInputImportTaskSuccessfulWaitTypeDef

```python
# GetImportTaskInputImportTaskSuccessfulWaitTypeDef definition

class GetImportTaskInputImportTaskSuccessfulWaitTypeDef(TypedDict):
    taskIdentifier: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetPrivateGraphEndpointInputPrivateGraphEndpointAvailableWaitTypeDef

```python
# GetPrivateGraphEndpointInputPrivateGraphEndpointAvailableWaitTypeDef definition

class GetPrivateGraphEndpointInputPrivateGraphEndpointAvailableWaitTypeDef(TypedDict):
    graphIdentifier: str,
    vpcId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetPrivateGraphEndpointInputPrivateGraphEndpointDeletedWaitTypeDef

```python
# GetPrivateGraphEndpointInputPrivateGraphEndpointDeletedWaitTypeDef definition

class GetPrivateGraphEndpointInputPrivateGraphEndpointDeletedWaitTypeDef(TypedDict):
    graphIdentifier: str,
    vpcId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GraphDataSummaryTypeDef

```python
# GraphDataSummaryTypeDef definition

class GraphDataSummaryTypeDef(TypedDict):
    numNodes: NotRequired[int],
    numEdges: NotRequired[int],
    numNodeLabels: NotRequired[int],
    numEdgeLabels: NotRequired[int],
    nodeLabels: NotRequired[List[str]],
    edgeLabels: NotRequired[List[str]],
    numNodeProperties: NotRequired[int],
    numEdgeProperties: NotRequired[int],
    nodeProperties: NotRequired[List[Dict[str, int]]],
    edgeProperties: NotRequired[List[Dict[str, int]]],
    totalNodePropertyValues: NotRequired[int],
    totalEdgePropertyValues: NotRequired[int],
    nodeStructures: NotRequired[List[NodeStructureTypeDef]],  # (1)
    edgeStructures: NotRequired[List[EdgeStructureTypeDef]],  # (2)
```

1. See [:material-code-braces: NodeStructureTypeDef](./type_defs.md#nodestructuretypedef) 
2. See [:material-code-braces: EdgeStructureTypeDef](./type_defs.md#edgestructuretypedef) 
## ListGraphSnapshotsOutputTypeDef

```python
# ListGraphSnapshotsOutputTypeDef definition

class ListGraphSnapshotsOutputTypeDef(TypedDict):
    graphSnapshots: List[GraphSnapshotSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: GraphSnapshotSummaryTypeDef](./type_defs.md#graphsnapshotsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGraphsOutputTypeDef

```python
# ListGraphsOutputTypeDef definition

class ListGraphsOutputTypeDef(TypedDict):
    graphs: List[GraphSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: GraphSummaryTypeDef](./type_defs.md#graphsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportOptionsTypeDef

```python
# ImportOptionsTypeDef definition

class ImportOptionsTypeDef(TypedDict):
    neptune: NotRequired[NeptuneImportOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: NeptuneImportOptionsTypeDef](./type_defs.md#neptuneimportoptionstypedef) 
## ListImportTasksOutputTypeDef

```python
# ListImportTasksOutputTypeDef definition

class ListImportTasksOutputTypeDef(TypedDict):
    tasks: List[ImportTaskSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportTaskSummaryTypeDef](./type_defs.md#importtasksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGraphSnapshotsInputListGraphSnapshotsPaginateTypeDef

```python
# ListGraphSnapshotsInputListGraphSnapshotsPaginateTypeDef definition

class ListGraphSnapshotsInputListGraphSnapshotsPaginateTypeDef(TypedDict):
    graphIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGraphsInputListGraphsPaginateTypeDef

```python
# ListGraphsInputListGraphsPaginateTypeDef definition

class ListGraphsInputListGraphsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListImportTasksInputListImportTasksPaginateTypeDef

```python
# ListImportTasksInputListImportTasksPaginateTypeDef definition

class ListImportTasksInputListImportTasksPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrivateGraphEndpointsInputListPrivateGraphEndpointsPaginateTypeDef

```python
# ListPrivateGraphEndpointsInputListPrivateGraphEndpointsPaginateTypeDef definition

class ListPrivateGraphEndpointsInputListPrivateGraphEndpointsPaginateTypeDef(TypedDict):
    graphIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrivateGraphEndpointsOutputTypeDef

```python
# ListPrivateGraphEndpointsOutputTypeDef definition

class ListPrivateGraphEndpointsOutputTypeDef(TypedDict):
    privateGraphEndpoints: List[PrivateGraphEndpointSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PrivateGraphEndpointSummaryTypeDef](./type_defs.md#privategraphendpointsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueriesOutputTypeDef

```python
# ListQueriesOutputTypeDef definition

class ListQueriesOutputTypeDef(TypedDict):
    queries: List[QuerySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QuerySummaryTypeDef](./type_defs.md#querysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGraphSummaryOutputTypeDef

```python
# GetGraphSummaryOutputTypeDef definition

class GetGraphSummaryOutputTypeDef(TypedDict):
    version: str,
    lastStatisticsComputationTime: datetime,
    graphSummary: GraphDataSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GraphDataSummaryTypeDef](./type_defs.md#graphdatasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGraphUsingImportTaskInputRequestTypeDef

```python
# CreateGraphUsingImportTaskInputRequestTypeDef definition

class CreateGraphUsingImportTaskInputRequestTypeDef(TypedDict):
    graphName: str,
    source: str,
    roleArn: str,
    tags: NotRequired[Mapping[str, str]],
    publicConnectivity: NotRequired[bool],
    kmsKeyIdentifier: NotRequired[str],
    vectorSearchConfiguration: NotRequired[VectorSearchConfigurationTypeDef],  # (1)
    replicaCount: NotRequired[int],
    deletionProtection: NotRequired[bool],
    importOptions: NotRequired[ImportOptionsTypeDef],  # (2)
    maxProvisionedMemory: NotRequired[int],
    minProvisionedMemory: NotRequired[int],
    failOnError: NotRequired[bool],
    format: NotRequired[FormatType],  # (3)
    blankNodeHandling: NotRequired[BlankNodeHandlingType],  # (4)
```

1. See [:material-code-braces: VectorSearchConfigurationTypeDef](./type_defs.md#vectorsearchconfigurationtypedef) 
2. See [:material-code-braces: ImportOptionsTypeDef](./type_defs.md#importoptionstypedef) 
3. See [:material-code-brackets: FormatType](./literals.md#formattype) 
4. See [:material-code-brackets: BlankNodeHandlingType](./literals.md#blanknodehandlingtype) 
## CreateGraphUsingImportTaskOutputTypeDef

```python
# CreateGraphUsingImportTaskOutputTypeDef definition

class CreateGraphUsingImportTaskOutputTypeDef(TypedDict):
    graphId: str,
    taskId: str,
    source: str,
    format: FormatType,  # (1)
    roleArn: str,
    status: ImportTaskStatusType,  # (2)
    importOptions: ImportOptionsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
2. See [:material-code-brackets: ImportTaskStatusType](./literals.md#importtaskstatustype) 
3. See [:material-code-braces: ImportOptionsTypeDef](./type_defs.md#importoptionstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetImportTaskOutputTypeDef

```python
# GetImportTaskOutputTypeDef definition

class GetImportTaskOutputTypeDef(TypedDict):
    graphId: str,
    taskId: str,
    source: str,
    format: FormatType,  # (1)
    roleArn: str,
    status: ImportTaskStatusType,  # (2)
    importOptions: ImportOptionsTypeDef,  # (3)
    importTaskDetails: ImportTaskDetailsTypeDef,  # (4)
    attemptNumber: int,
    statusReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
2. See [:material-code-brackets: ImportTaskStatusType](./literals.md#importtaskstatustype) 
3. See [:material-code-braces: ImportOptionsTypeDef](./type_defs.md#importoptionstypedef) 
4. See [:material-code-braces: ImportTaskDetailsTypeDef](./type_defs.md#importtaskdetailstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartImportTaskInputRequestTypeDef

```python
# StartImportTaskInputRequestTypeDef definition

class StartImportTaskInputRequestTypeDef(TypedDict):
    source: str,
    graphIdentifier: str,
    roleArn: str,
    importOptions: NotRequired[ImportOptionsTypeDef],  # (1)
    failOnError: NotRequired[bool],
    format: NotRequired[FormatType],  # (2)
    blankNodeHandling: NotRequired[BlankNodeHandlingType],  # (3)
```

1. See [:material-code-braces: ImportOptionsTypeDef](./type_defs.md#importoptionstypedef) 
2. See [:material-code-brackets: FormatType](./literals.md#formattype) 
3. See [:material-code-brackets: BlankNodeHandlingType](./literals.md#blanknodehandlingtype) 
## StartImportTaskOutputTypeDef

```python
# StartImportTaskOutputTypeDef definition

class StartImportTaskOutputTypeDef(TypedDict):
    graphId: str,
    taskId: str,
    source: str,
    format: FormatType,  # (1)
    roleArn: str,
    status: ImportTaskStatusType,  # (2)
    importOptions: ImportOptionsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
2. See [:material-code-brackets: ImportTaskStatusType](./literals.md#importtaskstatustype) 
3. See [:material-code-braces: ImportOptionsTypeDef](./type_defs.md#importoptionstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
