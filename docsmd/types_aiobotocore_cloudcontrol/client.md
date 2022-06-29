# CloudControlApiClient

> [Index](../README.md) > [CloudControlApi](./README.md) > CloudControlApiClient

!!! note ""

    Auto-generated documentation for [CloudControlApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
    type annotations stubs module [types-aiobotocore-cloudcontrol](https://pypi.org/project/types-aiobotocore-cloudcontrol/).

## CloudControlApiClient

Type annotations and code completion for `#!python session.create_client("cloudcontrol")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_cloudcontrol.client import CloudControlApiClient

session = get_session()
async with session.create_client("cloudcontrol") as client:
    client: CloudControlApiClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cloudcontrol").exceptions` structure.

```python title="Usage example"
async with session.create_client("cloudcontrol") as client:
    try:
        do_something(client)
    except (
            client.AlreadyExistsException,
        client.ClientError,
        client.ClientTokenConflictException,
        client.ConcurrentModificationException,
        client.ConcurrentOperationException,
        client.GeneralServiceException,
        client.HandlerFailureException,
        client.HandlerInternalFailureException,
        client.InvalidCredentialsException,
        client.InvalidRequestException,
        client.NetworkFailureException,
        client.NotStabilizedException,
        client.NotUpdatableException,
        client.PrivateTypeException,
        client.RequestTokenNotFoundException,
        client.ResourceConflictException,
        client.ResourceNotFoundException,
        client.ServiceInternalErrorException,
        client.ServiceLimitExceededException,
        client.ThrottlingException,
        client.TypeNotFoundException,
        client.UnsupportedActionException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_cloudcontrol.client import Exceptions

def handle_error(exc: Exceptions.AlreadyExistsException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("cloudcontrol").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_resource\_request

Cancels the specified resource operation request.

Type annotations and code completion for `#!python session.create_client("cloudcontrol").cancel_resource_request` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.cancel_resource_request)

```python title="Method definition"
await def cancel_resource_request(
    self,
    *,
    RequestToken: str,
) -> CancelResourceRequestOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelResourceRequestOutputTypeDef](./type_defs.md#cancelresourcerequestoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: CancelResourceRequestInputRequestTypeDef = {  # (1)
    "RequestToken": ...,
}

parent.cancel_resource_request(**kwargs)
```

1. See [:material-code-braces: CancelResourceRequestInputRequestTypeDef](./type_defs.md#cancelresourcerequestinputrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("cloudcontrol").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### create\_resource

Creates the specified resource.

Type annotations and code completion for `#!python session.create_client("cloudcontrol").create_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.create_resource)

```python title="Method definition"
await def create_resource(
    self,
    *,
    TypeName: str,
    DesiredState: str,
    TypeVersionId: str = ...,
    RoleArn: str = ...,
    ClientToken: str = ...,
) -> CreateResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateResourceOutputTypeDef](./type_defs.md#createresourceoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: CreateResourceInputRequestTypeDef = {  # (1)
    "TypeName": ...,
    "DesiredState": ...,
}

parent.create_resource(**kwargs)
```

1. See [:material-code-braces: CreateResourceInputRequestTypeDef](./type_defs.md#createresourceinputrequesttypedef) 

### delete\_resource

Deletes the specified resource.

Type annotations and code completion for `#!python session.create_client("cloudcontrol").delete_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.delete_resource)

```python title="Method definition"
await def delete_resource(
    self,
    *,
    TypeName: str,
    Identifier: str,
    TypeVersionId: str = ...,
    RoleArn: str = ...,
    ClientToken: str = ...,
) -> DeleteResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteResourceOutputTypeDef](./type_defs.md#deleteresourceoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DeleteResourceInputRequestTypeDef = {  # (1)
    "TypeName": ...,
    "Identifier": ...,
}

parent.delete_resource(**kwargs)
```

1. See [:material-code-braces: DeleteResourceInputRequestTypeDef](./type_defs.md#deleteresourceinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("cloudcontrol").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_resource

Returns information about the current state of the specified resource.

Type annotations and code completion for `#!python session.create_client("cloudcontrol").get_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.get_resource)

```python title="Method definition"
await def get_resource(
    self,
    *,
    TypeName: str,
    Identifier: str,
    TypeVersionId: str = ...,
    RoleArn: str = ...,
) -> GetResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourceOutputTypeDef](./type_defs.md#getresourceoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: GetResourceInputRequestTypeDef = {  # (1)
    "TypeName": ...,
    "Identifier": ...,
}

parent.get_resource(**kwargs)
```

1. See [:material-code-braces: GetResourceInputRequestTypeDef](./type_defs.md#getresourceinputrequesttypedef) 

### get\_resource\_request\_status

Returns the current status of a resource operation request.

Type annotations and code completion for `#!python session.create_client("cloudcontrol").get_resource_request_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.get_resource_request_status)

```python title="Method definition"
await def get_resource_request_status(
    self,
    *,
    RequestToken: str,
) -> GetResourceRequestStatusOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourceRequestStatusOutputTypeDef](./type_defs.md#getresourcerequeststatusoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: GetResourceRequestStatusInputRequestTypeDef = {  # (1)
    "RequestToken": ...,
}

parent.get_resource_request_status(**kwargs)
```

1. See [:material-code-braces: GetResourceRequestStatusInputRequestTypeDef](./type_defs.md#getresourcerequeststatusinputrequesttypedef) 

### list\_resource\_requests

Returns existing resource operation requests.

Type annotations and code completion for `#!python session.create_client("cloudcontrol").list_resource_requests` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.list_resource_requests)

```python title="Method definition"
await def list_resource_requests(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...,  # (1)
) -> ListResourceRequestsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceRequestStatusFilterTypeDef](./type_defs.md#resourcerequeststatusfiltertypedef) 
2. See [:material-code-braces: ListResourceRequestsOutputTypeDef](./type_defs.md#listresourcerequestsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListResourceRequestsInputRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_resource_requests(**kwargs)
```

1. See [:material-code-braces: ListResourceRequestsInputRequestTypeDef](./type_defs.md#listresourcerequestsinputrequesttypedef) 

### list\_resources

Returns information about the specified resources.

Type annotations and code completion for `#!python session.create_client("cloudcontrol").list_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.list_resources)

```python title="Method definition"
await def list_resources(
    self,
    *,
    TypeName: str,
    TypeVersionId: str = ...,
    RoleArn: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    ResourceModel: str = ...,
) -> ListResourcesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResourcesOutputTypeDef](./type_defs.md#listresourcesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListResourcesInputRequestTypeDef = {  # (1)
    "TypeName": ...,
}

parent.list_resources(**kwargs)
```

1. See [:material-code-braces: ListResourcesInputRequestTypeDef](./type_defs.md#listresourcesinputrequesttypedef) 

### update\_resource

.

Type annotations and code completion for `#!python session.create_client("cloudcontrol").update_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.update_resource)

```python title="Method definition"
await def update_resource(
    self,
    *,
    TypeName: str,
    Identifier: str,
    PatchDocument: str,
    TypeVersionId: str = ...,
    RoleArn: str = ...,
    ClientToken: str = ...,
) -> UpdateResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateResourceOutputTypeDef](./type_defs.md#updateresourceoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: UpdateResourceInputRequestTypeDef = {  # (1)
    "TypeName": ...,
    "Identifier": ...,
    "PatchDocument": ...,
}

parent.update_resource(**kwargs)
```

1. See [:material-code-braces: UpdateResourceInputRequestTypeDef](./type_defs.md#updateresourceinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cloudcontrol").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> CloudControlApiClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cloudcontrol").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("cloudcontrol").get_paginator` method with overloads.

- `client.get_paginator("list_resource_requests")` -> [ListResourceRequestsPaginator](./paginators.md#listresourcerequestspaginator)
- `client.get_paginator("list_resources")` -> [ListResourcesPaginator](./paginators.md#listresourcespaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("cloudcontrol").get_waiter` method with overloads.

- `client.get_waiter("resource_request_success")` -> [ResourceRequestSuccessWaiter](./waiters.md#resourcerequestsuccesswaiter)

