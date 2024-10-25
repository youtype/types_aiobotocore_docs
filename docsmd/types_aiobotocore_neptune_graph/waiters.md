# Waiters

> [Index](../README.md) > [NeptuneGraph](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [NeptuneGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph)
    type annotations stubs module [types-aiobotocore-neptune-graph](https://pypi.org/project/types-aiobotocore-neptune-graph/).

## GraphAvailableWaiter

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_waiter("graph_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Waiter.GraphAvailable)

```python
# GraphAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_neptune_graph.waiter import GraphAvailableWaiter

session = get_session()
async with session.create_client("neptune-graph") as client:  # (1)
    waiter: GraphAvailableWaiter = client.get_waiter("graph_available")  # (2)
    await waiter.wait()
```

1. client: [NeptuneGraphClient](./client.md)
2. waiter: [GraphAvailableWaiter](./waiters.md#graphavailablewaiter)


### wait

Type annotations and code completion for `#!python GraphAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    graphIdentifier: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetGraphInputGraphAvailableWaitTypeDef = {  # (1)
    "graphIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetGraphInputGraphAvailableWaitTypeDef](./type_defs.md#getgraphinputgraphavailablewaittypedef) 
## GraphDeletedWaiter

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_waiter("graph_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Waiter.GraphDeleted)

```python
# GraphDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_neptune_graph.waiter import GraphDeletedWaiter

session = get_session()
async with session.create_client("neptune-graph") as client:  # (1)
    waiter: GraphDeletedWaiter = client.get_waiter("graph_deleted")  # (2)
    await waiter.wait()
```

1. client: [NeptuneGraphClient](./client.md)
2. waiter: [GraphDeletedWaiter](./waiters.md#graphdeletedwaiter)


### wait

Type annotations and code completion for `#!python GraphDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    graphIdentifier: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetGraphInputGraphDeletedWaitTypeDef = {  # (1)
    "graphIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetGraphInputGraphDeletedWaitTypeDef](./type_defs.md#getgraphinputgraphdeletedwaittypedef) 
## GraphSnapshotAvailableWaiter

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_waiter("graph_snapshot_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Waiter.GraphSnapshotAvailable)

```python
# GraphSnapshotAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_neptune_graph.waiter import GraphSnapshotAvailableWaiter

session = get_session()
async with session.create_client("neptune-graph") as client:  # (1)
    waiter: GraphSnapshotAvailableWaiter = client.get_waiter("graph_snapshot_available")  # (2)
    await waiter.wait()
```

1. client: [NeptuneGraphClient](./client.md)
2. waiter: [GraphSnapshotAvailableWaiter](./waiters.md#graphsnapshotavailablewaiter)


### wait

Type annotations and code completion for `#!python GraphSnapshotAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    snapshotIdentifier: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetGraphSnapshotInputGraphSnapshotAvailableWaitTypeDef = {  # (1)
    "snapshotIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetGraphSnapshotInputGraphSnapshotAvailableWaitTypeDef](./type_defs.md#getgraphsnapshotinputgraphsnapshotavailablewaittypedef) 
## GraphSnapshotDeletedWaiter

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_waiter("graph_snapshot_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Waiter.GraphSnapshotDeleted)

```python
# GraphSnapshotDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_neptune_graph.waiter import GraphSnapshotDeletedWaiter

session = get_session()
async with session.create_client("neptune-graph") as client:  # (1)
    waiter: GraphSnapshotDeletedWaiter = client.get_waiter("graph_snapshot_deleted")  # (2)
    await waiter.wait()
```

1. client: [NeptuneGraphClient](./client.md)
2. waiter: [GraphSnapshotDeletedWaiter](./waiters.md#graphsnapshotdeletedwaiter)


### wait

Type annotations and code completion for `#!python GraphSnapshotDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    snapshotIdentifier: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetGraphSnapshotInputGraphSnapshotDeletedWaitTypeDef = {  # (1)
    "snapshotIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetGraphSnapshotInputGraphSnapshotDeletedWaitTypeDef](./type_defs.md#getgraphsnapshotinputgraphsnapshotdeletedwaittypedef) 
## ImportTaskCancelledWaiter

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_waiter("import_task_cancelled")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Waiter.ImportTaskCancelled)

```python
# ImportTaskCancelledWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_neptune_graph.waiter import ImportTaskCancelledWaiter

session = get_session()
async with session.create_client("neptune-graph") as client:  # (1)
    waiter: ImportTaskCancelledWaiter = client.get_waiter("import_task_cancelled")  # (2)
    await waiter.wait()
```

1. client: [NeptuneGraphClient](./client.md)
2. waiter: [ImportTaskCancelledWaiter](./waiters.md#importtaskcancelledwaiter)


### wait

Type annotations and code completion for `#!python ImportTaskCancelledWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    taskIdentifier: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetImportTaskInputImportTaskCancelledWaitTypeDef = {  # (1)
    "taskIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetImportTaskInputImportTaskCancelledWaitTypeDef](./type_defs.md#getimporttaskinputimporttaskcancelledwaittypedef) 
## ImportTaskSuccessfulWaiter

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_waiter("import_task_successful")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Waiter.ImportTaskSuccessful)

```python
# ImportTaskSuccessfulWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_neptune_graph.waiter import ImportTaskSuccessfulWaiter

session = get_session()
async with session.create_client("neptune-graph") as client:  # (1)
    waiter: ImportTaskSuccessfulWaiter = client.get_waiter("import_task_successful")  # (2)
    await waiter.wait()
```

1. client: [NeptuneGraphClient](./client.md)
2. waiter: [ImportTaskSuccessfulWaiter](./waiters.md#importtasksuccessfulwaiter)


### wait

Type annotations and code completion for `#!python ImportTaskSuccessfulWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    taskIdentifier: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetImportTaskInputImportTaskSuccessfulWaitTypeDef = {  # (1)
    "taskIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetImportTaskInputImportTaskSuccessfulWaitTypeDef](./type_defs.md#getimporttaskinputimporttasksuccessfulwaittypedef) 
## PrivateGraphEndpointAvailableWaiter

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_waiter("private_graph_endpoint_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Waiter.PrivateGraphEndpointAvailable)

```python
# PrivateGraphEndpointAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_neptune_graph.waiter import PrivateGraphEndpointAvailableWaiter

session = get_session()
async with session.create_client("neptune-graph") as client:  # (1)
    waiter: PrivateGraphEndpointAvailableWaiter = client.get_waiter("private_graph_endpoint_available")  # (2)
    await waiter.wait()
```

1. client: [NeptuneGraphClient](./client.md)
2. waiter: [PrivateGraphEndpointAvailableWaiter](./waiters.md#privategraphendpointavailablewaiter)


### wait

Type annotations and code completion for `#!python PrivateGraphEndpointAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    graphIdentifier: str,
    vpcId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetPrivateGraphEndpointInputPrivateGraphEndpointAvailableWaitTypeDef = {  # (1)
    "graphIdentifier": ...,
    "vpcId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetPrivateGraphEndpointInputPrivateGraphEndpointAvailableWaitTypeDef](./type_defs.md#getprivategraphendpointinputprivategraphendpointavailablewaittypedef) 
## PrivateGraphEndpointDeletedWaiter

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_waiter("private_graph_endpoint_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Waiter.PrivateGraphEndpointDeleted)

```python
# PrivateGraphEndpointDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_neptune_graph.waiter import PrivateGraphEndpointDeletedWaiter

session = get_session()
async with session.create_client("neptune-graph") as client:  # (1)
    waiter: PrivateGraphEndpointDeletedWaiter = client.get_waiter("private_graph_endpoint_deleted")  # (2)
    await waiter.wait()
```

1. client: [NeptuneGraphClient](./client.md)
2. waiter: [PrivateGraphEndpointDeletedWaiter](./waiters.md#privategraphendpointdeletedwaiter)


### wait

Type annotations and code completion for `#!python PrivateGraphEndpointDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    graphIdentifier: str,
    vpcId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetPrivateGraphEndpointInputPrivateGraphEndpointDeletedWaitTypeDef = {  # (1)
    "graphIdentifier": ...,
    "vpcId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetPrivateGraphEndpointInputPrivateGraphEndpointDeletedWaitTypeDef](./type_defs.md#getprivategraphendpointinputprivategraphendpointdeletedwaittypedef) 
