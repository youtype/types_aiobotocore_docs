# AIOpsClient

> [Index](../README.md) > [AIOps](./README.md) > AIOpsClient

!!! note ""

    Auto-generated documentation for [AIOps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops.html#aiops)
    type annotations stubs module [types-aiobotocore-aiops](https://pypi.org/project/types-aiobotocore-aiops/).

## AIOpsClient

Type annotations and code completion for `#!python session.create_client("aiops")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops.html#AIOps.Client)

```python
# AIOpsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_aiops.client import AIOpsClient

session = get_session()
async with session.create_client("aiops") as client:
    client: AIOpsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("aiops").exceptions` structure.

```python
# AIOpsClient.exceptions usage example

async with session.create_client("aiops") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.ForbiddenException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# AIOpsClient usage type checking example

from types_aiobotocore_aiops.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("aiops").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("aiops").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/client/generate_presigned_url.html)

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


### create\_investigation\_group

Creates an <i>investigation group</i> in your account.

Type annotations and code completion for `#!python session.create_client("aiops").create_investigation_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/client/create_investigation_group.html)

```python
# create_investigation_group method definition

await def create_investigation_group(
    self,
    *,
    name: str,
    roleArn: str,
    encryptionConfiguration: EncryptionConfigurationTypeDef = ...,  # (1)
    retentionInDays: int = ...,
    tags: Mapping[str, str] = ...,
    tagKeyBoundaries: Sequence[str] = ...,
    chatbotNotificationChannel: Mapping[str, Sequence[str]] = ...,
    isCloudTrailEventHistoryEnabled: bool = ...,
    crossAccountConfigurations: Sequence[CrossAccountConfigurationTypeDef] = ...,  # (2)
) -> CreateInvestigationGroupOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
2. See `Sequence[CrossAccountConfigurationTypeDef]`
3. See [:material-code-braces: CreateInvestigationGroupOutputTypeDef](./type_defs.md#createinvestigationgroupoutputtypedef)


```python
# create_investigation_group method usage example with argument unpacking

kwargs: CreateInvestigationGroupInputTypeDef = {  # (1)
    "name": ...,
    "roleArn": ...,
}

parent.create_investigation_group(**kwargs)
```

1. See [:material-code-braces: CreateInvestigationGroupInputTypeDef](./type_defs.md#createinvestigationgroupinputtypedef)

### delete\_investigation\_group

Deletes the specified investigation group from your account.

Type annotations and code completion for `#!python session.create_client("aiops").delete_investigation_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/client/delete_investigation_group.html)

```python
# delete_investigation_group method definition

await def delete_investigation_group(
    self,
    *,
    identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_investigation_group method usage example with argument unpacking

kwargs: DeleteInvestigationGroupRequestTypeDef = {  # (1)
    "identifier": ...,
}

parent.delete_investigation_group(**kwargs)
```

1. See [:material-code-braces: DeleteInvestigationGroupRequestTypeDef](./type_defs.md#deleteinvestigationgrouprequesttypedef)

### delete\_investigation\_group\_policy

Removes the IAM resource policy from being associated with the investigation
group that you specify.

Type annotations and code completion for `#!python session.create_client("aiops").delete_investigation_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/client/delete_investigation_group_policy.html)

```python
# delete_investigation_group_policy method definition

await def delete_investigation_group_policy(
    self,
    *,
    identifier: str,
) -> dict[str, Any]:
    ...
```

```python
# delete_investigation_group_policy method usage example with argument unpacking

kwargs: DeleteInvestigationGroupPolicyRequestTypeDef = {  # (1)
    "identifier": ...,
}

parent.delete_investigation_group_policy(**kwargs)
```

1. See [:material-code-braces: DeleteInvestigationGroupPolicyRequestTypeDef](./type_defs.md#deleteinvestigationgrouppolicyrequesttypedef)

### get\_investigation\_group

Returns the configuration information for the specified investigation group.

Type annotations and code completion for `#!python session.create_client("aiops").get_investigation_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/client/get_investigation_group.html)

```python
# get_investigation_group method definition

await def get_investigation_group(
    self,
    *,
    identifier: str,
) -> GetInvestigationGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInvestigationGroupResponseTypeDef](./type_defs.md#getinvestigationgroupresponsetypedef)


```python
# get_investigation_group method usage example with argument unpacking

kwargs: GetInvestigationGroupRequestTypeDef = {  # (1)
    "identifier": ...,
}

parent.get_investigation_group(**kwargs)
```

1. See [:material-code-braces: GetInvestigationGroupRequestTypeDef](./type_defs.md#getinvestigationgrouprequesttypedef)

### get\_investigation\_group\_policy

Returns the JSON of the IAM resource policy associated with the specified
investigation group in a string.

Type annotations and code completion for `#!python session.create_client("aiops").get_investigation_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/client/get_investigation_group_policy.html)

```python
# get_investigation_group_policy method definition

await def get_investigation_group_policy(
    self,
    *,
    identifier: str,
) -> GetInvestigationGroupPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInvestigationGroupPolicyResponseTypeDef](./type_defs.md#getinvestigationgrouppolicyresponsetypedef)


```python
# get_investigation_group_policy method usage example with argument unpacking

kwargs: GetInvestigationGroupPolicyRequestTypeDef = {  # (1)
    "identifier": ...,
}

parent.get_investigation_group_policy(**kwargs)
```

1. See [:material-code-braces: GetInvestigationGroupPolicyRequestTypeDef](./type_defs.md#getinvestigationgrouppolicyrequesttypedef)

### list\_investigation\_groups

Returns the ARN and name of each investigation group in the account.

Type annotations and code completion for `#!python session.create_client("aiops").list_investigation_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/client/list_investigation_groups.html)

```python
# list_investigation_groups method definition

await def list_investigation_groups(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListInvestigationGroupsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInvestigationGroupsOutputTypeDef](./type_defs.md#listinvestigationgroupsoutputtypedef)


```python
# list_investigation_groups method usage example with argument unpacking

kwargs: ListInvestigationGroupsInputTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_investigation_groups(**kwargs)
```

1. See [:material-code-braces: ListInvestigationGroupsInputTypeDef](./type_defs.md#listinvestigationgroupsinputtypedef)

### list\_tags\_for\_resource

Displays the tags associated with a CloudWatch investigations resource.

Type annotations and code completion for `#!python session.create_client("aiops").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/client/list_tags_for_resource.html)

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

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)

### put\_investigation\_group\_policy

Creates an IAM resource policy and assigns it to the specified investigation
group.

Type annotations and code completion for `#!python session.create_client("aiops").put_investigation_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/client/put_investigation_group_policy.html)

```python
# put_investigation_group_policy method definition

await def put_investigation_group_policy(
    self,
    *,
    identifier: str,
    policy: str,
) -> PutInvestigationGroupPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutInvestigationGroupPolicyResponseTypeDef](./type_defs.md#putinvestigationgrouppolicyresponsetypedef)


```python
# put_investigation_group_policy method usage example with argument unpacking

kwargs: PutInvestigationGroupPolicyRequestTypeDef = {  # (1)
    "identifier": ...,
    "policy": ...,
}

parent.put_investigation_group_policy(**kwargs)
```

1. See [:material-code-braces: PutInvestigationGroupPolicyRequestTypeDef](./type_defs.md#putinvestigationgrouppolicyrequesttypedef)

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified resource.

Type annotations and code completion for `#!python session.create_client("aiops").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> dict[str, Any]:
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

Removes one or more tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("aiops").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> dict[str, Any]:
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

### update\_investigation\_group

Updates the configuration of the specified investigation group.

Type annotations and code completion for `#!python session.create_client("aiops").update_investigation_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops/client/update_investigation_group.html)

```python
# update_investigation_group method definition

await def update_investigation_group(
    self,
    *,
    identifier: str,
    roleArn: str = ...,
    encryptionConfiguration: EncryptionConfigurationTypeDef = ...,  # (1)
    tagKeyBoundaries: Sequence[str] = ...,
    chatbotNotificationChannel: Mapping[str, Sequence[str]] = ...,
    isCloudTrailEventHistoryEnabled: bool = ...,
    crossAccountConfigurations: Sequence[CrossAccountConfigurationTypeDef] = ...,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
2. See `Sequence[CrossAccountConfigurationTypeDef]`


```python
# update_investigation_group method usage example with argument unpacking

kwargs: UpdateInvestigationGroupRequestTypeDef = {  # (1)
    "identifier": ...,
}

parent.update_investigation_group(**kwargs)
```

1. See [:material-code-braces: UpdateInvestigationGroupRequestTypeDef](./type_defs.md#updateinvestigationgrouprequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("aiops").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops.html#AIOps.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("aiops").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops.html#AIOps.Client)

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

Type annotations and code completion for `#!python session.create_client("aiops").get_paginator` method with overloads.

- `client.get_paginator("list_investigation_groups")` -> [ListInvestigationGroupsPaginator](./paginators.md#listinvestigationgroupspaginator)



