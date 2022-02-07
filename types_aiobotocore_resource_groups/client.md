<a id="resourcegroupsclient-for-aiobotocore-resourcegroups-module"></a>

# ResourceGroupsClient for aiobotocore ResourceGroups module

> [Index](..) > [ResourceGroups](.) > ResourceGroupsClient

Auto-generated documentation for
[ResourceGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
type annotations stubs module
[types-aiobotocore-resource-groups](https://pypi.org/project/types-aiobotocore-resource-groups/).

- [ResourceGroupsClient for aiobotocore ResourceGroups module](#resourcegroupsclient-for-aiobotocore-resourcegroups-module)
  - [ResourceGroupsClient](#resourcegroupsclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_group](#create_group)
    - [delete_group](#delete_group)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_group](#get_group)
    - [get_group_configuration](#get_group_configuration)
    - [get_group_query](#get_group_query)
    - [get_tags](#get_tags)
    - [group_resources](#group_resources)
    - [list_group_resources](#list_group_resources)
    - [list_groups](#list_groups)
    - [put_group_configuration](#put_group_configuration)
    - [search_resources](#search_resources)
    - [tag](#tag)
    - [ungroup_resources](#ungroup_resources)
    - [untag](#untag)
    - [update_group](#update_group)
    - [update_group_query](#update_group_query)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="resourcegroupsclient"></a>

## ResourceGroupsClient

Type annotations for `session.create_client("resource-groups")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_resource_groups.client import ResourceGroupsClient

session = get_session()
async with session.create_client("resource-groups") as client:
    client: ResourceGroupsClient
```

Boto3 documentation:
[ResourceGroups.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_resource_groups.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.ForbiddenException`
- `Exceptions.InternalServerErrorException`
- `Exceptions.MethodNotAllowedException`
- `Exceptions.NotFoundException`
- `Exceptions.TooManyRequestsException`
- `Exceptions.UnauthorizedException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ResourceGroupsClient exceptions.

Type annotations for `session.create_client("resource-groups").exceptions`
method.

Boto3 documentation:
[ResourceGroups.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("resource-groups").can_paginate`
method.

Boto3 documentation:
[ResourceGroups.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_group"></a>

### create_group

Creates a resource group with the specified name and description.

Type annotations for `session.create_client("resource-groups").create_group`
method.

Boto3 documentation:
[ResourceGroups.Client.create_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.create_group)

Asynchronous method. Use `await create_group(...)` for a synchronous call.

Arguments mapping described in
[CreateGroupInputRequestTypeDef](./type_defs.md#creategroupinputrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Description`: `str`
- `ResourceQuery`: [ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef)
- `Tags`: `Mapping`\[`str`, `str`\]
- `Configuration`:
  `Sequence`\[[GroupConfigurationItemTypeDef](./type_defs.md#groupconfigurationitemtypedef)\]

Returns a `Coroutine` for
[CreateGroupOutputTypeDef](./type_defs.md#creategroupoutputtypedef).

<a id="delete_group"></a>

### delete_group

Deletes the specified resource group.

Type annotations for `session.create_client("resource-groups").delete_group`
method.

Boto3 documentation:
[ResourceGroups.Client.delete_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.delete_group)

Asynchronous method. Use `await delete_group(...)` for a synchronous call.

Arguments mapping described in
[DeleteGroupInputRequestTypeDef](./type_defs.md#deletegroupinputrequesttypedef).

Keyword-only arguments:

- `GroupName`: `str`
- `Group`: `str`

Returns a `Coroutine` for
[DeleteGroupOutputTypeDef](./type_defs.md#deletegroupoutputtypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("resource-groups").generate_presigned_url` method.

Boto3 documentation:
[ResourceGroups.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_group"></a>

### get_group

Returns information about a specified resource group.

Type annotations for `session.create_client("resource-groups").get_group`
method.

Boto3 documentation:
[ResourceGroups.Client.get_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.get_group)

Asynchronous method. Use `await get_group(...)` for a synchronous call.

Arguments mapping described in
[GetGroupInputRequestTypeDef](./type_defs.md#getgroupinputrequesttypedef).

Keyword-only arguments:

- `GroupName`: `str`
- `Group`: `str`

Returns a `Coroutine` for
[GetGroupOutputTypeDef](./type_defs.md#getgroupoutputtypedef).

<a id="get_group_configuration"></a>

### get_group_configuration

Returns the service configuration associated with the specified resource group.

Type annotations for
`session.create_client("resource-groups").get_group_configuration` method.

Boto3 documentation:
[ResourceGroups.Client.get_group_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.get_group_configuration)

Asynchronous method. Use `await get_group_configuration(...)` for a synchronous
call.

Arguments mapping described in
[GetGroupConfigurationInputRequestTypeDef](./type_defs.md#getgroupconfigurationinputrequesttypedef).

Keyword-only arguments:

- `Group`: `str`

Returns a `Coroutine` for
[GetGroupConfigurationOutputTypeDef](./type_defs.md#getgroupconfigurationoutputtypedef).

<a id="get_group_query"></a>

### get_group_query

Retrieves the resource query associated with the specified resource group.

Type annotations for `session.create_client("resource-groups").get_group_query`
method.

Boto3 documentation:
[ResourceGroups.Client.get_group_query](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.get_group_query)

Asynchronous method. Use `await get_group_query(...)` for a synchronous call.

Arguments mapping described in
[GetGroupQueryInputRequestTypeDef](./type_defs.md#getgroupqueryinputrequesttypedef).

Keyword-only arguments:

- `GroupName`: `str`
- `Group`: `str`

Returns a `Coroutine` for
[GetGroupQueryOutputTypeDef](./type_defs.md#getgroupqueryoutputtypedef).

<a id="get_tags"></a>

### get_tags

Returns a list of tags that are associated with a resource group, specified by
an ARN.

Type annotations for `session.create_client("resource-groups").get_tags`
method.

Boto3 documentation:
[ResourceGroups.Client.get_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.get_tags)

Asynchronous method. Use `await get_tags(...)` for a synchronous call.

Arguments mapping described in
[GetTagsInputRequestTypeDef](./type_defs.md#gettagsinputrequesttypedef).

Keyword-only arguments:

- `Arn`: `str` *(required)*

Returns a `Coroutine` for
[GetTagsOutputTypeDef](./type_defs.md#gettagsoutputtypedef).

<a id="group_resources"></a>

### group_resources

Adds the specified resources to the specified group.

Type annotations for `session.create_client("resource-groups").group_resources`
method.

Boto3 documentation:
[ResourceGroups.Client.group_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.group_resources)

Asynchronous method. Use `await group_resources(...)` for a synchronous call.

Arguments mapping described in
[GroupResourcesInputRequestTypeDef](./type_defs.md#groupresourcesinputrequesttypedef).

Keyword-only arguments:

- `Group`: `str` *(required)*
- `ResourceArns`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[GroupResourcesOutputTypeDef](./type_defs.md#groupresourcesoutputtypedef).

<a id="list_group_resources"></a>

### list_group_resources

Returns a list of ARNs of the resources that are members of a specified
resource group.

Type annotations for
`session.create_client("resource-groups").list_group_resources` method.

Boto3 documentation:
[ResourceGroups.Client.list_group_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_group_resources)

Asynchronous method. Use `await list_group_resources(...)` for a synchronous
call.

Arguments mapping described in
[ListGroupResourcesInputRequestTypeDef](./type_defs.md#listgroupresourcesinputrequesttypedef).

Keyword-only arguments:

- `GroupName`: `str`
- `Group`: `str`
- `Filters`:
  `Sequence`\[[ResourceFilterTypeDef](./type_defs.md#resourcefiltertypedef)\]
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListGroupResourcesOutputTypeDef](./type_defs.md#listgroupresourcesoutputtypedef).

<a id="list_groups"></a>

### list_groups

Returns a list of existing resource groups in your account.

Type annotations for `session.create_client("resource-groups").list_groups`
method.

Boto3 documentation:
[ResourceGroups.Client.list_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_groups)

Asynchronous method. Use `await list_groups(...)` for a synchronous call.

Arguments mapping described in
[ListGroupsInputRequestTypeDef](./type_defs.md#listgroupsinputrequesttypedef).

Keyword-only arguments:

- `Filters`:
  `Sequence`\[[GroupFilterTypeDef](./type_defs.md#groupfiltertypedef)\]
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListGroupsOutputTypeDef](./type_defs.md#listgroupsoutputtypedef).

<a id="put_group_configuration"></a>

### put_group_configuration

Attaches a service configuration to the specified group.

Type annotations for
`session.create_client("resource-groups").put_group_configuration` method.

Boto3 documentation:
[ResourceGroups.Client.put_group_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.put_group_configuration)

Asynchronous method. Use `await put_group_configuration(...)` for a synchronous
call.

Arguments mapping described in
[PutGroupConfigurationInputRequestTypeDef](./type_defs.md#putgroupconfigurationinputrequesttypedef).

Keyword-only arguments:

- `Group`: `str`
- `Configuration`:
  `Sequence`\[[GroupConfigurationItemTypeDef](./type_defs.md#groupconfigurationitemtypedef)\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="search_resources"></a>

### search_resources

Returns a list of AWS resource identifiers that matches the specified query.

Type annotations for
`session.create_client("resource-groups").search_resources` method.

Boto3 documentation:
[ResourceGroups.Client.search_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.search_resources)

Asynchronous method. Use `await search_resources(...)` for a synchronous call.

Arguments mapping described in
[SearchResourcesInputRequestTypeDef](./type_defs.md#searchresourcesinputrequesttypedef).

Keyword-only arguments:

- `ResourceQuery`: [ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef)
  *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[SearchResourcesOutputTypeDef](./type_defs.md#searchresourcesoutputtypedef).

<a id="tag"></a>

### tag

Adds tags to a resource group with the specified ARN.

Type annotations for `session.create_client("resource-groups").tag` method.

Boto3 documentation:
[ResourceGroups.Client.tag](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.tag)

Asynchronous method. Use `await tag(...)` for a synchronous call.

Arguments mapping described in
[TagInputRequestTypeDef](./type_defs.md#taginputrequesttypedef).

Keyword-only arguments:

- `Arn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for [TagOutputTypeDef](./type_defs.md#tagoutputtypedef).

<a id="ungroup_resources"></a>

### ungroup_resources

Removes the specified resources from the specified group.

Type annotations for
`session.create_client("resource-groups").ungroup_resources` method.

Boto3 documentation:
[ResourceGroups.Client.ungroup_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.ungroup_resources)

Asynchronous method. Use `await ungroup_resources(...)` for a synchronous call.

Arguments mapping described in
[UngroupResourcesInputRequestTypeDef](./type_defs.md#ungroupresourcesinputrequesttypedef).

Keyword-only arguments:

- `Group`: `str` *(required)*
- `ResourceArns`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[UngroupResourcesOutputTypeDef](./type_defs.md#ungroupresourcesoutputtypedef).

<a id="untag"></a>

### untag

Deletes tags from a specified resource group.

Type annotations for `session.create_client("resource-groups").untag` method.

Boto3 documentation:
[ResourceGroups.Client.untag](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.untag)

Asynchronous method. Use `await untag(...)` for a synchronous call.

Arguments mapping described in
[UntagInputRequestTypeDef](./type_defs.md#untaginputrequesttypedef).

Keyword-only arguments:

- `Arn`: `str` *(required)*
- `Keys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[UntagOutputTypeDef](./type_defs.md#untagoutputtypedef).

<a id="update_group"></a>

### update_group

Updates the description for an existing group.

Type annotations for `session.create_client("resource-groups").update_group`
method.

Boto3 documentation:
[ResourceGroups.Client.update_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.update_group)

Asynchronous method. Use `await update_group(...)` for a synchronous call.

Arguments mapping described in
[UpdateGroupInputRequestTypeDef](./type_defs.md#updategroupinputrequesttypedef).

Keyword-only arguments:

- `GroupName`: `str`
- `Group`: `str`
- `Description`: `str`

Returns a `Coroutine` for
[UpdateGroupOutputTypeDef](./type_defs.md#updategroupoutputtypedef).

<a id="update_group_query"></a>

### update_group_query

Updates the resource query of a group.

Type annotations for
`session.create_client("resource-groups").update_group_query` method.

Boto3 documentation:
[ResourceGroups.Client.update_group_query](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.update_group_query)

Asynchronous method. Use `await update_group_query(...)` for a synchronous
call.

Arguments mapping described in
[UpdateGroupQueryInputRequestTypeDef](./type_defs.md#updategroupqueryinputrequesttypedef).

Keyword-only arguments:

- `ResourceQuery`: [ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef)
  *(required)*
- `GroupName`: `str`
- `Group`: `str`

Returns a `Coroutine` for
[UpdateGroupQueryOutputTypeDef](./type_defs.md#updategroupqueryoutputtypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("resource-groups").__aenter__`
method.

Boto3 documentation:
[ResourceGroups.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [ResourceGroupsClient](#resourcegroupsclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("resource-groups").__aexit__`
method.

Boto3 documentation:
[ResourceGroups.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("resource-groups").get_paginator`
method with overloads.

- `client.get_paginator("list_group_resources")` ->
  [ListGroupResourcesPaginator](./paginators.md#listgroupresourcespaginator)
- `client.get_paginator("list_groups")` ->
  [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- `client.get_paginator("search_resources")` ->
  [SearchResourcesPaginator](./paginators.md#searchresourcespaginator)
