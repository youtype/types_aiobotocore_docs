# WorkspacesInstancesClient

> [Index](../README.md) > [WorkspacesInstances](./README.md) > WorkspacesInstancesClient

!!! note ""

    Auto-generated documentation for [WorkspacesInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances.html#workspacesinstances)
    type annotations stubs module [types-aiobotocore-workspaces-instances](https://pypi.org/project/types-aiobotocore-workspaces-instances/).

## WorkspacesInstancesClient

Type annotations and code completion for `#!python session.create_client("workspaces-instances")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances.html#WorkspacesInstances.Client)

```python
# WorkspacesInstancesClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_workspaces_instances.client import WorkspacesInstancesClient

session = get_session()
async with session.create_client("workspaces-instances") as client:
    client: WorkspacesInstancesClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("workspaces-instances").exceptions` structure.

```python
# WorkspacesInstancesClient.exceptions usage example

async with session.create_client("workspaces-instances") as client:
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
# WorkspacesInstancesClient usage type checking example

from types_aiobotocore_workspaces_instances.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("workspaces-instances").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("workspaces-instances").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/generate_presigned_url.html)

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


### associate\_volume

Attaches a volume to a WorkSpace Instance.

Type annotations and code completion for `#!python session.create_client("workspaces-instances").associate_volume` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/associate_volume.html)

```python
# associate_volume method definition

await def associate_volume(
    self,
    *,
    WorkspaceInstanceId: str,
    VolumeId: str,
    Device: str,
) -> dict[str, Any]:
    ...
```

```python
# associate_volume method usage example with argument unpacking

kwargs: AssociateVolumeRequestTypeDef = {  # (1)
    "WorkspaceInstanceId": ...,
    "VolumeId": ...,
    "Device": ...,
}

parent.associate_volume(**kwargs)
```

1. See [:material-code-braces: AssociateVolumeRequestTypeDef](./type_defs.md#associatevolumerequesttypedef)

### create\_volume

Creates a new volume for WorkSpace Instances.

Type annotations and code completion for `#!python session.create_client("workspaces-instances").create_volume` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/create_volume.html)

```python
# create_volume method definition

await def create_volume(
    self,
    *,
    AvailabilityZone: str,
    ClientToken: str = ...,
    Encrypted: bool = ...,
    Iops: int = ...,
    KmsKeyId: str = ...,
    SizeInGB: int = ...,
    SnapshotId: str = ...,
    TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,  # (1)
    Throughput: int = ...,
    VolumeType: VolumeTypeEnumType = ...,  # (2)
) -> CreateVolumeResponseTypeDef:  # (3)
    ...
```

1. See `Sequence[TagSpecificationTypeDef]`
2. See [:material-code-brackets: VolumeTypeEnumType](./literals.md#volumetypeenumtype)
3. See [:material-code-braces: CreateVolumeResponseTypeDef](./type_defs.md#createvolumeresponsetypedef)


```python
# create_volume method usage example with argument unpacking

kwargs: CreateVolumeRequestTypeDef = {  # (1)
    "AvailabilityZone": ...,
}

parent.create_volume(**kwargs)
```

1. See [:material-code-braces: CreateVolumeRequestTypeDef](./type_defs.md#createvolumerequesttypedef)

### create\_workspace\_instance

Launches a new WorkSpace Instance with specified configuration parameters,
enabling programmatic workspace deployment.

Type annotations and code completion for `#!python session.create_client("workspaces-instances").create_workspace_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/create_workspace_instance.html)

```python
# create_workspace_instance method definition

await def create_workspace_instance(
    self,
    *,
    ManagedInstance: ManagedInstanceRequestTypeDef,  # (1)
    ClientToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    BillingConfiguration: BillingConfigurationTypeDef = ...,  # (3)
) -> CreateWorkspaceInstanceResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ManagedInstanceRequestTypeDef](./type_defs.md#managedinstancerequesttypedef)
2. See `Sequence[TagTypeDef]`
3. See [:material-code-braces: BillingConfigurationTypeDef](./type_defs.md#billingconfigurationtypedef)
4. See [:material-code-braces: CreateWorkspaceInstanceResponseTypeDef](./type_defs.md#createworkspaceinstanceresponsetypedef)


```python
# create_workspace_instance method usage example with argument unpacking

kwargs: CreateWorkspaceInstanceRequestTypeDef = {  # (1)
    "ManagedInstance": ...,
}

parent.create_workspace_instance(**kwargs)
```

1. See [:material-code-braces: CreateWorkspaceInstanceRequestTypeDef](./type_defs.md#createworkspaceinstancerequesttypedef)

### delete\_volume

Deletes a specified volume.

Type annotations and code completion for `#!python session.create_client("workspaces-instances").delete_volume` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/delete_volume.html)

```python
# delete_volume method definition

await def delete_volume(
    self,
    *,
    VolumeId: str,
) -> dict[str, Any]:
    ...
```

```python
# delete_volume method usage example with argument unpacking

kwargs: DeleteVolumeRequestTypeDef = {  # (1)
    "VolumeId": ...,
}

parent.delete_volume(**kwargs)
```

1. See [:material-code-braces: DeleteVolumeRequestTypeDef](./type_defs.md#deletevolumerequesttypedef)

### delete\_workspace\_instance

Deletes the specified WorkSpace.

Type annotations and code completion for `#!python session.create_client("workspaces-instances").delete_workspace_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/delete_workspace_instance.html)

```python
# delete_workspace_instance method definition

await def delete_workspace_instance(
    self,
    *,
    WorkspaceInstanceId: str,
) -> dict[str, Any]:
    ...
```

```python
# delete_workspace_instance method usage example with argument unpacking

kwargs: DeleteWorkspaceInstanceRequestTypeDef = {  # (1)
    "WorkspaceInstanceId": ...,
}

parent.delete_workspace_instance(**kwargs)
```

1. See [:material-code-braces: DeleteWorkspaceInstanceRequestTypeDef](./type_defs.md#deleteworkspaceinstancerequesttypedef)

### disassociate\_volume

Detaches a volume from a WorkSpace Instance.

Type annotations and code completion for `#!python session.create_client("workspaces-instances").disassociate_volume` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/disassociate_volume.html)

```python
# disassociate_volume method definition

await def disassociate_volume(
    self,
    *,
    WorkspaceInstanceId: str,
    VolumeId: str,
    Device: str = ...,
    DisassociateMode: DisassociateModeEnumType = ...,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: DisassociateModeEnumType](./literals.md#disassociatemodeenumtype)


```python
# disassociate_volume method usage example with argument unpacking

kwargs: DisassociateVolumeRequestTypeDef = {  # (1)
    "WorkspaceInstanceId": ...,
    "VolumeId": ...,
}

parent.disassociate_volume(**kwargs)
```

1. See [:material-code-braces: DisassociateVolumeRequestTypeDef](./type_defs.md#disassociatevolumerequesttypedef)

### get\_workspace\_instance

Retrieves detailed information about a specific WorkSpace Instance.

Type annotations and code completion for `#!python session.create_client("workspaces-instances").get_workspace_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/get_workspace_instance.html)

```python
# get_workspace_instance method definition

await def get_workspace_instance(
    self,
    *,
    WorkspaceInstanceId: str,
) -> GetWorkspaceInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkspaceInstanceResponseTypeDef](./type_defs.md#getworkspaceinstanceresponsetypedef)


```python
# get_workspace_instance method usage example with argument unpacking

kwargs: GetWorkspaceInstanceRequestTypeDef = {  # (1)
    "WorkspaceInstanceId": ...,
}

parent.get_workspace_instance(**kwargs)
```

1. See [:material-code-braces: GetWorkspaceInstanceRequestTypeDef](./type_defs.md#getworkspaceinstancerequesttypedef)

### list\_instance\_types

Retrieves a list of instance types supported by Amazon WorkSpaces Instances,
enabling precise workspace infrastructure configuration.

Type annotations and code completion for `#!python session.create_client("workspaces-instances").list_instance_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/list_instance_types.html)

```python
# list_instance_types method definition

await def list_instance_types(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    InstanceConfigurationFilter: InstanceConfigurationFilterTypeDef = ...,  # (1)
) -> ListInstanceTypesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InstanceConfigurationFilterTypeDef](./type_defs.md#instanceconfigurationfiltertypedef)
2. See [:material-code-braces: ListInstanceTypesResponseTypeDef](./type_defs.md#listinstancetypesresponsetypedef)


```python
# list_instance_types method usage example with argument unpacking

kwargs: ListInstanceTypesRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_instance_types(**kwargs)
```

1. See [:material-code-braces: ListInstanceTypesRequestTypeDef](./type_defs.md#listinstancetypesrequesttypedef)

### list\_regions

Retrieves a list of AWS regions supported by Amazon WorkSpaces Instances,
enabling region discovery for workspace deployments.

Type annotations and code completion for `#!python session.create_client("workspaces-instances").list_regions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/list_regions.html)

```python
# list_regions method definition

await def list_regions(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListRegionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRegionsResponseTypeDef](./type_defs.md#listregionsresponsetypedef)


```python
# list_regions method usage example with argument unpacking

kwargs: ListRegionsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_regions(**kwargs)
```

1. See [:material-code-braces: ListRegionsRequestTypeDef](./type_defs.md#listregionsrequesttypedef)

### list\_tags\_for\_resource

Retrieves tags for a WorkSpace Instance.

Type annotations and code completion for `#!python session.create_client("workspaces-instances").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    WorkspaceInstanceId: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "WorkspaceInstanceId": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)

### list\_workspace\_instances

Retrieves a collection of WorkSpaces Instances based on specified filters.

Type annotations and code completion for `#!python session.create_client("workspaces-instances").list_workspace_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/list_workspace_instances.html)

```python
# list_workspace_instances method definition

await def list_workspace_instances(
    self,
    *,
    ProvisionStates: Sequence[ProvisionStateEnumType] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListWorkspaceInstancesResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[ProvisionStateEnumType]`
2. See [:material-code-braces: ListWorkspaceInstancesResponseTypeDef](./type_defs.md#listworkspaceinstancesresponsetypedef)


```python
# list_workspace_instances method usage example with argument unpacking

kwargs: ListWorkspaceInstancesRequestTypeDef = {  # (1)
    "ProvisionStates": ...,
}

parent.list_workspace_instances(**kwargs)
```

1. See [:material-code-braces: ListWorkspaceInstancesRequestTypeDef](./type_defs.md#listworkspaceinstancesrequesttypedef)

### tag\_resource

Adds tags to a WorkSpace Instance.

Type annotations and code completion for `#!python session.create_client("workspaces-instances").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    WorkspaceInstanceId: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See `Sequence[TagTypeDef]`


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "WorkspaceInstanceId": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### untag\_resource

Removes tags from a WorkSpace Instance.

Type annotations and code completion for `#!python session.create_client("workspaces-instances").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    WorkspaceInstanceId: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```

```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "WorkspaceInstanceId": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("workspaces-instances").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances.html#WorkspacesInstances.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("workspaces-instances").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances.html#WorkspacesInstances.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("workspaces-instances").get_paginator` method with overloads.

- `client.get_paginator("list_instance_types")` -> [ListInstanceTypesPaginator](./paginators.md#listinstancetypespaginator)
- `client.get_paginator("list_regions")` -> [ListRegionsPaginator](./paginators.md#listregionspaginator)
- `client.get_paginator("list_workspace_instances")` -> [ListWorkspaceInstancesPaginator](./paginators.md#listworkspaceinstancespaginator)



