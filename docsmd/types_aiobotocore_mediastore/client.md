# MediaStoreClient

> [Index](../README.md) > [MediaStore](./README.md) > MediaStoreClient

!!! note ""

    Auto-generated documentation for [MediaStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#mediastore)
    type annotations stubs module [types-aiobotocore-mediastore](https://pypi.org/project/types-aiobotocore-mediastore/).

## MediaStoreClient

Type annotations and code completion for `#!python session.create_client("mediastore")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client)

```python
# MediaStoreClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_mediastore.client import MediaStoreClient

session = get_session()
async with session.create_client("mediastore") as client:
    client: MediaStoreClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("mediastore").exceptions` structure.

```python
# MediaStoreClient.exceptions usage example

async with session.create_client("mediastore") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ContainerInUseException,
        client.ContainerNotFoundException,
        client.CorsPolicyNotFoundException,
        client.InternalServerError,
        client.LimitExceededException,
        client.PolicyNotFoundException,
    ) as e:
        print(e)
```

```python
# MediaStoreClient usage type checking example

from types_aiobotocore_mediastore.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("mediastore").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("mediastore").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/generate_presigned_url.html)

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


### create\_container

Creates a storage container to hold objects.

Type annotations and code completion for `#!python session.create_client("mediastore").create_container` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/create_container.html)

```python
# create_container method definition

await def create_container(
    self,
    *,
    ContainerName: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateContainerOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateContainerOutputTypeDef](./type_defs.md#createcontaineroutputtypedef) 


```python
# create_container method usage example with argument unpacking

kwargs: CreateContainerInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
}

parent.create_container(**kwargs)
```

1. See [:material-code-braces: CreateContainerInputRequestTypeDef](./type_defs.md#createcontainerinputrequesttypedef) 

### delete\_container

Deletes the specified container.

Type annotations and code completion for `#!python session.create_client("mediastore").delete_container` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/delete_container.html)

```python
# delete_container method definition

await def delete_container(
    self,
    *,
    ContainerName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_container method usage example with argument unpacking

kwargs: DeleteContainerInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
}

parent.delete_container(**kwargs)
```

1. See [:material-code-braces: DeleteContainerInputRequestTypeDef](./type_defs.md#deletecontainerinputrequesttypedef) 

### delete\_container\_policy

Deletes the access policy that is associated with the specified container.

Type annotations and code completion for `#!python session.create_client("mediastore").delete_container_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/delete_container_policy.html)

```python
# delete_container_policy method definition

await def delete_container_policy(
    self,
    *,
    ContainerName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_container_policy method usage example with argument unpacking

kwargs: DeleteContainerPolicyInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
}

parent.delete_container_policy(**kwargs)
```

1. See [:material-code-braces: DeleteContainerPolicyInputRequestTypeDef](./type_defs.md#deletecontainerpolicyinputrequesttypedef) 

### delete\_cors\_policy

Deletes the cross-origin resource sharing (CORS) configuration information that
is set for the container.

Type annotations and code completion for `#!python session.create_client("mediastore").delete_cors_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/delete_cors_policy.html)

```python
# delete_cors_policy method definition

await def delete_cors_policy(
    self,
    *,
    ContainerName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_cors_policy method usage example with argument unpacking

kwargs: DeleteCorsPolicyInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
}

parent.delete_cors_policy(**kwargs)
```

1. See [:material-code-braces: DeleteCorsPolicyInputRequestTypeDef](./type_defs.md#deletecorspolicyinputrequesttypedef) 

### delete\_lifecycle\_policy

Removes an object lifecycle policy from a container.

Type annotations and code completion for `#!python session.create_client("mediastore").delete_lifecycle_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/delete_lifecycle_policy.html)

```python
# delete_lifecycle_policy method definition

await def delete_lifecycle_policy(
    self,
    *,
    ContainerName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_lifecycle_policy method usage example with argument unpacking

kwargs: DeleteLifecyclePolicyInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
}

parent.delete_lifecycle_policy(**kwargs)
```

1. See [:material-code-braces: DeleteLifecyclePolicyInputRequestTypeDef](./type_defs.md#deletelifecyclepolicyinputrequesttypedef) 

### delete\_metric\_policy

Deletes the metric policy that is associated with the specified container.

Type annotations and code completion for `#!python session.create_client("mediastore").delete_metric_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/delete_metric_policy.html)

```python
# delete_metric_policy method definition

await def delete_metric_policy(
    self,
    *,
    ContainerName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_metric_policy method usage example with argument unpacking

kwargs: DeleteMetricPolicyInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
}

parent.delete_metric_policy(**kwargs)
```

1. See [:material-code-braces: DeleteMetricPolicyInputRequestTypeDef](./type_defs.md#deletemetricpolicyinputrequesttypedef) 

### describe\_container

Retrieves the properties of the requested container.

Type annotations and code completion for `#!python session.create_client("mediastore").describe_container` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/describe_container.html)

```python
# describe_container method definition

await def describe_container(
    self,
    *,
    ContainerName: str = ...,
) -> DescribeContainerOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeContainerOutputTypeDef](./type_defs.md#describecontaineroutputtypedef) 


```python
# describe_container method usage example with argument unpacking

kwargs: DescribeContainerInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
}

parent.describe_container(**kwargs)
```

1. See [:material-code-braces: DescribeContainerInputRequestTypeDef](./type_defs.md#describecontainerinputrequesttypedef) 

### get\_container\_policy

Retrieves the access policy for the specified container.

Type annotations and code completion for `#!python session.create_client("mediastore").get_container_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/get_container_policy.html)

```python
# get_container_policy method definition

await def get_container_policy(
    self,
    *,
    ContainerName: str,
) -> GetContainerPolicyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContainerPolicyOutputTypeDef](./type_defs.md#getcontainerpolicyoutputtypedef) 


```python
# get_container_policy method usage example with argument unpacking

kwargs: GetContainerPolicyInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
}

parent.get_container_policy(**kwargs)
```

1. See [:material-code-braces: GetContainerPolicyInputRequestTypeDef](./type_defs.md#getcontainerpolicyinputrequesttypedef) 

### get\_cors\_policy

Returns the cross-origin resource sharing (CORS) configuration information that
is set for the container.

Type annotations and code completion for `#!python session.create_client("mediastore").get_cors_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/get_cors_policy.html)

```python
# get_cors_policy method definition

await def get_cors_policy(
    self,
    *,
    ContainerName: str,
) -> GetCorsPolicyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCorsPolicyOutputTypeDef](./type_defs.md#getcorspolicyoutputtypedef) 


```python
# get_cors_policy method usage example with argument unpacking

kwargs: GetCorsPolicyInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
}

parent.get_cors_policy(**kwargs)
```

1. See [:material-code-braces: GetCorsPolicyInputRequestTypeDef](./type_defs.md#getcorspolicyinputrequesttypedef) 

### get\_lifecycle\_policy

Retrieves the object lifecycle policy that is assigned to a container.

Type annotations and code completion for `#!python session.create_client("mediastore").get_lifecycle_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/get_lifecycle_policy.html)

```python
# get_lifecycle_policy method definition

await def get_lifecycle_policy(
    self,
    *,
    ContainerName: str,
) -> GetLifecyclePolicyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLifecyclePolicyOutputTypeDef](./type_defs.md#getlifecyclepolicyoutputtypedef) 


```python
# get_lifecycle_policy method usage example with argument unpacking

kwargs: GetLifecyclePolicyInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
}

parent.get_lifecycle_policy(**kwargs)
```

1. See [:material-code-braces: GetLifecyclePolicyInputRequestTypeDef](./type_defs.md#getlifecyclepolicyinputrequesttypedef) 

### get\_metric\_policy

Returns the metric policy for the specified container.

Type annotations and code completion for `#!python session.create_client("mediastore").get_metric_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/get_metric_policy.html)

```python
# get_metric_policy method definition

await def get_metric_policy(
    self,
    *,
    ContainerName: str,
) -> GetMetricPolicyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMetricPolicyOutputTypeDef](./type_defs.md#getmetricpolicyoutputtypedef) 


```python
# get_metric_policy method usage example with argument unpacking

kwargs: GetMetricPolicyInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
}

parent.get_metric_policy(**kwargs)
```

1. See [:material-code-braces: GetMetricPolicyInputRequestTypeDef](./type_defs.md#getmetricpolicyinputrequesttypedef) 

### list\_containers

Lists the properties of all containers in AWS Elemental MediaStore.

Type annotations and code completion for `#!python session.create_client("mediastore").list_containers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/list_containers.html)

```python
# list_containers method definition

await def list_containers(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListContainersOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListContainersOutputTypeDef](./type_defs.md#listcontainersoutputtypedef) 


```python
# list_containers method usage example with argument unpacking

kwargs: ListContainersInputRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_containers(**kwargs)
```

1. See [:material-code-braces: ListContainersInputRequestTypeDef](./type_defs.md#listcontainersinputrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of the tags assigned to the specified container.

Type annotations and code completion for `#!python session.create_client("mediastore").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    Resource: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "Resource": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### put\_container\_policy

Creates an access policy for the specified container to restrict the users and
clients that can access it.

Type annotations and code completion for `#!python session.create_client("mediastore").put_container_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/put_container_policy.html)

```python
# put_container_policy method definition

await def put_container_policy(
    self,
    *,
    ContainerName: str,
    Policy: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_container_policy method usage example with argument unpacking

kwargs: PutContainerPolicyInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
    "Policy": ...,
}

parent.put_container_policy(**kwargs)
```

1. See [:material-code-braces: PutContainerPolicyInputRequestTypeDef](./type_defs.md#putcontainerpolicyinputrequesttypedef) 

### put\_cors\_policy

Sets the cross-origin resource sharing (CORS) configuration on a container so
that the container can service cross-origin requests.

Type annotations and code completion for `#!python session.create_client("mediastore").put_cors_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/put_cors_policy.html)

```python
# put_cors_policy method definition

await def put_cors_policy(
    self,
    *,
    ContainerName: str,
    CorsPolicy: Sequence[CorsRuleUnionTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: CorsRuleTypeDef](./type_defs.md#corsruletypedef) [:material-code-braces: CorsRuleOutputTypeDef](./type_defs.md#corsruleoutputtypedef) 


```python
# put_cors_policy method usage example with argument unpacking

kwargs: PutCorsPolicyInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
    "CorsPolicy": ...,
}

parent.put_cors_policy(**kwargs)
```

1. See [:material-code-braces: PutCorsPolicyInputRequestTypeDef](./type_defs.md#putcorspolicyinputrequesttypedef) 

### put\_lifecycle\_policy

Writes an object lifecycle policy to a container.

Type annotations and code completion for `#!python session.create_client("mediastore").put_lifecycle_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/put_lifecycle_policy.html)

```python
# put_lifecycle_policy method definition

await def put_lifecycle_policy(
    self,
    *,
    ContainerName: str,
    LifecyclePolicy: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_lifecycle_policy method usage example with argument unpacking

kwargs: PutLifecyclePolicyInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
    "LifecyclePolicy": ...,
}

parent.put_lifecycle_policy(**kwargs)
```

1. See [:material-code-braces: PutLifecyclePolicyInputRequestTypeDef](./type_defs.md#putlifecyclepolicyinputrequesttypedef) 

### put\_metric\_policy

The metric policy that you want to add to the container.

Type annotations and code completion for `#!python session.create_client("mediastore").put_metric_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/put_metric_policy.html)

```python
# put_metric_policy method definition

await def put_metric_policy(
    self,
    *,
    ContainerName: str,
    MetricPolicy: MetricPolicyTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: MetricPolicyTypeDef](./type_defs.md#metricpolicytypedef) 


```python
# put_metric_policy method usage example with argument unpacking

kwargs: PutMetricPolicyInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
    "MetricPolicy": ...,
}

parent.put_metric_policy(**kwargs)
```

1. See [:material-code-braces: PutMetricPolicyInputRequestTypeDef](./type_defs.md#putmetricpolicyinputrequesttypedef) 

### start\_access\_logging

Starts access logging on the specified container.

Type annotations and code completion for `#!python session.create_client("mediastore").start_access_logging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/start_access_logging.html)

```python
# start_access_logging method definition

await def start_access_logging(
    self,
    *,
    ContainerName: str,
) -> Dict[str, Any]:
    ...
```



```python
# start_access_logging method usage example with argument unpacking

kwargs: StartAccessLoggingInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
}

parent.start_access_logging(**kwargs)
```

1. See [:material-code-braces: StartAccessLoggingInputRequestTypeDef](./type_defs.md#startaccesslogginginputrequesttypedef) 

### stop\_access\_logging

Stops access logging on the specified container.

Type annotations and code completion for `#!python session.create_client("mediastore").stop_access_logging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/stop_access_logging.html)

```python
# stop_access_logging method definition

await def stop_access_logging(
    self,
    *,
    ContainerName: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_access_logging method usage example with argument unpacking

kwargs: StopAccessLoggingInputRequestTypeDef = {  # (1)
    "ContainerName": ...,
}

parent.stop_access_logging(**kwargs)
```

1. See [:material-code-braces: StopAccessLoggingInputRequestTypeDef](./type_defs.md#stopaccesslogginginputrequesttypedef) 

### tag\_resource

Adds tags to the specified AWS Elemental MediaStore container.

Type annotations and code completion for `#!python session.create_client("mediastore").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    Resource: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "Resource": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Removes tags from the specified container.

Type annotations and code completion for `#!python session.create_client("mediastore").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    Resource: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "Resource": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("mediastore").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("mediastore").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client)

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

Type annotations and code completion for `#!python session.create_client("mediastore").get_paginator` method with overloads.

- `client.get_paginator("list_containers")` -> [ListContainersPaginator](./paginators.md#listcontainerspaginator)



