# SyntheticsClient

> [Index](../README.md) > [Synthetics](./README.md) > SyntheticsClient

!!! note ""

    Auto-generated documentation for [Synthetics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#synthetics)
    type annotations stubs module [types-aiobotocore-synthetics](https://pypi.org/project/types-aiobotocore-synthetics/).

## SyntheticsClient

Type annotations and code completion for `#!python session.create_client("synthetics")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client)

```python
# SyntheticsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_synthetics.client import SyntheticsClient

session = get_session()
async with session.create_client("synthetics") as client:
    client: SyntheticsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("synthetics").exceptions` structure.

```python
# SyntheticsClient.exceptions usage example

async with session.create_client("synthetics") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.InternalFailureException,
        client.InternalServerException,
        client.NotFoundException,
        client.RequestEntityTooLargeException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.TooManyRequestsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# SyntheticsClient usage type checking example

from types_aiobotocore_synthetics.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("synthetics").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("synthetics").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/generate_presigned_url.html)

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


### associate\_resource

Associates a canary with a group.

Type annotations and code completion for `#!python session.create_client("synthetics").associate_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/associate_resource.html)

```python
# associate_resource method definition

await def associate_resource(
    self,
    *,
    GroupIdentifier: str,
    ResourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_resource method usage example with argument unpacking

kwargs: AssociateResourceRequestTypeDef = {  # (1)
    "GroupIdentifier": ...,
    "ResourceArn": ...,
}

parent.associate_resource(**kwargs)
```

1. See [:material-code-braces: AssociateResourceRequestTypeDef](./type_defs.md#associateresourcerequesttypedef) 

### create\_canary

Creates a canary.

Type annotations and code completion for `#!python session.create_client("synthetics").create_canary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/create_canary.html)

```python
# create_canary method definition

await def create_canary(
    self,
    *,
    Name: str,
    Code: CanaryCodeInputTypeDef,  # (1)
    ArtifactS3Location: str,
    ExecutionRoleArn: str,
    Schedule: CanaryScheduleInputTypeDef,  # (2)
    RuntimeVersion: str,
    RunConfig: CanaryRunConfigInputTypeDef = ...,  # (3)
    SuccessRetentionPeriodInDays: int = ...,
    FailureRetentionPeriodInDays: int = ...,
    VpcConfig: VpcConfigInputTypeDef = ...,  # (4)
    ResourcesToReplicateTags: Sequence[ResourceToTagType] = ...,  # (5)
    ProvisionedResourceCleanup: ProvisionedResourceCleanupSettingType = ...,  # (6)
    Tags: Mapping[str, str] = ...,
    ArtifactConfig: ArtifactConfigInputTypeDef = ...,  # (7)
) -> CreateCanaryResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: CanaryCodeInputTypeDef](./type_defs.md#canarycodeinputtypedef) 
2. See [:material-code-braces: CanaryScheduleInputTypeDef](./type_defs.md#canaryscheduleinputtypedef) 
3. See [:material-code-braces: CanaryRunConfigInputTypeDef](./type_defs.md#canaryrunconfiginputtypedef) 
4. See [:material-code-braces: VpcConfigInputTypeDef](./type_defs.md#vpcconfiginputtypedef) 
5. See [:material-code-brackets: ResourceToTagType](./literals.md#resourcetotagtype) 
6. See [:material-code-brackets: ProvisionedResourceCleanupSettingType](./literals.md#provisionedresourcecleanupsettingtype) 
7. See [:material-code-braces: ArtifactConfigInputTypeDef](./type_defs.md#artifactconfiginputtypedef) 
8. See [:material-code-braces: CreateCanaryResponseTypeDef](./type_defs.md#createcanaryresponsetypedef) 


```python
# create_canary method usage example with argument unpacking

kwargs: CreateCanaryRequestTypeDef = {  # (1)
    "Name": ...,
    "Code": ...,
    "ArtifactS3Location": ...,
    "ExecutionRoleArn": ...,
    "Schedule": ...,
    "RuntimeVersion": ...,
}

parent.create_canary(**kwargs)
```

1. See [:material-code-braces: CreateCanaryRequestTypeDef](./type_defs.md#createcanaryrequesttypedef) 

### create\_group

Creates a group which you can use to associate canaries with each other,
including cross-Region canaries.

Type annotations and code completion for `#!python session.create_client("synthetics").create_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/create_group.html)

```python
# create_group method definition

await def create_group(
    self,
    *,
    Name: str,
    Tags: Mapping[str, str] = ...,
) -> CreateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef) 


```python
# create_group method usage example with argument unpacking

kwargs: CreateGroupRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_group(**kwargs)
```

1. See [:material-code-braces: CreateGroupRequestTypeDef](./type_defs.md#creategrouprequesttypedef) 

### delete\_canary

Permanently deletes the specified canary.

Type annotations and code completion for `#!python session.create_client("synthetics").delete_canary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/delete_canary.html)

```python
# delete_canary method definition

await def delete_canary(
    self,
    *,
    Name: str,
    DeleteLambda: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_canary method usage example with argument unpacking

kwargs: DeleteCanaryRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_canary(**kwargs)
```

1. See [:material-code-braces: DeleteCanaryRequestTypeDef](./type_defs.md#deletecanaryrequesttypedef) 

### delete\_group

Deletes a group.

Type annotations and code completion for `#!python session.create_client("synthetics").delete_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/delete_group.html)

```python
# delete_group method definition

await def delete_group(
    self,
    *,
    GroupIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_group method usage example with argument unpacking

kwargs: DeleteGroupRequestTypeDef = {  # (1)
    "GroupIdentifier": ...,
}

parent.delete_group(**kwargs)
```

1. See [:material-code-braces: DeleteGroupRequestTypeDef](./type_defs.md#deletegrouprequesttypedef) 

### describe\_canaries

This operation returns a list of the canaries in your account, along with full
details about each canary.

Type annotations and code completion for `#!python session.create_client("synthetics").describe_canaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/describe_canaries.html)

```python
# describe_canaries method definition

await def describe_canaries(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Names: Sequence[str] = ...,
) -> DescribeCanariesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCanariesResponseTypeDef](./type_defs.md#describecanariesresponsetypedef) 


```python
# describe_canaries method usage example with argument unpacking

kwargs: DescribeCanariesRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.describe_canaries(**kwargs)
```

1. See [:material-code-braces: DescribeCanariesRequestTypeDef](./type_defs.md#describecanariesrequesttypedef) 

### describe\_canaries\_last\_run

Use this operation to see information from the most recent run of each canary
that you have created.

Type annotations and code completion for `#!python session.create_client("synthetics").describe_canaries_last_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/describe_canaries_last_run.html)

```python
# describe_canaries_last_run method definition

await def describe_canaries_last_run(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Names: Sequence[str] = ...,
) -> DescribeCanariesLastRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCanariesLastRunResponseTypeDef](./type_defs.md#describecanarieslastrunresponsetypedef) 


```python
# describe_canaries_last_run method usage example with argument unpacking

kwargs: DescribeCanariesLastRunRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.describe_canaries_last_run(**kwargs)
```

1. See [:material-code-braces: DescribeCanariesLastRunRequestTypeDef](./type_defs.md#describecanarieslastrunrequesttypedef) 

### describe\_runtime\_versions

Returns a list of Synthetics canary runtime versions.

Type annotations and code completion for `#!python session.create_client("synthetics").describe_runtime_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/describe_runtime_versions.html)

```python
# describe_runtime_versions method definition

await def describe_runtime_versions(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeRuntimeVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRuntimeVersionsResponseTypeDef](./type_defs.md#describeruntimeversionsresponsetypedef) 


```python
# describe_runtime_versions method usage example with argument unpacking

kwargs: DescribeRuntimeVersionsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.describe_runtime_versions(**kwargs)
```

1. See [:material-code-braces: DescribeRuntimeVersionsRequestTypeDef](./type_defs.md#describeruntimeversionsrequesttypedef) 

### disassociate\_resource

Removes a canary from a group.

Type annotations and code completion for `#!python session.create_client("synthetics").disassociate_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/disassociate_resource.html)

```python
# disassociate_resource method definition

await def disassociate_resource(
    self,
    *,
    GroupIdentifier: str,
    ResourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_resource method usage example with argument unpacking

kwargs: DisassociateResourceRequestTypeDef = {  # (1)
    "GroupIdentifier": ...,
    "ResourceArn": ...,
}

parent.disassociate_resource(**kwargs)
```

1. See [:material-code-braces: DisassociateResourceRequestTypeDef](./type_defs.md#disassociateresourcerequesttypedef) 

### get\_canary

Retrieves complete information about one canary.

Type annotations and code completion for `#!python session.create_client("synthetics").get_canary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/get_canary.html)

```python
# get_canary method definition

await def get_canary(
    self,
    *,
    Name: str,
) -> GetCanaryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCanaryResponseTypeDef](./type_defs.md#getcanaryresponsetypedef) 


```python
# get_canary method usage example with argument unpacking

kwargs: GetCanaryRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_canary(**kwargs)
```

1. See [:material-code-braces: GetCanaryRequestTypeDef](./type_defs.md#getcanaryrequesttypedef) 

### get\_canary\_runs

Retrieves a list of runs for a specified canary.

Type annotations and code completion for `#!python session.create_client("synthetics").get_canary_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/get_canary_runs.html)

```python
# get_canary_runs method definition

await def get_canary_runs(
    self,
    *,
    Name: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetCanaryRunsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCanaryRunsResponseTypeDef](./type_defs.md#getcanaryrunsresponsetypedef) 


```python
# get_canary_runs method usage example with argument unpacking

kwargs: GetCanaryRunsRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_canary_runs(**kwargs)
```

1. See [:material-code-braces: GetCanaryRunsRequestTypeDef](./type_defs.md#getcanaryrunsrequesttypedef) 

### get\_group

Returns information about one group.

Type annotations and code completion for `#!python session.create_client("synthetics").get_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/get_group.html)

```python
# get_group method definition

await def get_group(
    self,
    *,
    GroupIdentifier: str,
) -> GetGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef) 


```python
# get_group method usage example with argument unpacking

kwargs: GetGroupRequestTypeDef = {  # (1)
    "GroupIdentifier": ...,
}

parent.get_group(**kwargs)
```

1. See [:material-code-braces: GetGroupRequestTypeDef](./type_defs.md#getgrouprequesttypedef) 

### list\_associated\_groups

Returns a list of the groups that the specified canary is associated with.

Type annotations and code completion for `#!python session.create_client("synthetics").list_associated_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/list_associated_groups.html)

```python
# list_associated_groups method definition

await def list_associated_groups(
    self,
    *,
    ResourceArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAssociatedGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAssociatedGroupsResponseTypeDef](./type_defs.md#listassociatedgroupsresponsetypedef) 


```python
# list_associated_groups method usage example with argument unpacking

kwargs: ListAssociatedGroupsRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_associated_groups(**kwargs)
```

1. See [:material-code-braces: ListAssociatedGroupsRequestTypeDef](./type_defs.md#listassociatedgroupsrequesttypedef) 

### list\_group\_resources

This operation returns a list of the ARNs of the canaries that are associated
with the specified group.

Type annotations and code completion for `#!python session.create_client("synthetics").list_group_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/list_group_resources.html)

```python
# list_group_resources method definition

await def list_group_resources(
    self,
    *,
    GroupIdentifier: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListGroupResourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupResourcesResponseTypeDef](./type_defs.md#listgroupresourcesresponsetypedef) 


```python
# list_group_resources method usage example with argument unpacking

kwargs: ListGroupResourcesRequestTypeDef = {  # (1)
    "GroupIdentifier": ...,
}

parent.list_group_resources(**kwargs)
```

1. See [:material-code-braces: ListGroupResourcesRequestTypeDef](./type_defs.md#listgroupresourcesrequesttypedef) 

### list\_groups

Returns a list of all groups in the account, displaying their names, unique
IDs, and ARNs.

Type annotations and code completion for `#!python session.create_client("synthetics").list_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/list_groups.html)

```python
# list_groups method definition

await def list_groups(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python
# list_groups method usage example with argument unpacking

kwargs: ListGroupsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_groups(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestTypeDef](./type_defs.md#listgroupsrequesttypedef) 

### list\_tags\_for\_resource

Displays the tags associated with a canary or group.

Type annotations and code completion for `#!python session.create_client("synthetics").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### start\_canary

Use this operation to run a canary that has already been created.

Type annotations and code completion for `#!python session.create_client("synthetics").start_canary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/start_canary.html)

```python
# start_canary method definition

await def start_canary(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# start_canary method usage example with argument unpacking

kwargs: StartCanaryRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.start_canary(**kwargs)
```

1. See [:material-code-braces: StartCanaryRequestTypeDef](./type_defs.md#startcanaryrequesttypedef) 

### stop\_canary

Stops the canary to prevent all future runs.

Type annotations and code completion for `#!python session.create_client("synthetics").stop_canary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/stop_canary.html)

```python
# stop_canary method definition

await def stop_canary(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_canary method usage example with argument unpacking

kwargs: StopCanaryRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.stop_canary(**kwargs)
```

1. See [:material-code-braces: StopCanaryRequestTypeDef](./type_defs.md#stopcanaryrequesttypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified canary or group.

Type annotations and code completion for `#!python session.create_client("synthetics").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes one or more tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("synthetics").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_canary

Updates the configuration of a canary that has already been created.

Type annotations and code completion for `#!python session.create_client("synthetics").update_canary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics/client/update_canary.html)

```python
# update_canary method definition

await def update_canary(
    self,
    *,
    Name: str,
    Code: CanaryCodeInputTypeDef = ...,  # (1)
    ExecutionRoleArn: str = ...,
    RuntimeVersion: str = ...,
    Schedule: CanaryScheduleInputTypeDef = ...,  # (2)
    RunConfig: CanaryRunConfigInputTypeDef = ...,  # (3)
    SuccessRetentionPeriodInDays: int = ...,
    FailureRetentionPeriodInDays: int = ...,
    VpcConfig: VpcConfigInputTypeDef = ...,  # (4)
    VisualReference: VisualReferenceInputTypeDef = ...,  # (5)
    ArtifactS3Location: str = ...,
    ArtifactConfig: ArtifactConfigInputTypeDef = ...,  # (6)
    ProvisionedResourceCleanup: ProvisionedResourceCleanupSettingType = ...,  # (7)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: CanaryCodeInputTypeDef](./type_defs.md#canarycodeinputtypedef) 
2. See [:material-code-braces: CanaryScheduleInputTypeDef](./type_defs.md#canaryscheduleinputtypedef) 
3. See [:material-code-braces: CanaryRunConfigInputTypeDef](./type_defs.md#canaryrunconfiginputtypedef) 
4. See [:material-code-braces: VpcConfigInputTypeDef](./type_defs.md#vpcconfiginputtypedef) 
5. See [:material-code-braces: VisualReferenceInputTypeDef](./type_defs.md#visualreferenceinputtypedef) 
6. See [:material-code-braces: ArtifactConfigInputTypeDef](./type_defs.md#artifactconfiginputtypedef) 
7. See [:material-code-brackets: ProvisionedResourceCleanupSettingType](./literals.md#provisionedresourcecleanupsettingtype) 


```python
# update_canary method usage example with argument unpacking

kwargs: UpdateCanaryRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_canary(**kwargs)
```

1. See [:material-code-braces: UpdateCanaryRequestTypeDef](./type_defs.md#updatecanaryrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("synthetics").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("synthetics").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client)

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





