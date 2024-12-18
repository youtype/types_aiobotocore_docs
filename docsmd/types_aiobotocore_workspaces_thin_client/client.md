# WorkSpacesThinClientClient

> [Index](../README.md) > [WorkSpacesThinClient](./README.md) > WorkSpacesThinClientClient

!!! note ""

    Auto-generated documentation for [WorkSpacesThinClient](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#workspacesthinclient)
    type annotations stubs module [types-aiobotocore-workspaces-thin-client](https://pypi.org/project/types-aiobotocore-workspaces-thin-client/).

## WorkSpacesThinClientClient

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client)

```python
# WorkSpacesThinClientClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_workspaces_thin_client.client import WorkSpacesThinClientClient

session = get_session()
async with session.create_client("workspaces-thin-client") as client:
    client: WorkSpacesThinClientClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("workspaces-thin-client").exceptions` structure.

```python
# WorkSpacesThinClientClient.exceptions usage example

async with session.create_client("workspaces-thin-client") as client:
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
# WorkSpacesThinClientClient usage type checking example

from types_aiobotocore_workspaces_thin_client.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/generate_presigned_url.html)

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


### close



Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_environment

Creates an environment for your thin client devices.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").create_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/create_environment.html)

```python
# create_environment method definition

await def create_environment(
    self,
    *,
    desktopArn: str,
    name: str = ...,
    desktopEndpoint: str = ...,
    softwareSetUpdateSchedule: SoftwareSetUpdateScheduleType = ...,  # (1)
    maintenanceWindow: MaintenanceWindowTypeDef = ...,  # (2)
    softwareSetUpdateMode: SoftwareSetUpdateModeType = ...,  # (3)
    desiredSoftwareSetId: str = ...,
    kmsKeyArn: str = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
    deviceCreationTags: Mapping[str, str] = ...,
) -> CreateEnvironmentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: SoftwareSetUpdateScheduleType](./literals.md#softwaresetupdatescheduletype) 
2. See [:material-code-braces: MaintenanceWindowTypeDef](./type_defs.md#maintenancewindowtypedef) 
3. See [:material-code-brackets: SoftwareSetUpdateModeType](./literals.md#softwaresetupdatemodetype) 
4. See [:material-code-braces: CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef) 


```python
# create_environment method usage example with argument unpacking

kwargs: CreateEnvironmentRequestRequestTypeDef = {  # (1)
    "desktopArn": ...,
}

parent.create_environment(**kwargs)
```

1. See [:material-code-braces: CreateEnvironmentRequestRequestTypeDef](./type_defs.md#createenvironmentrequestrequesttypedef) 

### delete\_device

Deletes a thin client device.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").delete_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/delete_device.html)

```python
# delete_device method definition

await def delete_device(
    self,
    *,
    id: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_device method usage example with argument unpacking

kwargs: DeleteDeviceRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_device(**kwargs)
```

1. See [:material-code-braces: DeleteDeviceRequestRequestTypeDef](./type_defs.md#deletedevicerequestrequesttypedef) 

### delete\_environment

Deletes an environment.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").delete_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/delete_environment.html)

```python
# delete_environment method definition

await def delete_environment(
    self,
    *,
    id: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_environment method usage example with argument unpacking

kwargs: DeleteEnvironmentRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_environment(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentRequestRequestTypeDef](./type_defs.md#deleteenvironmentrequestrequesttypedef) 

### deregister\_device

Deregisters a thin client device.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").deregister_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/deregister_device.html)

```python
# deregister_device method definition

await def deregister_device(
    self,
    *,
    id: str,
    targetDeviceStatus: TargetDeviceStatusType = ...,  # (1)
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: TargetDeviceStatusType](./literals.md#targetdevicestatustype) 


```python
# deregister_device method usage example with argument unpacking

kwargs: DeregisterDeviceRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.deregister_device(**kwargs)
```

1. See [:material-code-braces: DeregisterDeviceRequestRequestTypeDef](./type_defs.md#deregisterdevicerequestrequesttypedef) 

### get\_device

Returns information for a thin client device.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").get_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/get_device.html)

```python
# get_device method definition

await def get_device(
    self,
    *,
    id: str,
) -> GetDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeviceResponseTypeDef](./type_defs.md#getdeviceresponsetypedef) 


```python
# get_device method usage example with argument unpacking

kwargs: GetDeviceRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_device(**kwargs)
```

1. See [:material-code-braces: GetDeviceRequestRequestTypeDef](./type_defs.md#getdevicerequestrequesttypedef) 

### get\_environment

Returns information for an environment.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").get_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/get_environment.html)

```python
# get_environment method definition

await def get_environment(
    self,
    *,
    id: str,
) -> GetEnvironmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnvironmentResponseTypeDef](./type_defs.md#getenvironmentresponsetypedef) 


```python
# get_environment method usage example with argument unpacking

kwargs: GetEnvironmentRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_environment(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentRequestRequestTypeDef](./type_defs.md#getenvironmentrequestrequesttypedef) 

### get\_software\_set

Returns information for a software set.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").get_software_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/get_software_set.html)

```python
# get_software_set method definition

await def get_software_set(
    self,
    *,
    id: str,
) -> GetSoftwareSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSoftwareSetResponseTypeDef](./type_defs.md#getsoftwaresetresponsetypedef) 


```python
# get_software_set method usage example with argument unpacking

kwargs: GetSoftwareSetRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_software_set(**kwargs)
```

1. See [:material-code-braces: GetSoftwareSetRequestRequestTypeDef](./type_defs.md#getsoftwaresetrequestrequesttypedef) 

### list\_devices

Returns a list of thin client devices.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").list_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/list_devices.html)

```python
# list_devices method definition

await def list_devices(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDevicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef) 


```python
# list_devices method usage example with argument unpacking

kwargs: ListDevicesRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_devices(**kwargs)
```

1. See [:material-code-braces: ListDevicesRequestRequestTypeDef](./type_defs.md#listdevicesrequestrequesttypedef) 

### list\_environments

Returns a list of environments.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").list_environments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/list_environments.html)

```python
# list_environments method definition

await def list_environments(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListEnvironmentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef) 


```python
# list_environments method usage example with argument unpacking

kwargs: ListEnvironmentsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_environments(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsRequestRequestTypeDef](./type_defs.md#listenvironmentsrequestrequesttypedef) 

### list\_software\_sets

Returns a list of software sets.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").list_software_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/list_software_sets.html)

```python
# list_software_sets method definition

await def list_software_sets(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListSoftwareSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSoftwareSetsResponseTypeDef](./type_defs.md#listsoftwaresetsresponsetypedef) 


```python
# list_software_sets method usage example with argument unpacking

kwargs: ListSoftwareSetsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_software_sets(**kwargs)
```

1. See [:material-code-braces: ListSoftwareSetsRequestRequestTypeDef](./type_defs.md#listsoftwaresetsrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags for a resource.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/list_tags_for_resource.html)

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

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified resource.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/tag_resource.html)

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

Removes a tag or tags from a resource.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/untag_resource.html)

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

### update\_device

Updates a thin client device.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").update_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/update_device.html)

```python
# update_device method definition

await def update_device(
    self,
    *,
    id: str,
    name: str = ...,
    desiredSoftwareSetId: str = ...,
    softwareSetUpdateSchedule: SoftwareSetUpdateScheduleType = ...,  # (1)
) -> UpdateDeviceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SoftwareSetUpdateScheduleType](./literals.md#softwaresetupdatescheduletype) 
2. See [:material-code-braces: UpdateDeviceResponseTypeDef](./type_defs.md#updatedeviceresponsetypedef) 


```python
# update_device method usage example with argument unpacking

kwargs: UpdateDeviceRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.update_device(**kwargs)
```

1. See [:material-code-braces: UpdateDeviceRequestRequestTypeDef](./type_defs.md#updatedevicerequestrequesttypedef) 

### update\_environment

Updates an environment.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").update_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/update_environment.html)

```python
# update_environment method definition

await def update_environment(
    self,
    *,
    id: str,
    name: str = ...,
    desktopArn: str = ...,
    desktopEndpoint: str = ...,
    softwareSetUpdateSchedule: SoftwareSetUpdateScheduleType = ...,  # (1)
    maintenanceWindow: MaintenanceWindowTypeDef = ...,  # (2)
    softwareSetUpdateMode: SoftwareSetUpdateModeType = ...,  # (3)
    desiredSoftwareSetId: str = ...,
    deviceCreationTags: Mapping[str, str] = ...,
) -> UpdateEnvironmentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: SoftwareSetUpdateScheduleType](./literals.md#softwaresetupdatescheduletype) 
2. See [:material-code-braces: MaintenanceWindowTypeDef](./type_defs.md#maintenancewindowtypedef) 
3. See [:material-code-brackets: SoftwareSetUpdateModeType](./literals.md#softwaresetupdatemodetype) 
4. See [:material-code-braces: UpdateEnvironmentResponseTypeDef](./type_defs.md#updateenvironmentresponsetypedef) 


```python
# update_environment method usage example with argument unpacking

kwargs: UpdateEnvironmentRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.update_environment(**kwargs)
```

1. See [:material-code-braces: UpdateEnvironmentRequestRequestTypeDef](./type_defs.md#updateenvironmentrequestrequesttypedef) 

### update\_software\_set

Updates a software set.

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").update_software_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client/client/update_software_set.html)

```python
# update_software_set method definition

await def update_software_set(
    self,
    *,
    id: str,
    validationStatus: SoftwareSetValidationStatusType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: SoftwareSetValidationStatusType](./literals.md#softwaresetvalidationstatustype) 


```python
# update_software_set method usage example with argument unpacking

kwargs: UpdateSoftwareSetRequestRequestTypeDef = {  # (1)
    "id": ...,
    "validationStatus": ...,
}

parent.update_software_set(**kwargs)
```

1. See [:material-code-braces: UpdateSoftwareSetRequestRequestTypeDef](./type_defs.md#updatesoftwaresetrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "WorkSpacesThinClientClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client)

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

Type annotations and code completion for `#!python session.create_client("workspaces-thin-client").get_paginator` method with overloads.

- `client.get_paginator("list_devices")` -> [ListDevicesPaginator](./paginators.md#listdevicespaginator)
- `client.get_paginator("list_environments")` -> [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
- `client.get_paginator("list_software_sets")` -> [ListSoftwareSetsPaginator](./paginators.md#listsoftwaresetspaginator)



