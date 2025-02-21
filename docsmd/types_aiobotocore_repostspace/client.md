# RePostPrivateClient

> [Index](../README.md) > [RePostPrivate](./README.md) > RePostPrivateClient

!!! note ""

    Auto-generated documentation for [RePostPrivate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace.html#repostprivate)
    type annotations stubs module [types-aiobotocore-repostspace](https://pypi.org/project/types-aiobotocore-repostspace/).

## RePostPrivateClient

Type annotations and code completion for `#!python session.create_client("repostspace")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace.html#RePostPrivate.Client)

```python
# RePostPrivateClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_repostspace.client import RePostPrivateClient

session = get_session()
async with session.create_client("repostspace") as client:
    client: RePostPrivateClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("repostspace").exceptions` structure.

```python
# RePostPrivateClient.exceptions usage example

async with session.create_client("repostspace") as client:
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
# RePostPrivateClient usage type checking example

from types_aiobotocore_repostspace.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("repostspace").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("repostspace").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/generate_presigned_url.html)

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


### batch\_add\_role

Add role to multiple users or groups in a private re:Post.

Type annotations and code completion for `#!python session.create_client("repostspace").batch_add_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/batch_add_role.html)

```python
# batch_add_role method definition

await def batch_add_role(
    self,
    *,
    accessorIds: Sequence[str],
    role: RoleType,  # (1)
    spaceId: str,
) -> BatchAddRoleOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
2. See [:material-code-braces: BatchAddRoleOutputTypeDef](./type_defs.md#batchaddroleoutputtypedef) 


```python
# batch_add_role method usage example with argument unpacking

kwargs: BatchAddRoleInputTypeDef = {  # (1)
    "accessorIds": ...,
    "role": ...,
    "spaceId": ...,
}

parent.batch_add_role(**kwargs)
```

1. See [:material-code-braces: BatchAddRoleInputTypeDef](./type_defs.md#batchaddroleinputtypedef) 

### batch\_remove\_role

Remove role from multiple users or groups in a private re:Post.

Type annotations and code completion for `#!python session.create_client("repostspace").batch_remove_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/batch_remove_role.html)

```python
# batch_remove_role method definition

await def batch_remove_role(
    self,
    *,
    accessorIds: Sequence[str],
    role: RoleType,  # (1)
    spaceId: str,
) -> BatchRemoveRoleOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
2. See [:material-code-braces: BatchRemoveRoleOutputTypeDef](./type_defs.md#batchremoveroleoutputtypedef) 


```python
# batch_remove_role method usage example with argument unpacking

kwargs: BatchRemoveRoleInputTypeDef = {  # (1)
    "accessorIds": ...,
    "role": ...,
    "spaceId": ...,
}

parent.batch_remove_role(**kwargs)
```

1. See [:material-code-braces: BatchRemoveRoleInputTypeDef](./type_defs.md#batchremoveroleinputtypedef) 

### create\_space

Creates an AWS re:Post Private private re:Post.

Type annotations and code completion for `#!python session.create_client("repostspace").create_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/create_space.html)

```python
# create_space method definition

await def create_space(
    self,
    *,
    name: str,
    subdomain: str,
    tier: TierLevelType,  # (1)
    description: str = ...,
    roleArn: str = ...,
    tags: Mapping[str, str] = ...,
    userKMSKey: str = ...,
) -> CreateSpaceOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TierLevelType](./literals.md#tierleveltype) 
2. See [:material-code-braces: CreateSpaceOutputTypeDef](./type_defs.md#createspaceoutputtypedef) 


```python
# create_space method usage example with argument unpacking

kwargs: CreateSpaceInputTypeDef = {  # (1)
    "name": ...,
    "subdomain": ...,
    "tier": ...,
}

parent.create_space(**kwargs)
```

1. See [:material-code-braces: CreateSpaceInputTypeDef](./type_defs.md#createspaceinputtypedef) 

### delete\_space

Deletes an AWS re:Post Private private re:Post.

Type annotations and code completion for `#!python session.create_client("repostspace").delete_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/delete_space.html)

```python
# delete_space method definition

await def delete_space(
    self,
    *,
    spaceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_space method usage example with argument unpacking

kwargs: DeleteSpaceInputTypeDef = {  # (1)
    "spaceId": ...,
}

parent.delete_space(**kwargs)
```

1. See [:material-code-braces: DeleteSpaceInputTypeDef](./type_defs.md#deletespaceinputtypedef) 

### deregister\_admin

Removes the user or group from the list of administrators of the private
re:Post.

Type annotations and code completion for `#!python session.create_client("repostspace").deregister_admin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/deregister_admin.html)

```python
# deregister_admin method definition

await def deregister_admin(
    self,
    *,
    adminId: str,
    spaceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# deregister_admin method usage example with argument unpacking

kwargs: DeregisterAdminInputTypeDef = {  # (1)
    "adminId": ...,
    "spaceId": ...,
}

parent.deregister_admin(**kwargs)
```

1. See [:material-code-braces: DeregisterAdminInputTypeDef](./type_defs.md#deregisteradmininputtypedef) 

### get\_space

Displays information about the AWS re:Post Private private re:Post.

Type annotations and code completion for `#!python session.create_client("repostspace").get_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/get_space.html)

```python
# get_space method definition

await def get_space(
    self,
    *,
    spaceId: str,
) -> GetSpaceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSpaceOutputTypeDef](./type_defs.md#getspaceoutputtypedef) 


```python
# get_space method usage example with argument unpacking

kwargs: GetSpaceInputTypeDef = {  # (1)
    "spaceId": ...,
}

parent.get_space(**kwargs)
```

1. See [:material-code-braces: GetSpaceInputTypeDef](./type_defs.md#getspaceinputtypedef) 

### list\_spaces

Returns a list of AWS re:Post Private private re:Posts in the account with some
information about each private re:Post.

Type annotations and code completion for `#!python session.create_client("repostspace").list_spaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/list_spaces.html)

```python
# list_spaces method definition

await def list_spaces(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSpacesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSpacesOutputTypeDef](./type_defs.md#listspacesoutputtypedef) 


```python
# list_spaces method usage example with argument unpacking

kwargs: ListSpacesInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_spaces(**kwargs)
```

1. See [:material-code-braces: ListSpacesInputTypeDef](./type_defs.md#listspacesinputtypedef) 

### list\_tags\_for\_resource

Returns the tags that are associated with the AWS re:Post Private resource
specified by the resourceArn.

Type annotations and code completion for `#!python session.create_client("repostspace").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/list_tags_for_resource.html)

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

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### register\_admin

Adds a user or group to the list of administrators of the private re:Post.

Type annotations and code completion for `#!python session.create_client("repostspace").register_admin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/register_admin.html)

```python
# register_admin method definition

await def register_admin(
    self,
    *,
    adminId: str,
    spaceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# register_admin method usage example with argument unpacking

kwargs: RegisterAdminInputTypeDef = {  # (1)
    "adminId": ...,
    "spaceId": ...,
}

parent.register_admin(**kwargs)
```

1. See [:material-code-braces: RegisterAdminInputTypeDef](./type_defs.md#registeradmininputtypedef) 

### send\_invites

Sends an invitation email to selected users and groups.

Type annotations and code completion for `#!python session.create_client("repostspace").send_invites` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/send_invites.html)

```python
# send_invites method definition

await def send_invites(
    self,
    *,
    accessorIds: Sequence[str],
    body: str,
    spaceId: str,
    title: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# send_invites method usage example with argument unpacking

kwargs: SendInvitesInputTypeDef = {  # (1)
    "accessorIds": ...,
    "body": ...,
    "spaceId": ...,
    "title": ...,
}

parent.send_invites(**kwargs)
```

1. See [:material-code-braces: SendInvitesInputTypeDef](./type_defs.md#sendinvitesinputtypedef) 

### tag\_resource

Associates tags with an AWS re:Post Private resource.

Type annotations and code completion for `#!python session.create_client("repostspace").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/tag_resource.html)

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

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes the association of the tag with the AWS re:Post Private resource.

Type annotations and code completion for `#!python session.create_client("repostspace").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/untag_resource.html)

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

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_space

Modifies an existing AWS re:Post Private private re:Post.

Type annotations and code completion for `#!python session.create_client("repostspace").update_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace/client/update_space.html)

```python
# update_space method definition

await def update_space(
    self,
    *,
    spaceId: str,
    description: str = ...,
    roleArn: str = ...,
    tier: TierLevelType = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TierLevelType](./literals.md#tierleveltype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_space method usage example with argument unpacking

kwargs: UpdateSpaceInputTypeDef = {  # (1)
    "spaceId": ...,
}

parent.update_space(**kwargs)
```

1. See [:material-code-braces: UpdateSpaceInputTypeDef](./type_defs.md#updatespaceinputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("repostspace").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace.html#RePostPrivate.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("repostspace").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace.html#RePostPrivate.Client)

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

Type annotations and code completion for `#!python session.create_client("repostspace").get_paginator` method with overloads.

- `client.get_paginator("list_spaces")` -> [ListSpacesPaginator](./paginators.md#listspacespaginator)



