<a id="cloud9client-for-aiobotocore-cloud9-module"></a>

# Cloud9Client for aiobotocore Cloud9 module

> [Index](../README.md) > [Cloud9](./README.md) > Cloud9Client

Auto-generated documentation for
[Cloud9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
type annotations stubs module
[types-aiobotocore-cloud9](https://pypi.org/project/types-aiobotocore-cloud9/).

- [Cloud9Client for aiobotocore Cloud9 module](#cloud9client-for-aiobotocore-cloud9-module)
  - [Cloud9Client](#cloud9client)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_environment_ec2](#create_environment_ec2)
    - [create_environment_membership](#create_environment_membership)
    - [delete_environment](#delete_environment)
    - [delete_environment_membership](#delete_environment_membership)
    - [describe_environment_memberships](#describe_environment_memberships)
    - [describe_environment_status](#describe_environment_status)
    - [describe_environments](#describe_environments)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_environments](#list_environments)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_environment](#update_environment)
    - [update_environment_membership](#update_environment_membership)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="cloud9client"></a>

## Cloud9Client

Type annotations for `session.create_client("cloud9")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_cloud9.client import Cloud9Client

session = get_session()
async with session.create_client("cloud9") as client:
    client: Cloud9Client
```

Boto3 documentation:
[Cloud9.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_cloud9.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.ConcurrentAccessException`
- `Exceptions.ConflictException`
- `Exceptions.ForbiddenException`
- `Exceptions.InternalServerErrorException`
- `Exceptions.LimitExceededException`
- `Exceptions.NotFoundException`
- `Exceptions.TooManyRequestsException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

Cloud9Client exceptions.

Type annotations for `session.create_client("cloud9").exceptions` method.

Boto3 documentation:
[Cloud9.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("cloud9").can_paginate` method.

Boto3 documentation:
[Cloud9.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_environment\_ec2"></a>

### create_environment_ec2

Creates an Cloud9 development environment, launches an Amazon Elastic Compute
Cloud (Amazon EC2) instance, and then connects from the instance to the
environment.

Type annotations for `session.create_client("cloud9").create_environment_ec2`
method.

Boto3 documentation:
[Cloud9.Client.create_environment_ec2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.create_environment_ec2)

Asynchronous method. Use `await create_environment_ec2(...)` for a synchronous
call.

Arguments mapping described in
[CreateEnvironmentEC2RequestRequestTypeDef](./type_defs.md#createenvironmentec2requestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `instanceType`: `str` *(required)*
- `description`: `str`
- `clientRequestToken`: `str`
- `subnetId`: `str`
- `imageId`: `str`
- `automaticStopTimeMinutes`: `int`
- `ownerArn`: `str`
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `connectionType`: [ConnectionTypeType](./literals.md#connectiontypetype)
- `dryRun`: `bool`

Returns a `Coroutine` for
[CreateEnvironmentEC2ResultTypeDef](./type_defs.md#createenvironmentec2resulttypedef).

<a id="create\_environment\_membership"></a>

### create_environment_membership

Adds an environment member to an Cloud9 development environment.

Type annotations for
`session.create_client("cloud9").create_environment_membership` method.

Boto3 documentation:
[Cloud9.Client.create_environment_membership](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.create_environment_membership)

Asynchronous method. Use `await create_environment_membership(...)` for a
synchronous call.

Arguments mapping described in
[CreateEnvironmentMembershipRequestRequestTypeDef](./type_defs.md#createenvironmentmembershiprequestrequesttypedef).

Keyword-only arguments:

- `environmentId`: `str` *(required)*
- `userArn`: `str` *(required)*
- `permissions`: [MemberPermissionsType](./literals.md#memberpermissionstype)
  *(required)*

Returns a `Coroutine` for
[CreateEnvironmentMembershipResultTypeDef](./type_defs.md#createenvironmentmembershipresulttypedef).

<a id="delete\_environment"></a>

### delete_environment

Deletes an Cloud9 development environment.

Type annotations for `session.create_client("cloud9").delete_environment`
method.

Boto3 documentation:
[Cloud9.Client.delete_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.delete_environment)

Asynchronous method. Use `await delete_environment(...)` for a synchronous
call.

Arguments mapping described in
[DeleteEnvironmentRequestRequestTypeDef](./type_defs.md#deleteenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `environmentId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_environment\_membership"></a>

### delete_environment_membership

Deletes an environment member from an Cloud9 development environment.

Type annotations for
`session.create_client("cloud9").delete_environment_membership` method.

Boto3 documentation:
[Cloud9.Client.delete_environment_membership](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.delete_environment_membership)

Asynchronous method. Use `await delete_environment_membership(...)` for a
synchronous call.

Arguments mapping described in
[DeleteEnvironmentMembershipRequestRequestTypeDef](./type_defs.md#deleteenvironmentmembershiprequestrequesttypedef).

Keyword-only arguments:

- `environmentId`: `str` *(required)*
- `userArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe\_environment\_memberships"></a>

### describe_environment_memberships

Gets information about environment members for an Cloud9 development
environment.

Type annotations for
`session.create_client("cloud9").describe_environment_memberships` method.

Boto3 documentation:
[Cloud9.Client.describe_environment_memberships](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.describe_environment_memberships)

Asynchronous method. Use `await describe_environment_memberships(...)` for a
synchronous call.

Arguments mapping described in
[DescribeEnvironmentMembershipsRequestRequestTypeDef](./type_defs.md#describeenvironmentmembershipsrequestrequesttypedef).

Keyword-only arguments:

- `userArn`: `str`
- `environmentId`: `str`
- `permissions`: `Sequence`\[[PermissionsType](./literals.md#permissionstype)\]
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[DescribeEnvironmentMembershipsResultTypeDef](./type_defs.md#describeenvironmentmembershipsresulttypedef).

<a id="describe\_environment\_status"></a>

### describe_environment_status

Gets status information for an Cloud9 development environment.

Type annotations for
`session.create_client("cloud9").describe_environment_status` method.

Boto3 documentation:
[Cloud9.Client.describe_environment_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.describe_environment_status)

Asynchronous method. Use `await describe_environment_status(...)` for a
synchronous call.

Arguments mapping described in
[DescribeEnvironmentStatusRequestRequestTypeDef](./type_defs.md#describeenvironmentstatusrequestrequesttypedef).

Keyword-only arguments:

- `environmentId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeEnvironmentStatusResultTypeDef](./type_defs.md#describeenvironmentstatusresulttypedef).

<a id="describe\_environments"></a>

### describe_environments

Gets information about Cloud9 development environments.

Type annotations for `session.create_client("cloud9").describe_environments`
method.

Boto3 documentation:
[Cloud9.Client.describe_environments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.describe_environments)

Asynchronous method. Use `await describe_environments(...)` for a synchronous
call.

Arguments mapping described in
[DescribeEnvironmentsRequestRequestTypeDef](./type_defs.md#describeenvironmentsrequestrequesttypedef).

Keyword-only arguments:

- `environmentIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[DescribeEnvironmentsResultTypeDef](./type_defs.md#describeenvironmentsresulttypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("cloud9").generate_presigned_url`
method.

Boto3 documentation:
[Cloud9.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list\_environments"></a>

### list_environments

Gets a list of Cloud9 development environment identifiers.

Type annotations for `session.create_client("cloud9").list_environments`
method.

Boto3 documentation:
[Cloud9.Client.list_environments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.list_environments)

Asynchronous method. Use `await list_environments(...)` for a synchronous call.

Arguments mapping described in
[ListEnvironmentsRequestRequestTypeDef](./type_defs.md#listenvironmentsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListEnvironmentsResultTypeDef](./type_defs.md#listenvironmentsresulttypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Gets a list of the tags associated with an Cloud9 development environment.

Type annotations for `session.create_client("cloud9").list_tags_for_resource`
method.

Boto3 documentation:
[Cloud9.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="tag\_resource"></a>

### tag_resource

Adds tags to an Cloud9 development environment.

Type annotations for `session.create_client("cloud9").tag_resource` method.

Boto3 documentation:
[Cloud9.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Removes tags from an Cloud9 development environment.

Type annotations for `session.create_client("cloud9").untag_resource` method.

Boto3 documentation:
[Cloud9.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_environment"></a>

### update_environment

Changes the settings of an existing Cloud9 development environment.

Type annotations for `session.create_client("cloud9").update_environment`
method.

Boto3 documentation:
[Cloud9.Client.update_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.update_environment)

Asynchronous method. Use `await update_environment(...)` for a synchronous
call.

Arguments mapping described in
[UpdateEnvironmentRequestRequestTypeDef](./type_defs.md#updateenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `environmentId`: `str` *(required)*
- `name`: `str`
- `description`: `str`
- `managedCredentialsAction`:
  [ManagedCredentialsActionType](./literals.md#managedcredentialsactiontype)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_environment\_membership"></a>

### update_environment_membership

Changes the settings of an existing environment member for an Cloud9
development environment.

Type annotations for
`session.create_client("cloud9").update_environment_membership` method.

Boto3 documentation:
[Cloud9.Client.update_environment_membership](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.update_environment_membership)

Asynchronous method. Use `await update_environment_membership(...)` for a
synchronous call.

Arguments mapping described in
[UpdateEnvironmentMembershipRequestRequestTypeDef](./type_defs.md#updateenvironmentmembershiprequestrequesttypedef).

Keyword-only arguments:

- `environmentId`: `str` *(required)*
- `userArn`: `str` *(required)*
- `permissions`: [MemberPermissionsType](./literals.md#memberpermissionstype)
  *(required)*

Returns a `Coroutine` for
[UpdateEnvironmentMembershipResultTypeDef](./type_defs.md#updateenvironmentmembershipresulttypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("cloud9").__aenter__` method.

Boto3 documentation:
[Cloud9.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [Cloud9Client](#cloud9client).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("cloud9").__aexit__` method.

Boto3 documentation:
[Cloud9.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("cloud9").get_paginator` method
with overloads.

- `client.get_paginator("describe_environment_memberships")` ->
  [DescribeEnvironmentMembershipsPaginator](./paginators.md#describeenvironmentmembershipspaginator)
- `client.get_paginator("list_environments")` ->
  [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
