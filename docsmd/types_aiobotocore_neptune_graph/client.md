# NeptuneGraphClient

> [Index](../README.md) > [NeptuneGraph](./README.md) > NeptuneGraphClient

!!! note ""

    Auto-generated documentation for [NeptuneGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph)
    type annotations stubs module [types-aiobotocore-neptune-graph](https://pypi.org/project/types-aiobotocore-neptune-graph/).

## NeptuneGraphClient

Type annotations and code completion for `#!python session.create_client("neptune-graph")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client)

```python
# NeptuneGraphClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_neptune_graph.client import NeptuneGraphClient

session = get_session()
async with session.create_client("neptune-graph") as client:
    client: NeptuneGraphClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("neptune-graph").exceptions` structure.

```python
# NeptuneGraphClient.exceptions usage example

async with session.create_client("neptune-graph") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.UnprocessableException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# NeptuneGraphClient usage type checking example

from types_aiobotocore_neptune_graph.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("neptune-graph").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_import\_task

Deletes the specified import task.

Type annotations and code completion for `#!python session.create_client("neptune-graph").cancel_import_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.cancel_import_task)

```python
# cancel_import_task method definition

await def cancel_import_task(
    self,
    *,
    taskIdentifier: str,
) -> CancelImportTaskOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelImportTaskOutputTypeDef](./type_defs.md#cancelimporttaskoutputtypedef) 


```python
# cancel_import_task method usage example with argument unpacking

kwargs: CancelImportTaskInputRequestTypeDef = {  # (1)
    "taskIdentifier": ...,
}

parent.cancel_import_task(**kwargs)
```

1. See [:material-code-braces: CancelImportTaskInputRequestTypeDef](./type_defs.md#cancelimporttaskinputrequesttypedef) 

### cancel\_query

Cancels a specified query.

Type annotations and code completion for `#!python session.create_client("neptune-graph").cancel_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.cancel_query)

```python
# cancel_query method definition

await def cancel_query(
    self,
    *,
    graphIdentifier: str,
    queryId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# cancel_query method usage example with argument unpacking

kwargs: CancelQueryInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
    "queryId": ...,
}

parent.cancel_query(**kwargs)
```

1. See [:material-code-braces: CancelQueryInputRequestTypeDef](./type_defs.md#cancelqueryinputrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("neptune-graph").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_graph

Creates a new Neptune Analytics graph.

Type annotations and code completion for `#!python session.create_client("neptune-graph").create_graph` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.create_graph)

```python
# create_graph method definition

await def create_graph(
    self,
    *,
    graphName: str,
    provisionedMemory: int,
    tags: Mapping[str, str] = ...,
    publicConnectivity: bool = ...,
    kmsKeyIdentifier: str = ...,
    vectorSearchConfiguration: VectorSearchConfigurationTypeDef = ...,  # (1)
    replicaCount: int = ...,
    deletionProtection: bool = ...,
) -> CreateGraphOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VectorSearchConfigurationTypeDef](./type_defs.md#vectorsearchconfigurationtypedef) 
2. See [:material-code-braces: CreateGraphOutputTypeDef](./type_defs.md#creategraphoutputtypedef) 


```python
# create_graph method usage example with argument unpacking

kwargs: CreateGraphInputRequestTypeDef = {  # (1)
    "graphName": ...,
    "provisionedMemory": ...,
}

parent.create_graph(**kwargs)
```

1. See [:material-code-braces: CreateGraphInputRequestTypeDef](./type_defs.md#creategraphinputrequesttypedef) 

### create\_graph\_snapshot

Creates a snapshot of the specific graph.

Type annotations and code completion for `#!python session.create_client("neptune-graph").create_graph_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.create_graph_snapshot)

```python
# create_graph_snapshot method definition

await def create_graph_snapshot(
    self,
    *,
    graphIdentifier: str,
    snapshotName: str,
    tags: Mapping[str, str] = ...,
) -> CreateGraphSnapshotOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateGraphSnapshotOutputTypeDef](./type_defs.md#creategraphsnapshotoutputtypedef) 


```python
# create_graph_snapshot method usage example with argument unpacking

kwargs: CreateGraphSnapshotInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
    "snapshotName": ...,
}

parent.create_graph_snapshot(**kwargs)
```

1. See [:material-code-braces: CreateGraphSnapshotInputRequestTypeDef](./type_defs.md#creategraphsnapshotinputrequesttypedef) 

### create\_graph\_using\_import\_task

Creates a new Neptune Analytics graph and imports data into it, either from
Amazon Simple Storage Service (S3) or from a Neptune database or a Neptune
database
snapshot.

Type annotations and code completion for `#!python session.create_client("neptune-graph").create_graph_using_import_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.create_graph_using_import_task)

```python
# create_graph_using_import_task method definition

await def create_graph_using_import_task(
    self,
    *,
    graphName: str,
    source: str,
    roleArn: str,
    tags: Mapping[str, str] = ...,
    publicConnectivity: bool = ...,
    kmsKeyIdentifier: str = ...,
    vectorSearchConfiguration: VectorSearchConfigurationTypeDef = ...,  # (1)
    replicaCount: int = ...,
    deletionProtection: bool = ...,
    importOptions: ImportOptionsTypeDef = ...,  # (2)
    maxProvisionedMemory: int = ...,
    minProvisionedMemory: int = ...,
    failOnError: bool = ...,
    format: FormatType = ...,  # (3)
    blankNodeHandling: BlankNodeHandlingType = ...,  # (4)
) -> CreateGraphUsingImportTaskOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: VectorSearchConfigurationTypeDef](./type_defs.md#vectorsearchconfigurationtypedef) 
2. See [:material-code-braces: ImportOptionsTypeDef](./type_defs.md#importoptionstypedef) 
3. See [:material-code-brackets: FormatType](./literals.md#formattype) 
4. See [:material-code-brackets: BlankNodeHandlingType](./literals.md#blanknodehandlingtype) 
5. See [:material-code-braces: CreateGraphUsingImportTaskOutputTypeDef](./type_defs.md#creategraphusingimporttaskoutputtypedef) 


```python
# create_graph_using_import_task method usage example with argument unpacking

kwargs: CreateGraphUsingImportTaskInputRequestTypeDef = {  # (1)
    "graphName": ...,
    "source": ...,
    "roleArn": ...,
}

parent.create_graph_using_import_task(**kwargs)
```

1. See [:material-code-braces: CreateGraphUsingImportTaskInputRequestTypeDef](./type_defs.md#creategraphusingimporttaskinputrequesttypedef) 

### create\_private\_graph\_endpoint

Create a private graph endpoint to allow private access from to the graph from
within a
VPC.

Type annotations and code completion for `#!python session.create_client("neptune-graph").create_private_graph_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.create_private_graph_endpoint)

```python
# create_private_graph_endpoint method definition

await def create_private_graph_endpoint(
    self,
    *,
    graphIdentifier: str,
    vpcId: str = ...,
    subnetIds: Sequence[str] = ...,
    vpcSecurityGroupIds: Sequence[str] = ...,
) -> CreatePrivateGraphEndpointOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePrivateGraphEndpointOutputTypeDef](./type_defs.md#createprivategraphendpointoutputtypedef) 


```python
# create_private_graph_endpoint method usage example with argument unpacking

kwargs: CreatePrivateGraphEndpointInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
}

parent.create_private_graph_endpoint(**kwargs)
```

1. See [:material-code-braces: CreatePrivateGraphEndpointInputRequestTypeDef](./type_defs.md#createprivategraphendpointinputrequesttypedef) 

### delete\_graph

Deletes the specified graph.

Type annotations and code completion for `#!python session.create_client("neptune-graph").delete_graph` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.delete_graph)

```python
# delete_graph method definition

await def delete_graph(
    self,
    *,
    graphIdentifier: str,
    skipSnapshot: bool,
) -> DeleteGraphOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteGraphOutputTypeDef](./type_defs.md#deletegraphoutputtypedef) 


```python
# delete_graph method usage example with argument unpacking

kwargs: DeleteGraphInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
    "skipSnapshot": ...,
}

parent.delete_graph(**kwargs)
```

1. See [:material-code-braces: DeleteGraphInputRequestTypeDef](./type_defs.md#deletegraphinputrequesttypedef) 

### delete\_graph\_snapshot

Deletes the specifed graph snapshot.

Type annotations and code completion for `#!python session.create_client("neptune-graph").delete_graph_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.delete_graph_snapshot)

```python
# delete_graph_snapshot method definition

await def delete_graph_snapshot(
    self,
    *,
    snapshotIdentifier: str,
) -> DeleteGraphSnapshotOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteGraphSnapshotOutputTypeDef](./type_defs.md#deletegraphsnapshotoutputtypedef) 


```python
# delete_graph_snapshot method usage example with argument unpacking

kwargs: DeleteGraphSnapshotInputRequestTypeDef = {  # (1)
    "snapshotIdentifier": ...,
}

parent.delete_graph_snapshot(**kwargs)
```

1. See [:material-code-braces: DeleteGraphSnapshotInputRequestTypeDef](./type_defs.md#deletegraphsnapshotinputrequesttypedef) 

### delete\_private\_graph\_endpoint

Deletes a private graph endpoint.

Type annotations and code completion for `#!python session.create_client("neptune-graph").delete_private_graph_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.delete_private_graph_endpoint)

```python
# delete_private_graph_endpoint method definition

await def delete_private_graph_endpoint(
    self,
    *,
    graphIdentifier: str,
    vpcId: str,
) -> DeletePrivateGraphEndpointOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePrivateGraphEndpointOutputTypeDef](./type_defs.md#deleteprivategraphendpointoutputtypedef) 


```python
# delete_private_graph_endpoint method usage example with argument unpacking

kwargs: DeletePrivateGraphEndpointInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
    "vpcId": ...,
}

parent.delete_private_graph_endpoint(**kwargs)
```

1. See [:material-code-braces: DeletePrivateGraphEndpointInputRequestTypeDef](./type_defs.md#deleteprivategraphendpointinputrequesttypedef) 

### execute\_query

Execute an openCypher query.

Type annotations and code completion for `#!python session.create_client("neptune-graph").execute_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.execute_query)

```python
# execute_query method definition

await def execute_query(
    self,
    *,
    graphIdentifier: str,
    queryString: str,
    language: QueryLanguageType,  # (1)
    parameters: Mapping[str, Mapping[str, Any]] = ...,
    planCache: PlanCacheTypeType = ...,  # (2)
    explainMode: ExplainModeType = ...,  # (3)
    queryTimeoutMilliseconds: int = ...,
) -> ExecuteQueryOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: QueryLanguageType](./literals.md#querylanguagetype) 
2. See [:material-code-brackets: PlanCacheTypeType](./literals.md#plancachetypetype) 
3. See [:material-code-brackets: ExplainModeType](./literals.md#explainmodetype) 
4. See [:material-code-braces: ExecuteQueryOutputTypeDef](./type_defs.md#executequeryoutputtypedef) 


```python
# execute_query method usage example with argument unpacking

kwargs: ExecuteQueryInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
    "queryString": ...,
    "language": ...,
}

parent.execute_query(**kwargs)
```

1. See [:material-code-braces: ExecuteQueryInputRequestTypeDef](./type_defs.md#executequeryinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("neptune-graph").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_graph

Gets information about a specified graph.

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_graph` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.get_graph)

```python
# get_graph method definition

await def get_graph(
    self,
    *,
    graphIdentifier: str,
) -> GetGraphOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGraphOutputTypeDef](./type_defs.md#getgraphoutputtypedef) 


```python
# get_graph method usage example with argument unpacking

kwargs: GetGraphInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
}

parent.get_graph(**kwargs)
```

1. See [:material-code-braces: GetGraphInputRequestTypeDef](./type_defs.md#getgraphinputrequesttypedef) 

### get\_graph\_snapshot

Retrieves a specified graph snapshot.

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_graph_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.get_graph_snapshot)

```python
# get_graph_snapshot method definition

await def get_graph_snapshot(
    self,
    *,
    snapshotIdentifier: str,
) -> GetGraphSnapshotOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGraphSnapshotOutputTypeDef](./type_defs.md#getgraphsnapshotoutputtypedef) 


```python
# get_graph_snapshot method usage example with argument unpacking

kwargs: GetGraphSnapshotInputRequestTypeDef = {  # (1)
    "snapshotIdentifier": ...,
}

parent.get_graph_snapshot(**kwargs)
```

1. See [:material-code-braces: GetGraphSnapshotInputRequestTypeDef](./type_defs.md#getgraphsnapshotinputrequesttypedef) 

### get\_graph\_summary

Gets a graph summary for a property graph.

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_graph_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.get_graph_summary)

```python
# get_graph_summary method definition

await def get_graph_summary(
    self,
    *,
    graphIdentifier: str,
    mode: GraphSummaryModeType = ...,  # (1)
) -> GetGraphSummaryOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GraphSummaryModeType](./literals.md#graphsummarymodetype) 
2. See [:material-code-braces: GetGraphSummaryOutputTypeDef](./type_defs.md#getgraphsummaryoutputtypedef) 


```python
# get_graph_summary method usage example with argument unpacking

kwargs: GetGraphSummaryInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
}

parent.get_graph_summary(**kwargs)
```

1. See [:material-code-braces: GetGraphSummaryInputRequestTypeDef](./type_defs.md#getgraphsummaryinputrequesttypedef) 

### get\_import\_task

Retrieves a specified import task.

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_import_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.get_import_task)

```python
# get_import_task method definition

await def get_import_task(
    self,
    *,
    taskIdentifier: str,
) -> GetImportTaskOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetImportTaskOutputTypeDef](./type_defs.md#getimporttaskoutputtypedef) 


```python
# get_import_task method usage example with argument unpacking

kwargs: GetImportTaskInputRequestTypeDef = {  # (1)
    "taskIdentifier": ...,
}

parent.get_import_task(**kwargs)
```

1. See [:material-code-braces: GetImportTaskInputRequestTypeDef](./type_defs.md#getimporttaskinputrequesttypedef) 

### get\_private\_graph\_endpoint

Retrieves information about a specified private endpoint.

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_private_graph_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.get_private_graph_endpoint)

```python
# get_private_graph_endpoint method definition

await def get_private_graph_endpoint(
    self,
    *,
    graphIdentifier: str,
    vpcId: str,
) -> GetPrivateGraphEndpointOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPrivateGraphEndpointOutputTypeDef](./type_defs.md#getprivategraphendpointoutputtypedef) 


```python
# get_private_graph_endpoint method usage example with argument unpacking

kwargs: GetPrivateGraphEndpointInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
    "vpcId": ...,
}

parent.get_private_graph_endpoint(**kwargs)
```

1. See [:material-code-braces: GetPrivateGraphEndpointInputRequestTypeDef](./type_defs.md#getprivategraphendpointinputrequesttypedef) 

### get\_query

Retrieves the status of a specified query.

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.get_query)

```python
# get_query method definition

await def get_query(
    self,
    *,
    graphIdentifier: str,
    queryId: str,
) -> GetQueryOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueryOutputTypeDef](./type_defs.md#getqueryoutputtypedef) 


```python
# get_query method usage example with argument unpacking

kwargs: GetQueryInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
    "queryId": ...,
}

parent.get_query(**kwargs)
```

1. See [:material-code-braces: GetQueryInputRequestTypeDef](./type_defs.md#getqueryinputrequesttypedef) 

### list\_graph\_snapshots

Lists available snapshots of a specified Neptune Analytics graph.

Type annotations and code completion for `#!python session.create_client("neptune-graph").list_graph_snapshots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.list_graph_snapshots)

```python
# list_graph_snapshots method definition

await def list_graph_snapshots(
    self,
    *,
    graphIdentifier: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListGraphSnapshotsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGraphSnapshotsOutputTypeDef](./type_defs.md#listgraphsnapshotsoutputtypedef) 


```python
# list_graph_snapshots method usage example with argument unpacking

kwargs: ListGraphSnapshotsInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
}

parent.list_graph_snapshots(**kwargs)
```

1. See [:material-code-braces: ListGraphSnapshotsInputRequestTypeDef](./type_defs.md#listgraphsnapshotsinputrequesttypedef) 

### list\_graphs

Lists available Neptune Analytics graphs.

Type annotations and code completion for `#!python session.create_client("neptune-graph").list_graphs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.list_graphs)

```python
# list_graphs method definition

await def list_graphs(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListGraphsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGraphsOutputTypeDef](./type_defs.md#listgraphsoutputtypedef) 


```python
# list_graphs method usage example with argument unpacking

kwargs: ListGraphsInputRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_graphs(**kwargs)
```

1. See [:material-code-braces: ListGraphsInputRequestTypeDef](./type_defs.md#listgraphsinputrequesttypedef) 

### list\_import\_tasks

Lists import tasks.

Type annotations and code completion for `#!python session.create_client("neptune-graph").list_import_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.list_import_tasks)

```python
# list_import_tasks method definition

await def list_import_tasks(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListImportTasksOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListImportTasksOutputTypeDef](./type_defs.md#listimporttasksoutputtypedef) 


```python
# list_import_tasks method usage example with argument unpacking

kwargs: ListImportTasksInputRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_import_tasks(**kwargs)
```

1. See [:material-code-braces: ListImportTasksInputRequestTypeDef](./type_defs.md#listimporttasksinputrequesttypedef) 

### list\_private\_graph\_endpoints

Lists private endpoints for a specified Neptune Analytics graph.

Type annotations and code completion for `#!python session.create_client("neptune-graph").list_private_graph_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.list_private_graph_endpoints)

```python
# list_private_graph_endpoints method definition

await def list_private_graph_endpoints(
    self,
    *,
    graphIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPrivateGraphEndpointsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPrivateGraphEndpointsOutputTypeDef](./type_defs.md#listprivategraphendpointsoutputtypedef) 


```python
# list_private_graph_endpoints method usage example with argument unpacking

kwargs: ListPrivateGraphEndpointsInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
}

parent.list_private_graph_endpoints(**kwargs)
```

1. See [:material-code-braces: ListPrivateGraphEndpointsInputRequestTypeDef](./type_defs.md#listprivategraphendpointsinputrequesttypedef) 

### list\_queries

Lists active openCypher queries.

Type annotations and code completion for `#!python session.create_client("neptune-graph").list_queries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.list_queries)

```python
# list_queries method definition

await def list_queries(
    self,
    *,
    graphIdentifier: str,
    maxResults: int,
    state: QueryStateInputType = ...,  # (1)
) -> ListQueriesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueryStateInputType](./literals.md#querystateinputtype) 
2. See [:material-code-braces: ListQueriesOutputTypeDef](./type_defs.md#listqueriesoutputtypedef) 


```python
# list_queries method usage example with argument unpacking

kwargs: ListQueriesInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
    "maxResults": ...,
}

parent.list_queries(**kwargs)
```

1. See [:material-code-braces: ListQueriesInputRequestTypeDef](./type_defs.md#listqueriesinputrequesttypedef) 

### list\_tags\_for\_resource

Lists tags associated with a specified resource.

Type annotations and code completion for `#!python session.create_client("neptune-graph").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### reset\_graph

Empties the data from a specified Neptune Analytics graph.

Type annotations and code completion for `#!python session.create_client("neptune-graph").reset_graph` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.reset_graph)

```python
# reset_graph method definition

await def reset_graph(
    self,
    *,
    graphIdentifier: str,
    skipSnapshot: bool,
) -> ResetGraphOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResetGraphOutputTypeDef](./type_defs.md#resetgraphoutputtypedef) 


```python
# reset_graph method usage example with argument unpacking

kwargs: ResetGraphInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
    "skipSnapshot": ...,
}

parent.reset_graph(**kwargs)
```

1. See [:material-code-braces: ResetGraphInputRequestTypeDef](./type_defs.md#resetgraphinputrequesttypedef) 

### restore\_graph\_from\_snapshot

Restores a graph from a snapshot.

Type annotations and code completion for `#!python session.create_client("neptune-graph").restore_graph_from_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.restore_graph_from_snapshot)

```python
# restore_graph_from_snapshot method definition

await def restore_graph_from_snapshot(
    self,
    *,
    snapshotIdentifier: str,
    graphName: str,
    provisionedMemory: int = ...,
    deletionProtection: bool = ...,
    tags: Mapping[str, str] = ...,
    replicaCount: int = ...,
    publicConnectivity: bool = ...,
) -> RestoreGraphFromSnapshotOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RestoreGraphFromSnapshotOutputTypeDef](./type_defs.md#restoregraphfromsnapshotoutputtypedef) 


```python
# restore_graph_from_snapshot method usage example with argument unpacking

kwargs: RestoreGraphFromSnapshotInputRequestTypeDef = {  # (1)
    "snapshotIdentifier": ...,
    "graphName": ...,
}

parent.restore_graph_from_snapshot(**kwargs)
```

1. See [:material-code-braces: RestoreGraphFromSnapshotInputRequestTypeDef](./type_defs.md#restoregraphfromsnapshotinputrequesttypedef) 

### start\_import\_task

Import data into existing Neptune Analytics graph from Amazon Simple Storage
Service
(S3).

Type annotations and code completion for `#!python session.create_client("neptune-graph").start_import_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.start_import_task)

```python
# start_import_task method definition

await def start_import_task(
    self,
    *,
    source: str,
    graphIdentifier: str,
    roleArn: str,
    importOptions: ImportOptionsTypeDef = ...,  # (1)
    failOnError: bool = ...,
    format: FormatType = ...,  # (2)
    blankNodeHandling: BlankNodeHandlingType = ...,  # (3)
) -> StartImportTaskOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ImportOptionsTypeDef](./type_defs.md#importoptionstypedef) 
2. See [:material-code-brackets: FormatType](./literals.md#formattype) 
3. See [:material-code-brackets: BlankNodeHandlingType](./literals.md#blanknodehandlingtype) 
4. See [:material-code-braces: StartImportTaskOutputTypeDef](./type_defs.md#startimporttaskoutputtypedef) 


```python
# start_import_task method usage example with argument unpacking

kwargs: StartImportTaskInputRequestTypeDef = {  # (1)
    "source": ...,
    "graphIdentifier": ...,
    "roleArn": ...,
}

parent.start_import_task(**kwargs)
```

1. See [:material-code-braces: StartImportTaskInputRequestTypeDef](./type_defs.md#startimporttaskinputrequesttypedef) 

### tag\_resource

Adds tags to the specified resource.

Type annotations and code completion for `#!python session.create_client("neptune-graph").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Removes the specified tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("neptune-graph").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_graph

Updates the configuration of a specified Neptune Analytics graph See also: [AWS
API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/neptune-graph-2023-11-29/UpdateGraph).

Type annotations and code completion for `#!python session.create_client("neptune-graph").update_graph` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.update_graph)

```python
# update_graph method definition

await def update_graph(
    self,
    *,
    graphIdentifier: str,
    publicConnectivity: bool = ...,
    provisionedMemory: int = ...,
    deletionProtection: bool = ...,
) -> UpdateGraphOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateGraphOutputTypeDef](./type_defs.md#updategraphoutputtypedef) 


```python
# update_graph method usage example with argument unpacking

kwargs: UpdateGraphInputRequestTypeDef = {  # (1)
    "graphIdentifier": ...,
}

parent.update_graph(**kwargs)
```

1. See [:material-code-braces: UpdateGraphInputRequestTypeDef](./type_defs.md#updategraphinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("neptune-graph").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "NeptuneGraphClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("neptune-graph").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_paginator` method with overloads.

- `client.get_paginator("list_graph_snapshots")` -> [ListGraphSnapshotsPaginator](./paginators.md#listgraphsnapshotspaginator)
- `client.get_paginator("list_graphs")` -> [ListGraphsPaginator](./paginators.md#listgraphspaginator)
- `client.get_paginator("list_import_tasks")` -> [ListImportTasksPaginator](./paginators.md#listimporttaskspaginator)
- `client.get_paginator("list_private_graph_endpoints")` -> [ListPrivateGraphEndpointsPaginator](./paginators.md#listprivategraphendpointspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_waiter` method with overloads.

- `client.get_waiter("graph_available")` -> [GraphAvailableWaiter](./waiters.md#graphavailablewaiter)
- `client.get_waiter("graph_deleted")` -> [GraphDeletedWaiter](./waiters.md#graphdeletedwaiter)
- `client.get_waiter("graph_snapshot_available")` -> [GraphSnapshotAvailableWaiter](./waiters.md#graphsnapshotavailablewaiter)
- `client.get_waiter("graph_snapshot_deleted")` -> [GraphSnapshotDeletedWaiter](./waiters.md#graphsnapshotdeletedwaiter)
- `client.get_waiter("import_task_cancelled")` -> [ImportTaskCancelledWaiter](./waiters.md#importtaskcancelledwaiter)
- `client.get_waiter("import_task_successful")` -> [ImportTaskSuccessfulWaiter](./waiters.md#importtasksuccessfulwaiter)
- `client.get_waiter("private_graph_endpoint_available")` -> [PrivateGraphEndpointAvailableWaiter](./waiters.md#privategraphendpointavailablewaiter)
- `client.get_waiter("private_graph_endpoint_deleted")` -> [PrivateGraphEndpointDeletedWaiter](./waiters.md#privategraphendpointdeletedwaiter)

