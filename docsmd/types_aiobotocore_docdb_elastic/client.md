# DocDBElasticClient

> [Index](../README.md) > [DocDBElastic](./README.md) > DocDBElasticClient

!!! note ""

    Auto-generated documentation for [DocDBElastic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
    type annotations stubs module [types-aiobotocore-docdb-elastic](https://pypi.org/project/types-aiobotocore-docdb-elastic/).

## DocDBElasticClient

Type annotations and code completion for `#!python session.create_client("docdb-elastic")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
DocDBElasticClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_docdb_elastic.client import DocDBElasticClient

session = get_session()
async with session.create_client("docdb-elastic") as client:
    client: DocDBElasticClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("docdb-elastic").exceptions` structure.

```python
DocDBElasticClient.exceptions usage example

async with session.create_client("docdb-elastic") as client:
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
DocDBElasticClient usage type checking example

from types_aiobotocore_docdb_elastic.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("docdb-elastic").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("docdb-elastic").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_cluster

Creates a new Elastic DocumentDB cluster and returns its Cluster structure.

Type annotations and code completion for `#!python session.create_client("docdb-elastic").create_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.create_cluster)

```python
# create_cluster method definition

await def create_cluster(
    self,
    *,
    adminUserName: str,
    adminUserPassword: str,
    authType: AuthType,  # (1)
    clusterName: str,
    shardCapacity: int,
    shardCount: int,
    clientToken: str = ...,
    kmsKeyId: str = ...,
    preferredMaintenanceWindow: str = ...,
    subnetIds: Sequence[str] = ...,
    tags: Mapping[str, str] = ...,
    vpcSecurityGroupIds: Sequence[str] = ...,
) -> CreateClusterOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthType](./literals.md#authtype) 
2. See [:material-code-braces: CreateClusterOutputTypeDef](./type_defs.md#createclusteroutputtypedef) 


```python
# create_cluster method usage example with argument unpacking

kwargs: CreateClusterInputRequestTypeDef = {  # (1)
    "adminUserName": ...,
    "adminUserPassword": ...,
    "authType": ...,
    "clusterName": ...,
    "shardCapacity": ...,
    "shardCount": ...,
}

parent.create_cluster(**kwargs)
```

1. See [:material-code-braces: CreateClusterInputRequestTypeDef](./type_defs.md#createclusterinputrequesttypedef) 

### create\_cluster\_snapshot

Creates a snapshot of a cluster.

Type annotations and code completion for `#!python session.create_client("docdb-elastic").create_cluster_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.create_cluster_snapshot)

```python
# create_cluster_snapshot method definition

await def create_cluster_snapshot(
    self,
    *,
    clusterArn: str,
    snapshotName: str,
    tags: Mapping[str, str] = ...,
) -> CreateClusterSnapshotOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateClusterSnapshotOutputTypeDef](./type_defs.md#createclustersnapshotoutputtypedef) 


```python
# create_cluster_snapshot method usage example with argument unpacking

kwargs: CreateClusterSnapshotInputRequestTypeDef = {  # (1)
    "clusterArn": ...,
    "snapshotName": ...,
}

parent.create_cluster_snapshot(**kwargs)
```

1. See [:material-code-braces: CreateClusterSnapshotInputRequestTypeDef](./type_defs.md#createclustersnapshotinputrequesttypedef) 

### delete\_cluster

Delete a Elastic DocumentDB cluster.

Type annotations and code completion for `#!python session.create_client("docdb-elastic").delete_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.delete_cluster)

```python
# delete_cluster method definition

await def delete_cluster(
    self,
    *,
    clusterArn: str,
) -> DeleteClusterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteClusterOutputTypeDef](./type_defs.md#deleteclusteroutputtypedef) 


```python
# delete_cluster method usage example with argument unpacking

kwargs: DeleteClusterInputRequestTypeDef = {  # (1)
    "clusterArn": ...,
}

parent.delete_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteClusterInputRequestTypeDef](./type_defs.md#deleteclusterinputrequesttypedef) 

### delete\_cluster\_snapshot

Delete a Elastic DocumentDB snapshot.

Type annotations and code completion for `#!python session.create_client("docdb-elastic").delete_cluster_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.delete_cluster_snapshot)

```python
# delete_cluster_snapshot method definition

await def delete_cluster_snapshot(
    self,
    *,
    snapshotArn: str,
) -> DeleteClusterSnapshotOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteClusterSnapshotOutputTypeDef](./type_defs.md#deleteclustersnapshotoutputtypedef) 


```python
# delete_cluster_snapshot method usage example with argument unpacking

kwargs: DeleteClusterSnapshotInputRequestTypeDef = {  # (1)
    "snapshotArn": ...,
}

parent.delete_cluster_snapshot(**kwargs)
```

1. See [:material-code-braces: DeleteClusterSnapshotInputRequestTypeDef](./type_defs.md#deleteclustersnapshotinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("docdb-elastic").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.generate_presigned_url)

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

Returns information about a specific Elastic DocumentDB cluster.

Type annotations and code completion for `#!python session.create_client("docdb-elastic").get_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.get_cluster)

```python
# get_cluster method definition

await def get_cluster(
    self,
    *,
    clusterArn: str,
) -> GetClusterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetClusterOutputTypeDef](./type_defs.md#getclusteroutputtypedef) 


```python
# get_cluster method usage example with argument unpacking

kwargs: GetClusterInputRequestTypeDef = {  # (1)
    "clusterArn": ...,
}

parent.get_cluster(**kwargs)
```

1. See [:material-code-braces: GetClusterInputRequestTypeDef](./type_defs.md#getclusterinputrequesttypedef) 

### get\_cluster\_snapshot

Returns information about a specific Elastic DocumentDB snapshot See also: [AWS
API Documentation](https://docs.aws.amazon.com/goto/WebAPI/docdb-
elastic-2022-11-28/GetClusterSnapshot).

Type annotations and code completion for `#!python session.create_client("docdb-elastic").get_cluster_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.get_cluster_snapshot)

```python
# get_cluster_snapshot method definition

await def get_cluster_snapshot(
    self,
    *,
    snapshotArn: str,
) -> GetClusterSnapshotOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetClusterSnapshotOutputTypeDef](./type_defs.md#getclustersnapshotoutputtypedef) 


```python
# get_cluster_snapshot method usage example with argument unpacking

kwargs: GetClusterSnapshotInputRequestTypeDef = {  # (1)
    "snapshotArn": ...,
}

parent.get_cluster_snapshot(**kwargs)
```

1. See [:material-code-braces: GetClusterSnapshotInputRequestTypeDef](./type_defs.md#getclustersnapshotinputrequesttypedef) 

### list\_cluster\_snapshots

Returns information about Elastic DocumentDB snapshots for a specified cluster.

Type annotations and code completion for `#!python session.create_client("docdb-elastic").list_cluster_snapshots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.list_cluster_snapshots)

```python
# list_cluster_snapshots method definition

await def list_cluster_snapshots(
    self,
    *,
    clusterArn: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListClusterSnapshotsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListClusterSnapshotsOutputTypeDef](./type_defs.md#listclustersnapshotsoutputtypedef) 


```python
# list_cluster_snapshots method usage example with argument unpacking

kwargs: ListClusterSnapshotsInputRequestTypeDef = {  # (1)
    "clusterArn": ...,
}

parent.list_cluster_snapshots(**kwargs)
```

1. See [:material-code-braces: ListClusterSnapshotsInputRequestTypeDef](./type_defs.md#listclustersnapshotsinputrequesttypedef) 

### list\_clusters

Returns information about provisioned Elastic DocumentDB clusters.

Type annotations and code completion for `#!python session.create_client("docdb-elastic").list_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.list_clusters)

```python
# list_clusters method definition

await def list_clusters(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListClustersOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef) 


```python
# list_clusters method usage example with argument unpacking

kwargs: ListClustersInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_clusters(**kwargs)
```

1. See [:material-code-braces: ListClustersInputRequestTypeDef](./type_defs.md#listclustersinputrequesttypedef) 

### list\_tags\_for\_resource

Lists all tags on a Elastic DocumentDB resource See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/docdb-
elastic-2022-11-28/ListTagsForResource).

Type annotations and code completion for `#!python session.create_client("docdb-elastic").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.list_tags_for_resource)

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

### restore\_cluster\_from\_snapshot

Restores a Elastic DocumentDB cluster from a snapshot.

Type annotations and code completion for `#!python session.create_client("docdb-elastic").restore_cluster_from_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.restore_cluster_from_snapshot)

```python
# restore_cluster_from_snapshot method definition

await def restore_cluster_from_snapshot(
    self,
    *,
    clusterName: str,
    snapshotArn: str,
    kmsKeyId: str = ...,
    subnetIds: Sequence[str] = ...,
    tags: Mapping[str, str] = ...,
    vpcSecurityGroupIds: Sequence[str] = ...,
) -> RestoreClusterFromSnapshotOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RestoreClusterFromSnapshotOutputTypeDef](./type_defs.md#restoreclusterfromsnapshotoutputtypedef) 


```python
# restore_cluster_from_snapshot method usage example with argument unpacking

kwargs: RestoreClusterFromSnapshotInputRequestTypeDef = {  # (1)
    "clusterName": ...,
    "snapshotArn": ...,
}

parent.restore_cluster_from_snapshot(**kwargs)
```

1. See [:material-code-braces: RestoreClusterFromSnapshotInputRequestTypeDef](./type_defs.md#restoreclusterfromsnapshotinputrequesttypedef) 

### tag\_resource

Adds metadata tags to a Elastic DocumentDB resource See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/docdb-
elastic-2022-11-28/TagResource).

Type annotations and code completion for `#!python session.create_client("docdb-elastic").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.tag_resource)

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

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes metadata tags to a Elastic DocumentDB resource See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/docdb-
elastic-2022-11-28/UntagResource).

Type annotations and code completion for `#!python session.create_client("docdb-elastic").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.untag_resource)

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

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_cluster

Modifies a Elastic DocumentDB cluster.

Type annotations and code completion for `#!python session.create_client("docdb-elastic").update_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.update_cluster)

```python
# update_cluster method definition

await def update_cluster(
    self,
    *,
    clusterArn: str,
    adminUserPassword: str = ...,
    authType: AuthType = ...,  # (1)
    clientToken: str = ...,
    preferredMaintenanceWindow: str = ...,
    shardCapacity: int = ...,
    shardCount: int = ...,
    subnetIds: Sequence[str] = ...,
    vpcSecurityGroupIds: Sequence[str] = ...,
) -> UpdateClusterOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthType](./literals.md#authtype) 
2. See [:material-code-braces: UpdateClusterOutputTypeDef](./type_defs.md#updateclusteroutputtypedef) 


```python
# update_cluster method usage example with argument unpacking

kwargs: UpdateClusterInputRequestTypeDef = {  # (1)
    "clusterArn": ...,
}

parent.update_cluster(**kwargs)
```

1. See [:material-code-braces: UpdateClusterInputRequestTypeDef](./type_defs.md#updateclusterinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("docdb-elastic").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> DocDBElasticClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("docdb-elastic").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("docdb-elastic").get_paginator` method with overloads.

- `client.get_paginator("list_cluster_snapshots")` -> [ListClusterSnapshotsPaginator](./paginators.md#listclustersnapshotspaginator)
- `client.get_paginator("list_clusters")` -> [ListClustersPaginator](./paginators.md#listclusterspaginator)



