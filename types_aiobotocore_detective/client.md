<a id="detectiveclient-for-aiobotocore-detective-module"></a>

# DetectiveClient for aiobotocore Detective module

> [Index](..) > [Detective](.) > DetectiveClient

Auto-generated documentation for
[Detective](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
type annotations stubs module
[types-aiobotocore-detective](https://pypi.org/project/types-aiobotocore-detective/).

- [DetectiveClient for aiobotocore Detective module](#detectiveclient-for-aiobotocore-detective-module)
  - [DetectiveClient](#detectiveclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [accept_invitation](#accept_invitation)
    - [can_paginate](#can_paginate)
    - [create_graph](#create_graph)
    - [create_members](#create_members)
    - [delete_graph](#delete_graph)
    - [delete_members](#delete_members)
    - [disassociate_membership](#disassociate_membership)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_members](#get_members)
    - [list_graphs](#list_graphs)
    - [list_invitations](#list_invitations)
    - [list_members](#list_members)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [reject_invitation](#reject_invitation)
    - [start_monitoring_member](#start_monitoring_member)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)

<a id="detectiveclient"></a>

## DetectiveClient

Type annotations for `session.create_client("detective")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_detective.client import DetectiveClient

session = get_session()
async with session.create_client("detective") as client:
    client: DetectiveClient
```

Boto3 documentation:
[Detective.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_detective.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

DetectiveClient exceptions.

Type annotations for `session.create_client("detective").exceptions` method.

Boto3 documentation:
[Detective.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="accept_invitation"></a>

### accept_invitation

Accepts an invitation for the member account to contribute data to a behavior
graph.

Type annotations for `session.create_client("detective").accept_invitation`
method.

Boto3 documentation:
[Detective.Client.accept_invitation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.accept_invitation)

Asynchronous method. Use `await accept_invitation(...)` for a synchronous call.

Arguments mapping described in
[AcceptInvitationRequestRequestTypeDef](./type_defs.md#acceptinvitationrequestrequesttypedef).

Keyword-only arguments:

- `GraphArn`: `str` *(required)*

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("detective").can_paginate` method.

Boto3 documentation:
[Detective.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_graph"></a>

### create_graph

Creates a new behavior graph for the calling account, and sets that account as
the administrator account.

Type annotations for `session.create_client("detective").create_graph` method.

Boto3 documentation:
[Detective.Client.create_graph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.create_graph)

Asynchronous method. Use `await create_graph(...)` for a synchronous call.

Arguments mapping described in
[CreateGraphRequestRequestTypeDef](./type_defs.md#creategraphrequestrequesttypedef).

Keyword-only arguments:

- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateGraphResponseTypeDef](./type_defs.md#creategraphresponsetypedef).

<a id="create_members"></a>

### create_members

Sends a request to invite the specified AWS accounts to be member accounts in
the behavior graph.

Type annotations for `session.create_client("detective").create_members`
method.

Boto3 documentation:
[Detective.Client.create_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.create_members)

Asynchronous method. Use `await create_members(...)` for a synchronous call.

Arguments mapping described in
[CreateMembersRequestRequestTypeDef](./type_defs.md#createmembersrequestrequesttypedef).

Keyword-only arguments:

- `GraphArn`: `str` *(required)*
- `Accounts`: `Sequence`\[[AccountTypeDef](./type_defs.md#accounttypedef)\]
  *(required)*
- `Message`: `str`
- `DisableEmailNotification`: `bool`

Returns a `Coroutine` for
[CreateMembersResponseTypeDef](./type_defs.md#createmembersresponsetypedef).

<a id="delete_graph"></a>

### delete_graph

Disables the specified behavior graph and queues it to be deleted.

Type annotations for `session.create_client("detective").delete_graph` method.

Boto3 documentation:
[Detective.Client.delete_graph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.delete_graph)

Asynchronous method. Use `await delete_graph(...)` for a synchronous call.

Arguments mapping described in
[DeleteGraphRequestRequestTypeDef](./type_defs.md#deletegraphrequestrequesttypedef).

Keyword-only arguments:

- `GraphArn`: `str` *(required)*

<a id="delete_members"></a>

### delete_members

Deletes one or more member accounts from the administrator account's behavior
graph.

Type annotations for `session.create_client("detective").delete_members`
method.

Boto3 documentation:
[Detective.Client.delete_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.delete_members)

Asynchronous method. Use `await delete_members(...)` for a synchronous call.

Arguments mapping described in
[DeleteMembersRequestRequestTypeDef](./type_defs.md#deletemembersrequestrequesttypedef).

Keyword-only arguments:

- `GraphArn`: `str` *(required)*
- `AccountIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[DeleteMembersResponseTypeDef](./type_defs.md#deletemembersresponsetypedef).

<a id="disassociate_membership"></a>

### disassociate_membership

Removes the member account from the specified behavior graph.

Type annotations for
`session.create_client("detective").disassociate_membership` method.

Boto3 documentation:
[Detective.Client.disassociate_membership](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.disassociate_membership)

Asynchronous method. Use `await disassociate_membership(...)` for a synchronous
call.

Arguments mapping described in
[DisassociateMembershipRequestRequestTypeDef](./type_defs.md#disassociatemembershiprequestrequesttypedef).

Keyword-only arguments:

- `GraphArn`: `str` *(required)*

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("detective").generate_presigned_url` method.

Boto3 documentation:
[Detective.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_members"></a>

### get_members

Returns the membership details for specified member accounts for a behavior
graph.

Type annotations for `session.create_client("detective").get_members` method.

Boto3 documentation:
[Detective.Client.get_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.get_members)

Asynchronous method. Use `await get_members(...)` for a synchronous call.

Arguments mapping described in
[GetMembersRequestRequestTypeDef](./type_defs.md#getmembersrequestrequesttypedef).

Keyword-only arguments:

- `GraphArn`: `str` *(required)*
- `AccountIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[GetMembersResponseTypeDef](./type_defs.md#getmembersresponsetypedef).

<a id="list_graphs"></a>

### list_graphs

Returns the list of behavior graphs that the calling account is an
administrator account of.

Type annotations for `session.create_client("detective").list_graphs` method.

Boto3 documentation:
[Detective.Client.list_graphs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_graphs)

Asynchronous method. Use `await list_graphs(...)` for a synchronous call.

Arguments mapping described in
[ListGraphsRequestRequestTypeDef](./type_defs.md#listgraphsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListGraphsResponseTypeDef](./type_defs.md#listgraphsresponsetypedef).

<a id="list_invitations"></a>

### list_invitations

Retrieves the list of open and accepted behavior graph invitations for the
member account.

Type annotations for `session.create_client("detective").list_invitations`
method.

Boto3 documentation:
[Detective.Client.list_invitations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_invitations)

Asynchronous method. Use `await list_invitations(...)` for a synchronous call.

Arguments mapping described in
[ListInvitationsRequestRequestTypeDef](./type_defs.md#listinvitationsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef).

<a id="list_members"></a>

### list_members

Retrieves the list of member accounts for a behavior graph.

Type annotations for `session.create_client("detective").list_members` method.

Boto3 documentation:
[Detective.Client.list_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_members)

Asynchronous method. Use `await list_members(...)` for a synchronous call.

Arguments mapping described in
[ListMembersRequestRequestTypeDef](./type_defs.md#listmembersrequestrequesttypedef).

Keyword-only arguments:

- `GraphArn`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Returns the tag values that are assigned to a behavior graph.

Type annotations for
`session.create_client("detective").list_tags_for_resource` method.

Boto3 documentation:
[Detective.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="reject_invitation"></a>

### reject_invitation

Rejects an invitation to contribute the account data to a behavior graph.

Type annotations for `session.create_client("detective").reject_invitation`
method.

Boto3 documentation:
[Detective.Client.reject_invitation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.reject_invitation)

Asynchronous method. Use `await reject_invitation(...)` for a synchronous call.

Arguments mapping described in
[RejectInvitationRequestRequestTypeDef](./type_defs.md#rejectinvitationrequestrequesttypedef).

Keyword-only arguments:

- `GraphArn`: `str` *(required)*

<a id="start_monitoring_member"></a>

### start_monitoring_member

Sends a request to enable data ingest for a member account that has a status of
`ACCEPTED_BUT_DISABLED` .

Type annotations for
`session.create_client("detective").start_monitoring_member` method.

Boto3 documentation:
[Detective.Client.start_monitoring_member](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.start_monitoring_member)

Asynchronous method. Use `await start_monitoring_member(...)` for a synchronous
call.

Arguments mapping described in
[StartMonitoringMemberRequestRequestTypeDef](./type_defs.md#startmonitoringmemberrequestrequesttypedef).

Keyword-only arguments:

- `GraphArn`: `str` *(required)*
- `AccountId`: `str` *(required)*

<a id="tag_resource"></a>

### tag_resource

Applies tag values to a behavior graph.

Type annotations for `session.create_client("detective").tag_resource` method.

Boto3 documentation:
[Detective.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes tags from a behavior graph.

Type annotations for `session.create_client("detective").untag_resource`
method.

Boto3 documentation:
[Detective.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("detective").__aenter__` method.

Boto3 documentation:
[Detective.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [DetectiveClient](#detectiveclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("detective").__aexit__` method.

Boto3 documentation:
[Detective.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
