# AuroraDSQLClient

> [Index](../README.md) > [AuroraDSQL](./README.md) > AuroraDSQLClient

!!! note ""

    Auto-generated documentation for [AuroraDSQL](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql.html#auroradsql)
    type annotations stubs module [types-aiobotocore-dsql](https://pypi.org/project/types-aiobotocore-dsql/).

## AuroraDSQLClient

Type annotations and code completion for `#!python session.create_client("dsql")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql.html#AuroraDSQL.Client)

```python
# AuroraDSQLClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_dsql.client import AuroraDSQLClient

session = get_session()
async with session.create_client("dsql") as client:
    client: AuroraDSQLClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("dsql").exceptions` structure.

```python
# AuroraDSQLClient.exceptions usage example

async with session.create_client("dsql") as client:
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
# AuroraDSQLClient usage type checking example

from types_aiobotocore_dsql.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("dsql").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("dsql").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/client/generate_presigned_url.html)

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


### create\_cluster

Creates a cluster in Amazon Aurora DSQL.

Type annotations and code completion for `#!python session.create_client("dsql").create_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/client/create_cluster.html)

```python
# create_cluster method definition

await def create_cluster(
    self,
    *,
    deletionProtectionEnabled: bool = ...,
    tags: Mapping[str, str] = ...,
    clientToken: str = ...,
) -> CreateClusterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateClusterOutputTypeDef](./type_defs.md#createclusteroutputtypedef) 


```python
# create_cluster method usage example with argument unpacking

kwargs: CreateClusterInputTypeDef = {  # (1)
    "deletionProtectionEnabled": ...,
}

parent.create_cluster(**kwargs)
```

1. See [:material-code-braces: CreateClusterInputTypeDef](./type_defs.md#createclusterinputtypedef) 

### create\_multi\_region\_clusters

Creates multi-Region clusters in Amazon Aurora DSQL.

Type annotations and code completion for `#!python session.create_client("dsql").create_multi_region_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/client/create_multi_region_clusters.html)

```python
# create_multi_region_clusters method definition

await def create_multi_region_clusters(
    self,
    *,
    linkedRegionList: Sequence[str],
    witnessRegion: str,
    clusterProperties: Mapping[str, LinkedClusterPropertiesTypeDef] = ...,  # (1)
    clientToken: str = ...,
) -> CreateMultiRegionClustersOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LinkedClusterPropertiesTypeDef](./type_defs.md#linkedclusterpropertiestypedef) 
2. See [:material-code-braces: CreateMultiRegionClustersOutputTypeDef](./type_defs.md#createmultiregionclustersoutputtypedef) 


```python
# create_multi_region_clusters method usage example with argument unpacking

kwargs: CreateMultiRegionClustersInputTypeDef = {  # (1)
    "linkedRegionList": ...,
    "witnessRegion": ...,
}

parent.create_multi_region_clusters(**kwargs)
```

1. See [:material-code-braces: CreateMultiRegionClustersInputTypeDef](./type_defs.md#createmultiregionclustersinputtypedef) 

### delete\_cluster

Deletes a cluster in Amazon Aurora DSQL.

Type annotations and code completion for `#!python session.create_client("dsql").delete_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/client/delete_cluster.html)

```python
# delete_cluster method definition

await def delete_cluster(
    self,
    *,
    identifier: str,
    clientToken: str = ...,
) -> DeleteClusterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteClusterOutputTypeDef](./type_defs.md#deleteclusteroutputtypedef) 


```python
# delete_cluster method usage example with argument unpacking

kwargs: DeleteClusterInputTypeDef = {  # (1)
    "identifier": ...,
}

parent.delete_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteClusterInputTypeDef](./type_defs.md#deleteclusterinputtypedef) 

### delete\_multi\_region\_clusters

Deletes a multi-Region cluster in Amazon Aurora DSQL.

Type annotations and code completion for `#!python session.create_client("dsql").delete_multi_region_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/client/delete_multi_region_clusters.html)

```python
# delete_multi_region_clusters method definition

await def delete_multi_region_clusters(
    self,
    *,
    linkedClusterArns: Sequence[str],
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_multi_region_clusters method usage example with argument unpacking

kwargs: DeleteMultiRegionClustersInputTypeDef = {  # (1)
    "linkedClusterArns": ...,
}

parent.delete_multi_region_clusters(**kwargs)
```

1. See [:material-code-braces: DeleteMultiRegionClustersInputTypeDef](./type_defs.md#deletemultiregionclustersinputtypedef) 

### get\_cluster

Retrieves information about a cluster.

Type annotations and code completion for `#!python session.create_client("dsql").get_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/client/get_cluster.html)

```python
# get_cluster method definition

await def get_cluster(
    self,
    *,
    identifier: str,
) -> GetClusterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetClusterOutputTypeDef](./type_defs.md#getclusteroutputtypedef) 


```python
# get_cluster method usage example with argument unpacking

kwargs: GetClusterInputTypeDef = {  # (1)
    "identifier": ...,
}

parent.get_cluster(**kwargs)
```

1. See [:material-code-braces: GetClusterInputTypeDef](./type_defs.md#getclusterinputtypedef) 

### list\_clusters

Retrieves information about a list of clusters.

Type annotations and code completion for `#!python session.create_client("dsql").list_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/client/list_clusters.html)

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

kwargs: ListClustersInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_clusters(**kwargs)
```

1. See [:material-code-braces: ListClustersInputTypeDef](./type_defs.md#listclustersinputtypedef) 

### list\_tags\_for\_resource

Lists all of the tags for a resource.

Type annotations and code completion for `#!python session.create_client("dsql").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/client/list_tags_for_resource.html)

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

kwargs: ListTagsForResourceInputTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef) 

### tag\_resource

Tags a resource with a map of key and value pairs.

Type annotations and code completion for `#!python session.create_client("dsql").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/client/tag_resource.html)

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

kwargs: TagResourceInputTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef) 

### untag\_resource

Removes a tag from a resource.

Type annotations and code completion for `#!python session.create_client("dsql").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/client/untag_resource.html)

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

kwargs: UntagResourceInputTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef) 

### update\_cluster

Updates a cluster.

Type annotations and code completion for `#!python session.create_client("dsql").update_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql/client/update_cluster.html)

```python
# update_cluster method definition

await def update_cluster(
    self,
    *,
    identifier: str,
    deletionProtectionEnabled: bool = ...,
    clientToken: str = ...,
) -> UpdateClusterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateClusterOutputTypeDef](./type_defs.md#updateclusteroutputtypedef) 


```python
# update_cluster method usage example with argument unpacking

kwargs: UpdateClusterInputTypeDef = {  # (1)
    "identifier": ...,
}

parent.update_cluster(**kwargs)
```

1. See [:material-code-braces: UpdateClusterInputTypeDef](./type_defs.md#updateclusterinputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("dsql").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql.html#AuroraDSQL.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("dsql").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql.html#AuroraDSQL.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("dsql").get_paginator` method with overloads.

- `client.get_paginator("list_clusters")` -> [ListClustersPaginator](./paginators.md#listclusterspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("dsql").get_waiter` method with overloads.

- `client.get_waiter("cluster_active")` -> [ClusterActiveWaiter](./waiters.md#clusteractivewaiter)
- `client.get_waiter("cluster_not_exists")` -> [ClusterNotExistsWaiter](./waiters.md#clusternotexistswaiter)

