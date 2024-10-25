# ParallelComputingServiceClient

> [Index](../README.md) > [ParallelComputingService](./README.md) > ParallelComputingServiceClient

!!! note ""

    Auto-generated documentation for [ParallelComputingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService)
    type annotations stubs module [types-aiobotocore-pcs](https://pypi.org/project/types-aiobotocore-pcs/).

## ParallelComputingServiceClient

Type annotations and code completion for `#!python session.create_client("pcs")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client)

```python
# ParallelComputingServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_pcs.client import ParallelComputingServiceClient

session = get_session()
async with session.create_client("pcs") as client:
    client: ParallelComputingServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("pcs").exceptions` structure.

```python
# ParallelComputingServiceClient.exceptions usage example

async with session.create_client("pcs") as client:
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
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# ParallelComputingServiceClient usage type checking example

from types_aiobotocore_pcs.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("pcs").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("pcs").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_cluster

Creates a cluster in your account.

Type annotations and code completion for `#!python session.create_client("pcs").create_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.create_cluster)

```python
# create_cluster method definition

await def create_cluster(
    self,
    *,
    clusterName: str,
    scheduler: SchedulerRequestTypeDef,  # (1)
    size: SizeType,  # (2)
    networking: NetworkingRequestTypeDef,  # (3)
    slurmConfiguration: ClusterSlurmConfigurationRequestTypeDef = ...,  # (4)
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateClusterResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: SchedulerRequestTypeDef](./type_defs.md#schedulerrequesttypedef) 
2. See [:material-code-brackets: SizeType](./literals.md#sizetype) 
3. See [:material-code-braces: NetworkingRequestTypeDef](./type_defs.md#networkingrequesttypedef) 
4. See [:material-code-braces: ClusterSlurmConfigurationRequestTypeDef](./type_defs.md#clusterslurmconfigurationrequesttypedef) 
5. See [:material-code-braces: CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef) 


```python
# create_cluster method usage example with argument unpacking

kwargs: CreateClusterRequestRequestTypeDef = {  # (1)
    "clusterName": ...,
    "scheduler": ...,
    "size": ...,
    "networking": ...,
}

parent.create_cluster(**kwargs)
```

1. See [:material-code-braces: CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef) 

### create\_compute\_node\_group

Creates a managed set of compute nodes.

Type annotations and code completion for `#!python session.create_client("pcs").create_compute_node_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.create_compute_node_group)

```python
# create_compute_node_group method definition

await def create_compute_node_group(
    self,
    *,
    clusterIdentifier: str,
    computeNodeGroupName: str,
    subnetIds: Sequence[str],
    customLaunchTemplate: CustomLaunchTemplateTypeDef,  # (1)
    iamInstanceProfileArn: str,
    scalingConfiguration: ScalingConfigurationRequestTypeDef,  # (2)
    instanceConfigs: Sequence[InstanceConfigTypeDef],  # (3)
    amiId: str = ...,
    purchaseOption: PurchaseOptionType = ...,  # (4)
    spotOptions: SpotOptionsTypeDef = ...,  # (5)
    slurmConfiguration: ComputeNodeGroupSlurmConfigurationRequestTypeDef = ...,  # (6)
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateComputeNodeGroupResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: CustomLaunchTemplateTypeDef](./type_defs.md#customlaunchtemplatetypedef) 
2. See [:material-code-braces: ScalingConfigurationRequestTypeDef](./type_defs.md#scalingconfigurationrequesttypedef) 
3. See [:material-code-braces: InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef) 
4. See [:material-code-brackets: PurchaseOptionType](./literals.md#purchaseoptiontype) 
5. See [:material-code-braces: SpotOptionsTypeDef](./type_defs.md#spotoptionstypedef) 
6. See [:material-code-braces: ComputeNodeGroupSlurmConfigurationRequestTypeDef](./type_defs.md#computenodegroupslurmconfigurationrequesttypedef) 
7. See [:material-code-braces: CreateComputeNodeGroupResponseTypeDef](./type_defs.md#createcomputenodegroupresponsetypedef) 


```python
# create_compute_node_group method usage example with argument unpacking

kwargs: CreateComputeNodeGroupRequestRequestTypeDef = {  # (1)
    "clusterIdentifier": ...,
    "computeNodeGroupName": ...,
    "subnetIds": ...,
    "customLaunchTemplate": ...,
    "iamInstanceProfileArn": ...,
    "scalingConfiguration": ...,
    "instanceConfigs": ...,
}

parent.create_compute_node_group(**kwargs)
```

1. See [:material-code-braces: CreateComputeNodeGroupRequestRequestTypeDef](./type_defs.md#createcomputenodegrouprequestrequesttypedef) 

### create\_queue

Creates a job queue.

Type annotations and code completion for `#!python session.create_client("pcs").create_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.create_queue)

```python
# create_queue method definition

await def create_queue(
    self,
    *,
    clusterIdentifier: str,
    queueName: str,
    computeNodeGroupConfigurations: Sequence[ComputeNodeGroupConfigurationTypeDef] = ...,  # (1)
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateQueueResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ComputeNodeGroupConfigurationTypeDef](./type_defs.md#computenodegroupconfigurationtypedef) 
2. See [:material-code-braces: CreateQueueResponseTypeDef](./type_defs.md#createqueueresponsetypedef) 


```python
# create_queue method usage example with argument unpacking

kwargs: CreateQueueRequestRequestTypeDef = {  # (1)
    "clusterIdentifier": ...,
    "queueName": ...,
}

parent.create_queue(**kwargs)
```

1. See [:material-code-braces: CreateQueueRequestRequestTypeDef](./type_defs.md#createqueuerequestrequesttypedef) 

### delete\_cluster

Deletes a cluster and all its linked resources.

Type annotations and code completion for `#!python session.create_client("pcs").delete_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.delete_cluster)

```python
# delete_cluster method definition

await def delete_cluster(
    self,
    *,
    clusterIdentifier: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_cluster method usage example with argument unpacking

kwargs: DeleteClusterRequestRequestTypeDef = {  # (1)
    "clusterIdentifier": ...,
}

parent.delete_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef) 

### delete\_compute\_node\_group

Deletes a compute node group.

Type annotations and code completion for `#!python session.create_client("pcs").delete_compute_node_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.delete_compute_node_group)

```python
# delete_compute_node_group method definition

await def delete_compute_node_group(
    self,
    *,
    clusterIdentifier: str,
    computeNodeGroupIdentifier: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_compute_node_group method usage example with argument unpacking

kwargs: DeleteComputeNodeGroupRequestRequestTypeDef = {  # (1)
    "clusterIdentifier": ...,
    "computeNodeGroupIdentifier": ...,
}

parent.delete_compute_node_group(**kwargs)
```

1. See [:material-code-braces: DeleteComputeNodeGroupRequestRequestTypeDef](./type_defs.md#deletecomputenodegrouprequestrequesttypedef) 

### delete\_queue

Deletes a job queue.

Type annotations and code completion for `#!python session.create_client("pcs").delete_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.delete_queue)

```python
# delete_queue method definition

await def delete_queue(
    self,
    *,
    clusterIdentifier: str,
    queueIdentifier: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_queue method usage example with argument unpacking

kwargs: DeleteQueueRequestRequestTypeDef = {  # (1)
    "clusterIdentifier": ...,
    "queueIdentifier": ...,
}

parent.delete_queue(**kwargs)
```

1. See [:material-code-braces: DeleteQueueRequestRequestTypeDef](./type_defs.md#deletequeuerequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("pcs").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.generate_presigned_url)

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


### get\_cluster

Returns detailed information about a running cluster in your account.

Type annotations and code completion for `#!python session.create_client("pcs").get_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.get_cluster)

```python
# get_cluster method definition

await def get_cluster(
    self,
    *,
    clusterIdentifier: str,
) -> GetClusterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetClusterResponseTypeDef](./type_defs.md#getclusterresponsetypedef) 


```python
# get_cluster method usage example with argument unpacking

kwargs: GetClusterRequestRequestTypeDef = {  # (1)
    "clusterIdentifier": ...,
}

parent.get_cluster(**kwargs)
```

1. See [:material-code-braces: GetClusterRequestRequestTypeDef](./type_defs.md#getclusterrequestrequesttypedef) 

### get\_compute\_node\_group

Returns detailed information about a compute node group.

Type annotations and code completion for `#!python session.create_client("pcs").get_compute_node_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.get_compute_node_group)

```python
# get_compute_node_group method definition

await def get_compute_node_group(
    self,
    *,
    clusterIdentifier: str,
    computeNodeGroupIdentifier: str,
) -> GetComputeNodeGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetComputeNodeGroupResponseTypeDef](./type_defs.md#getcomputenodegroupresponsetypedef) 


```python
# get_compute_node_group method usage example with argument unpacking

kwargs: GetComputeNodeGroupRequestRequestTypeDef = {  # (1)
    "clusterIdentifier": ...,
    "computeNodeGroupIdentifier": ...,
}

parent.get_compute_node_group(**kwargs)
```

1. See [:material-code-braces: GetComputeNodeGroupRequestRequestTypeDef](./type_defs.md#getcomputenodegrouprequestrequesttypedef) 

### get\_queue

Returns detailed information about a queue.

Type annotations and code completion for `#!python session.create_client("pcs").get_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.get_queue)

```python
# get_queue method definition

await def get_queue(
    self,
    *,
    clusterIdentifier: str,
    queueIdentifier: str,
) -> GetQueueResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueueResponseTypeDef](./type_defs.md#getqueueresponsetypedef) 


```python
# get_queue method usage example with argument unpacking

kwargs: GetQueueRequestRequestTypeDef = {  # (1)
    "clusterIdentifier": ...,
    "queueIdentifier": ...,
}

parent.get_queue(**kwargs)
```

1. See [:material-code-braces: GetQueueRequestRequestTypeDef](./type_defs.md#getqueuerequestrequesttypedef) 

### list\_clusters

Returns a list of running clusters in your account.

Type annotations and code completion for `#!python session.create_client("pcs").list_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.list_clusters)

```python
# list_clusters method definition

await def list_clusters(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListClustersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


```python
# list_clusters method usage example with argument unpacking

kwargs: ListClustersRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_clusters(**kwargs)
```

1. See [:material-code-braces: ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef) 

### list\_compute\_node\_groups

Returns a list of all compute node groups associated with a cluster.

Type annotations and code completion for `#!python session.create_client("pcs").list_compute_node_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.list_compute_node_groups)

```python
# list_compute_node_groups method definition

await def list_compute_node_groups(
    self,
    *,
    clusterIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListComputeNodeGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListComputeNodeGroupsResponseTypeDef](./type_defs.md#listcomputenodegroupsresponsetypedef) 


```python
# list_compute_node_groups method usage example with argument unpacking

kwargs: ListComputeNodeGroupsRequestRequestTypeDef = {  # (1)
    "clusterIdentifier": ...,
}

parent.list_compute_node_groups(**kwargs)
```

1. See [:material-code-braces: ListComputeNodeGroupsRequestRequestTypeDef](./type_defs.md#listcomputenodegroupsrequestrequesttypedef) 

### list\_queues

Returns a list of all queues associated with a cluster.

Type annotations and code completion for `#!python session.create_client("pcs").list_queues` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.list_queues)

```python
# list_queues method definition

await def list_queues(
    self,
    *,
    clusterIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListQueuesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef) 


```python
# list_queues method usage example with argument unpacking

kwargs: ListQueuesRequestRequestTypeDef = {  # (1)
    "clusterIdentifier": ...,
}

parent.list_queues(**kwargs)
```

1. See [:material-code-braces: ListQueuesRequestRequestTypeDef](./type_defs.md#listqueuesrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of all tags on an Amazon Web Services PCS resource.

Type annotations and code completion for `#!python session.create_client("pcs").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### register\_compute\_node\_group\_instance

.

Type annotations and code completion for `#!python session.create_client("pcs").register_compute_node_group_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.register_compute_node_group_instance)

```python
# register_compute_node_group_instance method definition

await def register_compute_node_group_instance(
    self,
    *,
    clusterIdentifier: str,
    bootstrapId: str,
) -> RegisterComputeNodeGroupInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterComputeNodeGroupInstanceResponseTypeDef](./type_defs.md#registercomputenodegroupinstanceresponsetypedef) 


```python
# register_compute_node_group_instance method usage example with argument unpacking

kwargs: RegisterComputeNodeGroupInstanceRequestRequestTypeDef = {  # (1)
    "clusterIdentifier": ...,
    "bootstrapId": ...,
}

parent.register_compute_node_group_instance(**kwargs)
```

1. See [:material-code-braces: RegisterComputeNodeGroupInstanceRequestRequestTypeDef](./type_defs.md#registercomputenodegroupinstancerequestrequesttypedef) 

### tag\_resource

Adds or edits tags on an Amazon Web Services PCS resource.

Type annotations and code completion for `#!python session.create_client("pcs").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Deletes tags from an Amazon Web Services PCS resource.

Type annotations and code completion for `#!python session.create_client("pcs").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_compute\_node\_group

Updates a compute node group.

Type annotations and code completion for `#!python session.create_client("pcs").update_compute_node_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.update_compute_node_group)

```python
# update_compute_node_group method definition

await def update_compute_node_group(
    self,
    *,
    clusterIdentifier: str,
    computeNodeGroupIdentifier: str,
    amiId: str = ...,
    subnetIds: Sequence[str] = ...,
    customLaunchTemplate: CustomLaunchTemplateTypeDef = ...,  # (1)
    purchaseOption: PurchaseOptionType = ...,  # (2)
    spotOptions: SpotOptionsTypeDef = ...,  # (3)
    scalingConfiguration: ScalingConfigurationRequestTypeDef = ...,  # (4)
    iamInstanceProfileArn: str = ...,
    slurmConfiguration: UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef = ...,  # (5)
    clientToken: str = ...,
) -> UpdateComputeNodeGroupResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: CustomLaunchTemplateTypeDef](./type_defs.md#customlaunchtemplatetypedef) 
2. See [:material-code-brackets: PurchaseOptionType](./literals.md#purchaseoptiontype) 
3. See [:material-code-braces: SpotOptionsTypeDef](./type_defs.md#spotoptionstypedef) 
4. See [:material-code-braces: ScalingConfigurationRequestTypeDef](./type_defs.md#scalingconfigurationrequesttypedef) 
5. See [:material-code-braces: UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef](./type_defs.md#updatecomputenodegroupslurmconfigurationrequesttypedef) 
6. See [:material-code-braces: UpdateComputeNodeGroupResponseTypeDef](./type_defs.md#updatecomputenodegroupresponsetypedef) 


```python
# update_compute_node_group method usage example with argument unpacking

kwargs: UpdateComputeNodeGroupRequestRequestTypeDef = {  # (1)
    "clusterIdentifier": ...,
    "computeNodeGroupIdentifier": ...,
}

parent.update_compute_node_group(**kwargs)
```

1. See [:material-code-braces: UpdateComputeNodeGroupRequestRequestTypeDef](./type_defs.md#updatecomputenodegrouprequestrequesttypedef) 

### update\_queue

Updates the compute node group configuration of a queue.

Type annotations and code completion for `#!python session.create_client("pcs").update_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.update_queue)

```python
# update_queue method definition

await def update_queue(
    self,
    *,
    clusterIdentifier: str,
    queueIdentifier: str,
    computeNodeGroupConfigurations: Sequence[ComputeNodeGroupConfigurationTypeDef] = ...,  # (1)
    clientToken: str = ...,
) -> UpdateQueueResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ComputeNodeGroupConfigurationTypeDef](./type_defs.md#computenodegroupconfigurationtypedef) 
2. See [:material-code-braces: UpdateQueueResponseTypeDef](./type_defs.md#updatequeueresponsetypedef) 


```python
# update_queue method usage example with argument unpacking

kwargs: UpdateQueueRequestRequestTypeDef = {  # (1)
    "clusterIdentifier": ...,
    "queueIdentifier": ...,
}

parent.update_queue(**kwargs)
```

1. See [:material-code-braces: UpdateQueueRequestRequestTypeDef](./type_defs.md#updatequeuerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("pcs").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "ParallelComputingServiceClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("pcs").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("pcs").get_paginator` method with overloads.

- `client.get_paginator("list_clusters")` -> [ListClustersPaginator](./paginators.md#listclusterspaginator)
- `client.get_paginator("list_compute_node_groups")` -> [ListComputeNodeGroupsPaginator](./paginators.md#listcomputenodegroupspaginator)
- `client.get_paginator("list_queues")` -> [ListQueuesPaginator](./paginators.md#listqueuespaginator)



