<a id="cloudcontrolapiclient-for-aiobotocore-cloudcontrolapi-module"></a>

# CloudControlApiClient for aiobotocore CloudControlApi module

> [Index](../README.md) > [CloudControlApi](./README.md) >
> CloudControlApiClient

Auto-generated documentation for
[CloudControlApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
type annotations stubs module
[types-aiobotocore-cloudcontrol](https://pypi.org/project/types-aiobotocore-cloudcontrol/).

- [CloudControlApiClient for aiobotocore CloudControlApi module](#cloudcontrolapiclient-for-aiobotocore-cloudcontrolapi-module)
  - [CloudControlApiClient](#cloudcontrolapiclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [cancel_resource_request](#cancel_resource_request)
    - [create_resource](#create_resource)
    - [delete_resource](#delete_resource)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_resource](#get_resource)
    - [get_resource_request_status](#get_resource_request_status)
    - [list_resource_requests](#list_resource_requests)
    - [list_resources](#list_resources)
    - [update_resource](#update_resource)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_waiter](#get_waiter)

<a id="cloudcontrolapiclient"></a>

## CloudControlApiClient

Type annotations for `session.create_client("cloudcontrol")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_cloudcontrol.client import CloudControlApiClient

session = get_session()
async with session.create_client("cloudcontrol") as client:
    client: CloudControlApiClient
```

Boto3 documentation:
[CloudControlApi.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_cloudcontrol.client import Exceptions

def handle_error(exc: Exceptions.AlreadyExistsException) -> None:
    ...
```

Exceptions:

- `Exceptions.AlreadyExistsException`
- `Exceptions.ClientError`
- `Exceptions.ClientTokenConflictException`
- `Exceptions.ConcurrentModificationException`
- `Exceptions.ConcurrentOperationException`
- `Exceptions.GeneralServiceException`
- `Exceptions.HandlerFailureException`
- `Exceptions.HandlerInternalFailureException`
- `Exceptions.InvalidCredentialsException`
- `Exceptions.InvalidRequestException`
- `Exceptions.NetworkFailureException`
- `Exceptions.NotStabilizedException`
- `Exceptions.NotUpdatableException`
- `Exceptions.PrivateTypeException`
- `Exceptions.RequestTokenNotFoundException`
- `Exceptions.ResourceConflictException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceInternalErrorException`
- `Exceptions.ServiceLimitExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.TypeNotFoundException`
- `Exceptions.UnsupportedActionException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

CloudControlApiClient exceptions.

Type annotations for `session.create_client("cloudcontrol").exceptions` method.

Boto3 documentation:
[CloudControlApi.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("cloudcontrol").can_paginate`
method.

Boto3 documentation:
[CloudControlApi.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel\_resource\_request"></a>

### cancel_resource_request

Cancels the specified resource operation request.

Type annotations for
`session.create_client("cloudcontrol").cancel_resource_request` method.

Boto3 documentation:
[CloudControlApi.Client.cancel_resource_request](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.cancel_resource_request)

Asynchronous method. Use `await cancel_resource_request(...)` for a synchronous
call.

Arguments mapping described in
[CancelResourceRequestInputRequestTypeDef](./type_defs.md#cancelresourcerequestinputrequesttypedef).

Keyword-only arguments:

- `RequestToken`: `str` *(required)*

Returns a `Coroutine` for
[CancelResourceRequestOutputTypeDef](./type_defs.md#cancelresourcerequestoutputtypedef).

<a id="create\_resource"></a>

### create_resource

Creates the specified resource.

Type annotations for `session.create_client("cloudcontrol").create_resource`
method.

Boto3 documentation:
[CloudControlApi.Client.create_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.create_resource)

Asynchronous method. Use `await create_resource(...)` for a synchronous call.

Arguments mapping described in
[CreateResourceInputRequestTypeDef](./type_defs.md#createresourceinputrequesttypedef).

Keyword-only arguments:

- `TypeName`: `str` *(required)*
- `DesiredState`: `str` *(required)*
- `TypeVersionId`: `str`
- `RoleArn`: `str`
- `ClientToken`: `str`

Returns a `Coroutine` for
[CreateResourceOutputTypeDef](./type_defs.md#createresourceoutputtypedef).

<a id="delete\_resource"></a>

### delete_resource

Deletes the specified resource.

Type annotations for `session.create_client("cloudcontrol").delete_resource`
method.

Boto3 documentation:
[CloudControlApi.Client.delete_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.delete_resource)

Asynchronous method. Use `await delete_resource(...)` for a synchronous call.

Arguments mapping described in
[DeleteResourceInputRequestTypeDef](./type_defs.md#deleteresourceinputrequesttypedef).

Keyword-only arguments:

- `TypeName`: `str` *(required)*
- `Identifier`: `str` *(required)*
- `TypeVersionId`: `str`
- `RoleArn`: `str`
- `ClientToken`: `str`

Returns a `Coroutine` for
[DeleteResourceOutputTypeDef](./type_defs.md#deleteresourceoutputtypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("cloudcontrol").generate_presigned_url` method.

Boto3 documentation:
[CloudControlApi.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_resource"></a>

### get_resource

Returns information about the current state of the specified resource.

Type annotations for `session.create_client("cloudcontrol").get_resource`
method.

Boto3 documentation:
[CloudControlApi.Client.get_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.get_resource)

Asynchronous method. Use `await get_resource(...)` for a synchronous call.

Arguments mapping described in
[GetResourceInputRequestTypeDef](./type_defs.md#getresourceinputrequesttypedef).

Keyword-only arguments:

- `TypeName`: `str` *(required)*
- `Identifier`: `str` *(required)*
- `TypeVersionId`: `str`
- `RoleArn`: `str`

Returns a `Coroutine` for
[GetResourceOutputTypeDef](./type_defs.md#getresourceoutputtypedef).

<a id="get\_resource\_request\_status"></a>

### get_resource_request_status

Returns the current status of a resource operation request.

Type annotations for
`session.create_client("cloudcontrol").get_resource_request_status` method.

Boto3 documentation:
[CloudControlApi.Client.get_resource_request_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.get_resource_request_status)

Asynchronous method. Use `await get_resource_request_status(...)` for a
synchronous call.

Arguments mapping described in
[GetResourceRequestStatusInputRequestTypeDef](./type_defs.md#getresourcerequeststatusinputrequesttypedef).

Keyword-only arguments:

- `RequestToken`: `str` *(required)*

Returns a `Coroutine` for
[GetResourceRequestStatusOutputTypeDef](./type_defs.md#getresourcerequeststatusoutputtypedef).

<a id="list\_resource\_requests"></a>

### list_resource_requests

Returns existing resource operation requests.

Type annotations for
`session.create_client("cloudcontrol").list_resource_requests` method.

Boto3 documentation:
[CloudControlApi.Client.list_resource_requests](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.list_resource_requests)

Asynchronous method. Use `await list_resource_requests(...)` for a synchronous
call.

Arguments mapping described in
[ListResourceRequestsInputRequestTypeDef](./type_defs.md#listresourcerequestsinputrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`
- `ResourceRequestStatusFilter`:
  [ResourceRequestStatusFilterTypeDef](./type_defs.md#resourcerequeststatusfiltertypedef)

Returns a `Coroutine` for
[ListResourceRequestsOutputTypeDef](./type_defs.md#listresourcerequestsoutputtypedef).

<a id="list\_resources"></a>

### list_resources

Returns information about the specified resources.

Type annotations for `session.create_client("cloudcontrol").list_resources`
method.

Boto3 documentation:
[CloudControlApi.Client.list_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.list_resources)

Asynchronous method. Use `await list_resources(...)` for a synchronous call.

Arguments mapping described in
[ListResourcesInputRequestTypeDef](./type_defs.md#listresourcesinputrequesttypedef).

Keyword-only arguments:

- `TypeName`: `str` *(required)*
- `TypeVersionId`: `str`
- `RoleArn`: `str`
- `NextToken`: `str`
- `MaxResults`: `int`
- `ResourceModel`: `str`

Returns a `Coroutine` for
[ListResourcesOutputTypeDef](./type_defs.md#listresourcesoutputtypedef).

<a id="update\_resource"></a>

### update_resource

.

Type annotations for `session.create_client("cloudcontrol").update_resource`
method.

Boto3 documentation:
[CloudControlApi.Client.update_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.update_resource)

Asynchronous method. Use `await update_resource(...)` for a synchronous call.

Arguments mapping described in
[UpdateResourceInputRequestTypeDef](./type_defs.md#updateresourceinputrequesttypedef).

Keyword-only arguments:

- `TypeName`: `str` *(required)*
- `Identifier`: `str` *(required)*
- `PatchDocument`: `str` *(required)*
- `TypeVersionId`: `str`
- `RoleArn`: `str`
- `ClientToken`: `str`

Returns a `Coroutine` for
[UpdateResourceOutputTypeDef](./type_defs.md#updateresourceoutputtypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("cloudcontrol").__aenter__` method.

Boto3 documentation:
[CloudControlApi.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [CloudControlApiClient](#cloudcontrolapiclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("cloudcontrol").__aexit__` method.

Boto3 documentation:
[CloudControlApi.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("cloudcontrol").get_waiter` method
with overloads.

- `client.get_waiter("resource_request_success")` ->
  [ResourceRequestSuccessWaiter](./waiters.md#resourcerequestsuccesswaiter)
