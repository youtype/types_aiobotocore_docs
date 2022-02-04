<a id="mediastoreclient-for-aiobotocore-mediastore-module"></a>

# MediaStoreClient for aiobotocore MediaStore module

> [Index](..) > [MediaStore](.) > MediaStoreClient

Auto-generated documentation for
[MediaStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
type annotations stubs module
[types-aiobotocore-mediastore](https://pypi.org/project/types-aiobotocore-mediastore/).

- [MediaStoreClient for aiobotocore MediaStore module](#mediastoreclient-for-aiobotocore-mediastore-module)
  - [MediaStoreClient](#mediastoreclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_container](#create_container)
    - [delete_container](#delete_container)
    - [delete_container_policy](#delete_container_policy)
    - [delete_cors_policy](#delete_cors_policy)
    - [delete_lifecycle_policy](#delete_lifecycle_policy)
    - [delete_metric_policy](#delete_metric_policy)
    - [describe_container](#describe_container)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_container_policy](#get_container_policy)
    - [get_cors_policy](#get_cors_policy)
    - [get_lifecycle_policy](#get_lifecycle_policy)
    - [get_metric_policy](#get_metric_policy)
    - [list_containers](#list_containers)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [put_container_policy](#put_container_policy)
    - [put_cors_policy](#put_cors_policy)
    - [put_lifecycle_policy](#put_lifecycle_policy)
    - [put_metric_policy](#put_metric_policy)
    - [start_access_logging](#start_access_logging)
    - [stop_access_logging](#stop_access_logging)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [get_paginator](#get_paginator)

<a id="mediastoreclient"></a>

## MediaStoreClient

Type annotations for `aiobotocore.create_client("mediastore")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_mediastore.client import MediaStoreClient

def get_mediastore_client() -> MediaStoreClient:
    return Session().client("mediastore")
```

Boto3 documentation:
[MediaStore.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_mediastore.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ContainerInUseException`
- `Exceptions.ContainerNotFoundException`
- `Exceptions.CorsPolicyNotFoundException`
- `Exceptions.InternalServerError`
- `Exceptions.LimitExceededException`
- `Exceptions.PolicyNotFoundException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

MediaStoreClient exceptions.

Type annotations for `aiobotocore.create_client("mediastore").exceptions`
method.

Boto3 documentation:
[MediaStore.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("mediastore").can_paginate`
method.

Boto3 documentation:
[MediaStore.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_container"></a>

### create_container

Creates a storage container to hold objects.

Type annotations for `aiobotocore.create_client("mediastore").create_container`
method.

Boto3 documentation:
[MediaStore.Client.create_container](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.create_container)

Asynchronous method. Use `await create_container(...)` for a synchronous call.

Arguments mapping described in
[CreateContainerInputRequestTypeDef](./type_defs.md#createcontainerinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateContainerOutputTypeDef](./type_defs.md#createcontaineroutputtypedef).

<a id="delete_container"></a>

### delete_container

Deletes the specified container.

Type annotations for `aiobotocore.create_client("mediastore").delete_container`
method.

Boto3 documentation:
[MediaStore.Client.delete_container](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.delete_container)

Asynchronous method. Use `await delete_container(...)` for a synchronous call.

Arguments mapping described in
[DeleteContainerInputRequestTypeDef](./type_defs.md#deletecontainerinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_container_policy"></a>

### delete_container_policy

Deletes the access policy that is associated with the specified container.

Type annotations for
`aiobotocore.create_client("mediastore").delete_container_policy` method.

Boto3 documentation:
[MediaStore.Client.delete_container_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.delete_container_policy)

Asynchronous method. Use `await delete_container_policy(...)` for a synchronous
call.

Arguments mapping described in
[DeleteContainerPolicyInputRequestTypeDef](./type_defs.md#deletecontainerpolicyinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_cors_policy"></a>

### delete_cors_policy

Deletes the cross-origin resource sharing (CORS) configuration information that
is set for the container.

Type annotations for
`aiobotocore.create_client("mediastore").delete_cors_policy` method.

Boto3 documentation:
[MediaStore.Client.delete_cors_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.delete_cors_policy)

Asynchronous method. Use `await delete_cors_policy(...)` for a synchronous
call.

Arguments mapping described in
[DeleteCorsPolicyInputRequestTypeDef](./type_defs.md#deletecorspolicyinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_lifecycle_policy"></a>

### delete_lifecycle_policy

Removes an object lifecycle policy from a container.

Type annotations for
`aiobotocore.create_client("mediastore").delete_lifecycle_policy` method.

Boto3 documentation:
[MediaStore.Client.delete_lifecycle_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.delete_lifecycle_policy)

Asynchronous method. Use `await delete_lifecycle_policy(...)` for a synchronous
call.

Arguments mapping described in
[DeleteLifecyclePolicyInputRequestTypeDef](./type_defs.md#deletelifecyclepolicyinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_metric_policy"></a>

### delete_metric_policy

Deletes the metric policy that is associated with the specified container.

Type annotations for
`aiobotocore.create_client("mediastore").delete_metric_policy` method.

Boto3 documentation:
[MediaStore.Client.delete_metric_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.delete_metric_policy)

Asynchronous method. Use `await delete_metric_policy(...)` for a synchronous
call.

Arguments mapping described in
[DeleteMetricPolicyInputRequestTypeDef](./type_defs.md#deletemetricpolicyinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_container"></a>

### describe_container

Retrieves the properties of the requested container.

Type annotations for
`aiobotocore.create_client("mediastore").describe_container` method.

Boto3 documentation:
[MediaStore.Client.describe_container](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.describe_container)

Asynchronous method. Use `await describe_container(...)` for a synchronous
call.

Arguments mapping described in
[DescribeContainerInputRequestTypeDef](./type_defs.md#describecontainerinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str`

Returns a `Coroutine` for
[DescribeContainerOutputTypeDef](./type_defs.md#describecontaineroutputtypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("mediastore").generate_presigned_url` method.

Boto3 documentation:
[MediaStore.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_container_policy"></a>

### get_container_policy

Retrieves the access policy for the specified container.

Type annotations for
`aiobotocore.create_client("mediastore").get_container_policy` method.

Boto3 documentation:
[MediaStore.Client.get_container_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.get_container_policy)

Asynchronous method. Use `await get_container_policy(...)` for a synchronous
call.

Arguments mapping described in
[GetContainerPolicyInputRequestTypeDef](./type_defs.md#getcontainerpolicyinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*

Returns a `Coroutine` for
[GetContainerPolicyOutputTypeDef](./type_defs.md#getcontainerpolicyoutputtypedef).

<a id="get_cors_policy"></a>

### get_cors_policy

Returns the cross-origin resource sharing (CORS) configuration information that
is set for the container.

Type annotations for `aiobotocore.create_client("mediastore").get_cors_policy`
method.

Boto3 documentation:
[MediaStore.Client.get_cors_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.get_cors_policy)

Asynchronous method. Use `await get_cors_policy(...)` for a synchronous call.

Arguments mapping described in
[GetCorsPolicyInputRequestTypeDef](./type_defs.md#getcorspolicyinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*

Returns a `Coroutine` for
[GetCorsPolicyOutputTypeDef](./type_defs.md#getcorspolicyoutputtypedef).

<a id="get_lifecycle_policy"></a>

### get_lifecycle_policy

Retrieves the object lifecycle policy that is assigned to a container.

Type annotations for
`aiobotocore.create_client("mediastore").get_lifecycle_policy` method.

Boto3 documentation:
[MediaStore.Client.get_lifecycle_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.get_lifecycle_policy)

Asynchronous method. Use `await get_lifecycle_policy(...)` for a synchronous
call.

Arguments mapping described in
[GetLifecyclePolicyInputRequestTypeDef](./type_defs.md#getlifecyclepolicyinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*

Returns a `Coroutine` for
[GetLifecyclePolicyOutputTypeDef](./type_defs.md#getlifecyclepolicyoutputtypedef).

<a id="get_metric_policy"></a>

### get_metric_policy

Returns the metric policy for the specified container.

Type annotations for
`aiobotocore.create_client("mediastore").get_metric_policy` method.

Boto3 documentation:
[MediaStore.Client.get_metric_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.get_metric_policy)

Asynchronous method. Use `await get_metric_policy(...)` for a synchronous call.

Arguments mapping described in
[GetMetricPolicyInputRequestTypeDef](./type_defs.md#getmetricpolicyinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*

Returns a `Coroutine` for
[GetMetricPolicyOutputTypeDef](./type_defs.md#getmetricpolicyoutputtypedef).

<a id="list_containers"></a>

### list_containers

Lists the properties of all containers in AWS Elemental MediaStore.

Type annotations for `aiobotocore.create_client("mediastore").list_containers`
method.

Boto3 documentation:
[MediaStore.Client.list_containers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.list_containers)

Asynchronous method. Use `await list_containers(...)` for a synchronous call.

Arguments mapping described in
[ListContainersInputRequestTypeDef](./type_defs.md#listcontainersinputrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListContainersOutputTypeDef](./type_defs.md#listcontainersoutputtypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Returns a list of the tags assigned to the specified container.

Type annotations for
`aiobotocore.create_client("mediastore").list_tags_for_resource` method.

Boto3 documentation:
[MediaStore.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef).

Keyword-only arguments:

- `Resource`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef).

<a id="put_container_policy"></a>

### put_container_policy

Creates an access policy for the specified container to restrict the users and
clients that can access it.

Type annotations for
`aiobotocore.create_client("mediastore").put_container_policy` method.

Boto3 documentation:
[MediaStore.Client.put_container_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_container_policy)

Asynchronous method. Use `await put_container_policy(...)` for a synchronous
call.

Arguments mapping described in
[PutContainerPolicyInputRequestTypeDef](./type_defs.md#putcontainerpolicyinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*
- `Policy`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="put_cors_policy"></a>

### put_cors_policy

Sets the cross-origin resource sharing (CORS) configuration on a container so
that the container can service cross-origin requests.

Type annotations for `aiobotocore.create_client("mediastore").put_cors_policy`
method.

Boto3 documentation:
[MediaStore.Client.put_cors_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_cors_policy)

Asynchronous method. Use `await put_cors_policy(...)` for a synchronous call.

Arguments mapping described in
[PutCorsPolicyInputRequestTypeDef](./type_defs.md#putcorspolicyinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*
- `CorsPolicy`: `Sequence`\[[CorsRuleTypeDef](./type_defs.md#corsruletypedef)\]
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="put_lifecycle_policy"></a>

### put_lifecycle_policy

Writes an object lifecycle policy to a container.

Type annotations for
`aiobotocore.create_client("mediastore").put_lifecycle_policy` method.

Boto3 documentation:
[MediaStore.Client.put_lifecycle_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_lifecycle_policy)

Asynchronous method. Use `await put_lifecycle_policy(...)` for a synchronous
call.

Arguments mapping described in
[PutLifecyclePolicyInputRequestTypeDef](./type_defs.md#putlifecyclepolicyinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*
- `LifecyclePolicy`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="put_metric_policy"></a>

### put_metric_policy

The metric policy that you want to add to the container.

Type annotations for
`aiobotocore.create_client("mediastore").put_metric_policy` method.

Boto3 documentation:
[MediaStore.Client.put_metric_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_metric_policy)

Asynchronous method. Use `await put_metric_policy(...)` for a synchronous call.

Arguments mapping described in
[PutMetricPolicyInputRequestTypeDef](./type_defs.md#putmetricpolicyinputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*
- `MetricPolicy`: [MetricPolicyTypeDef](./type_defs.md#metricpolicytypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="start_access_logging"></a>

### start_access_logging

Starts access logging on the specified container.

Type annotations for
`aiobotocore.create_client("mediastore").start_access_logging` method.

Boto3 documentation:
[MediaStore.Client.start_access_logging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.start_access_logging)

Asynchronous method. Use `await start_access_logging(...)` for a synchronous
call.

Arguments mapping described in
[StartAccessLoggingInputRequestTypeDef](./type_defs.md#startaccesslogginginputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="stop_access_logging"></a>

### stop_access_logging

Stops access logging on the specified container.

Type annotations for
`aiobotocore.create_client("mediastore").stop_access_logging` method.

Boto3 documentation:
[MediaStore.Client.stop_access_logging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.stop_access_logging)

Asynchronous method. Use `await stop_access_logging(...)` for a synchronous
call.

Arguments mapping described in
[StopAccessLoggingInputRequestTypeDef](./type_defs.md#stopaccesslogginginputrequesttypedef).

Keyword-only arguments:

- `ContainerName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="tag_resource"></a>

### tag_resource

Adds tags to the specified AWS Elemental MediaStore container.

Type annotations for `aiobotocore.create_client("mediastore").tag_resource`
method.

Boto3 documentation:
[MediaStore.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef).

Keyword-only arguments:

- `Resource`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes tags from the specified container.

Type annotations for `aiobotocore.create_client("mediastore").untag_resource`
method.

Boto3 documentation:
[MediaStore.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef).

Keyword-only arguments:

- `Resource`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("mediastore").get_paginator`
method with overloads.

- `client.get_paginator("list_containers")` ->
  [ListContainersPaginator](./paginators.md#listcontainerspaginator)
