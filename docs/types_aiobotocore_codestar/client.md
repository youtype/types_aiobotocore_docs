<a id="codestarclient-for-aiobotocore-codestar-module"></a>

# CodeStarClient for aiobotocore CodeStar module

> [Index](../README.md) > [CodeStar](./README.md) > CodeStarClient

Auto-generated documentation for
[CodeStar](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
type annotations stubs module
[types-aiobotocore-codestar](https://pypi.org/project/types-aiobotocore-codestar/).

- [CodeStarClient for aiobotocore CodeStar module](#codestarclient-for-aiobotocore-codestar-module)
  - [CodeStarClient](#codestarclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [associate_team_member](#associate_team_member)
    - [can_paginate](#can_paginate)
    - [create_project](#create_project)
    - [create_user_profile](#create_user_profile)
    - [delete_project](#delete_project)
    - [delete_user_profile](#delete_user_profile)
    - [describe_project](#describe_project)
    - [describe_user_profile](#describe_user_profile)
    - [disassociate_team_member](#disassociate_team_member)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_projects](#list_projects)
    - [list_resources](#list_resources)
    - [list_tags_for_project](#list_tags_for_project)
    - [list_team_members](#list_team_members)
    - [list_user_profiles](#list_user_profiles)
    - [tag_project](#tag_project)
    - [untag_project](#untag_project)
    - [update_project](#update_project)
    - [update_team_member](#update_team_member)
    - [update_user_profile](#update_user_profile)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="codestarclient"></a>

## CodeStarClient

Type annotations for `session.create_client("codestar")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_codestar.client import CodeStarClient

session = get_session()
async with session.create_client("codestar") as client:
    client: CodeStarClient
```

Boto3 documentation:
[CodeStar.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_codestar.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConcurrentModificationException`
- `Exceptions.InvalidNextTokenException`
- `Exceptions.InvalidServiceRoleException`
- `Exceptions.LimitExceededException`
- `Exceptions.ProjectAlreadyExistsException`
- `Exceptions.ProjectConfigurationException`
- `Exceptions.ProjectCreationFailedException`
- `Exceptions.ProjectNotFoundException`
- `Exceptions.TeamMemberAlreadyAssociatedException`
- `Exceptions.TeamMemberNotFoundException`
- `Exceptions.UserProfileAlreadyExistsException`
- `Exceptions.UserProfileNotFoundException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

CodeStarClient exceptions.

Type annotations for `session.create_client("codestar").exceptions` method.

Boto3 documentation:
[CodeStar.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="associate\_team\_member"></a>

### associate_team_member

Adds an IAM user to the team for an AWS CodeStar project.

Type annotations for `session.create_client("codestar").associate_team_member`
method.

Boto3 documentation:
[CodeStar.Client.associate_team_member](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.associate_team_member)

Asynchronous method. Use `await associate_team_member(...)` for a synchronous
call.

Arguments mapping described in
[AssociateTeamMemberRequestRequestTypeDef](./type_defs.md#associateteammemberrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `userArn`: `str` *(required)*
- `projectRole`: `str` *(required)*
- `clientRequestToken`: `str`
- `remoteAccessAllowed`: `bool`

Returns a `Coroutine` for
[AssociateTeamMemberResultTypeDef](./type_defs.md#associateteammemberresulttypedef).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("codestar").can_paginate` method.

Boto3 documentation:
[CodeStar.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_project"></a>

### create_project

Creates a project, including project resources.

Type annotations for `session.create_client("codestar").create_project` method.

Boto3 documentation:
[CodeStar.Client.create_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.create_project)

Asynchronous method. Use `await create_project(...)` for a synchronous call.

Arguments mapping described in
[CreateProjectRequestRequestTypeDef](./type_defs.md#createprojectrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `id`: `str` *(required)*
- `description`: `str`
- `clientRequestToken`: `str`
- `sourceCode`: `Sequence`\[[CodeTypeDef](./type_defs.md#codetypedef)\]
- `toolchain`: [ToolchainTypeDef](./type_defs.md#toolchaintypedef)
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateProjectResultTypeDef](./type_defs.md#createprojectresulttypedef).

<a id="create\_user\_profile"></a>

### create_user_profile

Creates a profile for a user that includes user preferences, such as the
display name and email address assocciated with the user, in AWS CodeStar.

Type annotations for `session.create_client("codestar").create_user_profile`
method.

Boto3 documentation:
[CodeStar.Client.create_user_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.create_user_profile)

Asynchronous method. Use `await create_user_profile(...)` for a synchronous
call.

Arguments mapping described in
[CreateUserProfileRequestRequestTypeDef](./type_defs.md#createuserprofilerequestrequesttypedef).

Keyword-only arguments:

- `userArn`: `str` *(required)*
- `displayName`: `str` *(required)*
- `emailAddress`: `str` *(required)*
- `sshPublicKey`: `str`

Returns a `Coroutine` for
[CreateUserProfileResultTypeDef](./type_defs.md#createuserprofileresulttypedef).

<a id="delete\_project"></a>

### delete_project

Deletes a project, including project resources.

Type annotations for `session.create_client("codestar").delete_project` method.

Boto3 documentation:
[CodeStar.Client.delete_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.delete_project)

Asynchronous method. Use `await delete_project(...)` for a synchronous call.

Arguments mapping described in
[DeleteProjectRequestRequestTypeDef](./type_defs.md#deleteprojectrequestrequesttypedef).

Keyword-only arguments:

- `id`: `str` *(required)*
- `clientRequestToken`: `str`
- `deleteStack`: `bool`

Returns a `Coroutine` for
[DeleteProjectResultTypeDef](./type_defs.md#deleteprojectresulttypedef).

<a id="delete\_user\_profile"></a>

### delete_user_profile

Deletes a user profile in AWS CodeStar, including all personal preference data
associated with that profile, such as display name and email address.

Type annotations for `session.create_client("codestar").delete_user_profile`
method.

Boto3 documentation:
[CodeStar.Client.delete_user_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.delete_user_profile)

Asynchronous method. Use `await delete_user_profile(...)` for a synchronous
call.

Arguments mapping described in
[DeleteUserProfileRequestRequestTypeDef](./type_defs.md#deleteuserprofilerequestrequesttypedef).

Keyword-only arguments:

- `userArn`: `str` *(required)*

Returns a `Coroutine` for
[DeleteUserProfileResultTypeDef](./type_defs.md#deleteuserprofileresulttypedef).

<a id="describe\_project"></a>

### describe_project

Describes a project and its resources.

Type annotations for `session.create_client("codestar").describe_project`
method.

Boto3 documentation:
[CodeStar.Client.describe_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.describe_project)

Asynchronous method. Use `await describe_project(...)` for a synchronous call.

Arguments mapping described in
[DescribeProjectRequestRequestTypeDef](./type_defs.md#describeprojectrequestrequesttypedef).

Keyword-only arguments:

- `id`: `str` *(required)*

Returns a `Coroutine` for
[DescribeProjectResultTypeDef](./type_defs.md#describeprojectresulttypedef).

<a id="describe\_user\_profile"></a>

### describe_user_profile

Describes a user in AWS CodeStar and the user attributes across all projects.

Type annotations for `session.create_client("codestar").describe_user_profile`
method.

Boto3 documentation:
[CodeStar.Client.describe_user_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.describe_user_profile)

Asynchronous method. Use `await describe_user_profile(...)` for a synchronous
call.

Arguments mapping described in
[DescribeUserProfileRequestRequestTypeDef](./type_defs.md#describeuserprofilerequestrequesttypedef).

Keyword-only arguments:

- `userArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeUserProfileResultTypeDef](./type_defs.md#describeuserprofileresulttypedef).

<a id="disassociate\_team\_member"></a>

### disassociate_team_member

Removes a user from a project.

Type annotations for
`session.create_client("codestar").disassociate_team_member` method.

Boto3 documentation:
[CodeStar.Client.disassociate_team_member](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.disassociate_team_member)

Asynchronous method. Use `await disassociate_team_member(...)` for a
synchronous call.

Arguments mapping described in
[DisassociateTeamMemberRequestRequestTypeDef](./type_defs.md#disassociateteammemberrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `userArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("codestar").generate_presigned_url`
method.

Boto3 documentation:
[CodeStar.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list\_projects"></a>

### list_projects

Lists all projects in AWS CodeStar associated with your AWS account.

Type annotations for `session.create_client("codestar").list_projects` method.

Boto3 documentation:
[CodeStar.Client.list_projects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.list_projects)

Asynchronous method. Use `await list_projects(...)` for a synchronous call.

Arguments mapping described in
[ListProjectsRequestRequestTypeDef](./type_defs.md#listprojectsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef).

<a id="list\_resources"></a>

### list_resources

Lists resources associated with a project in AWS CodeStar.

Type annotations for `session.create_client("codestar").list_resources` method.

Boto3 documentation:
[CodeStar.Client.list_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.list_resources)

Asynchronous method. Use `await list_resources(...)` for a synchronous call.

Arguments mapping described in
[ListResourcesRequestRequestTypeDef](./type_defs.md#listresourcesrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListResourcesResultTypeDef](./type_defs.md#listresourcesresulttypedef).

<a id="list\_tags\_for\_project"></a>

### list_tags_for_project

Gets the tags for a project.

Type annotations for `session.create_client("codestar").list_tags_for_project`
method.

Boto3 documentation:
[CodeStar.Client.list_tags_for_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.list_tags_for_project)

Asynchronous method. Use `await list_tags_for_project(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForProjectRequestRequestTypeDef](./type_defs.md#listtagsforprojectrequestrequesttypedef).

Keyword-only arguments:

- `id`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListTagsForProjectResultTypeDef](./type_defs.md#listtagsforprojectresulttypedef).

<a id="list\_team\_members"></a>

### list_team_members

Lists all team members associated with a project.

Type annotations for `session.create_client("codestar").list_team_members`
method.

Boto3 documentation:
[CodeStar.Client.list_team_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.list_team_members)

Asynchronous method. Use `await list_team_members(...)` for a synchronous call.

Arguments mapping described in
[ListTeamMembersRequestRequestTypeDef](./type_defs.md#listteammembersrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListTeamMembersResultTypeDef](./type_defs.md#listteammembersresulttypedef).

<a id="list\_user\_profiles"></a>

### list_user_profiles

Lists all the user profiles configured for your AWS account in AWS CodeStar.

Type annotations for `session.create_client("codestar").list_user_profiles`
method.

Boto3 documentation:
[CodeStar.Client.list_user_profiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.list_user_profiles)

Asynchronous method. Use `await list_user_profiles(...)` for a synchronous
call.

Arguments mapping described in
[ListUserProfilesRequestRequestTypeDef](./type_defs.md#listuserprofilesrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListUserProfilesResultTypeDef](./type_defs.md#listuserprofilesresulttypedef).

<a id="tag\_project"></a>

### tag_project

Adds tags to a project.

Type annotations for `session.create_client("codestar").tag_project` method.

Boto3 documentation:
[CodeStar.Client.tag_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.tag_project)

Asynchronous method. Use `await tag_project(...)` for a synchronous call.

Arguments mapping described in
[TagProjectRequestRequestTypeDef](./type_defs.md#tagprojectrequestrequesttypedef).

Keyword-only arguments:

- `id`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for
[TagProjectResultTypeDef](./type_defs.md#tagprojectresulttypedef).

<a id="untag\_project"></a>

### untag_project

Removes tags from a project.

Type annotations for `session.create_client("codestar").untag_project` method.

Boto3 documentation:
[CodeStar.Client.untag_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.untag_project)

Asynchronous method. Use `await untag_project(...)` for a synchronous call.

Arguments mapping described in
[UntagProjectRequestRequestTypeDef](./type_defs.md#untagprojectrequestrequesttypedef).

Keyword-only arguments:

- `id`: `str` *(required)*
- `tags`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_project"></a>

### update_project

Updates a project in AWS CodeStar.

Type annotations for `session.create_client("codestar").update_project` method.

Boto3 documentation:
[CodeStar.Client.update_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.update_project)

Asynchronous method. Use `await update_project(...)` for a synchronous call.

Arguments mapping described in
[UpdateProjectRequestRequestTypeDef](./type_defs.md#updateprojectrequestrequesttypedef).

Keyword-only arguments:

- `id`: `str` *(required)*
- `name`: `str`
- `description`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_team\_member"></a>

### update_team_member

Updates a team member's attributes in an AWS CodeStar project.

Type annotations for `session.create_client("codestar").update_team_member`
method.

Boto3 documentation:
[CodeStar.Client.update_team_member](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.update_team_member)

Asynchronous method. Use `await update_team_member(...)` for a synchronous
call.

Arguments mapping described in
[UpdateTeamMemberRequestRequestTypeDef](./type_defs.md#updateteammemberrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `userArn`: `str` *(required)*
- `projectRole`: `str`
- `remoteAccessAllowed`: `bool`

Returns a `Coroutine` for
[UpdateTeamMemberResultTypeDef](./type_defs.md#updateteammemberresulttypedef).

<a id="update\_user\_profile"></a>

### update_user_profile

Updates a user's profile in AWS CodeStar.

Type annotations for `session.create_client("codestar").update_user_profile`
method.

Boto3 documentation:
[CodeStar.Client.update_user_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.update_user_profile)

Asynchronous method. Use `await update_user_profile(...)` for a synchronous
call.

Arguments mapping described in
[UpdateUserProfileRequestRequestTypeDef](./type_defs.md#updateuserprofilerequestrequesttypedef).

Keyword-only arguments:

- `userArn`: `str` *(required)*
- `displayName`: `str`
- `emailAddress`: `str`
- `sshPublicKey`: `str`

Returns a `Coroutine` for
[UpdateUserProfileResultTypeDef](./type_defs.md#updateuserprofileresulttypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("codestar").__aenter__` method.

Boto3 documentation:
[CodeStar.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [CodeStarClient](#codestarclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("codestar").__aexit__` method.

Boto3 documentation:
[CodeStar.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("codestar").get_paginator` method
with overloads.

- `client.get_paginator("list_projects")` ->
  [ListProjectsPaginator](./paginators.md#listprojectspaginator)
- `client.get_paginator("list_resources")` ->
  [ListResourcesPaginator](./paginators.md#listresourcespaginator)
- `client.get_paginator("list_team_members")` ->
  [ListTeamMembersPaginator](./paginators.md#listteammemberspaginator)
- `client.get_paginator("list_user_profiles")` ->
  [ListUserProfilesPaginator](./paginators.md#listuserprofilespaginator)
