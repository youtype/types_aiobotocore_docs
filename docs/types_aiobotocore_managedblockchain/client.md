<a id="managedblockchainclient-for-aiobotocore-managedblockchain-module"></a>

# ManagedBlockchainClient for aiobotocore ManagedBlockchain module

> [Index](../README.md) > [ManagedBlockchain](./README.md) >
> ManagedBlockchainClient

Auto-generated documentation for
[ManagedBlockchain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
type annotations stubs module
[types-aiobotocore-managedblockchain](https://pypi.org/project/types-aiobotocore-managedblockchain/).

- [ManagedBlockchainClient for aiobotocore ManagedBlockchain module](#managedblockchainclient-for-aiobotocore-managedblockchain-module)
  - [ManagedBlockchainClient](#managedblockchainclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_member](#create_member)
    - [create_network](#create_network)
    - [create_node](#create_node)
    - [create_proposal](#create_proposal)
    - [delete_member](#delete_member)
    - [delete_node](#delete_node)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_member](#get_member)
    - [get_network](#get_network)
    - [get_node](#get_node)
    - [get_proposal](#get_proposal)
    - [list_invitations](#list_invitations)
    - [list_members](#list_members)
    - [list_networks](#list_networks)
    - [list_nodes](#list_nodes)
    - [list_proposal_votes](#list_proposal_votes)
    - [list_proposals](#list_proposals)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [reject_invitation](#reject_invitation)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_member](#update_member)
    - [update_node](#update_node)
    - [vote_on_proposal](#vote_on_proposal)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="managedblockchainclient"></a>

## ManagedBlockchainClient

Type annotations for `session.create_client("managedblockchain")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_managedblockchain.client import ManagedBlockchainClient

session = get_session()
async with session.create_client("managedblockchain") as client:
    client: ManagedBlockchainClient
```

Boto3 documentation:
[ManagedBlockchain.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_managedblockchain.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.IllegalActionException`
- `Exceptions.InternalServiceErrorException`
- `Exceptions.InvalidRequestException`
- `Exceptions.ResourceAlreadyExistsException`
- `Exceptions.ResourceLimitExceededException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ResourceNotReadyException`
- `Exceptions.ThrottlingException`
- `Exceptions.TooManyTagsException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ManagedBlockchainClient exceptions.

Type annotations for `session.create_client("managedblockchain").exceptions`
method.

Boto3 documentation:
[ManagedBlockchain.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("managedblockchain").can_paginate`
method.

Boto3 documentation:
[ManagedBlockchain.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_member"></a>

### create_member

Creates a member within a Managed Blockchain network.

Type annotations for `session.create_client("managedblockchain").create_member`
method.

Boto3 documentation:
[ManagedBlockchain.Client.create_member](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_member)

Asynchronous method. Use `await create_member(...)` for a synchronous call.

Arguments mapping described in
[CreateMemberInputRequestTypeDef](./type_defs.md#creatememberinputrequesttypedef).

Keyword-only arguments:

- `ClientRequestToken`: `str` *(required)*
- `InvitationId`: `str` *(required)*
- `NetworkId`: `str` *(required)*
- `MemberConfiguration`:
  [MemberConfigurationTypeDef](./type_defs.md#memberconfigurationtypedef)
  *(required)*

Returns a `Coroutine` for
[CreateMemberOutputTypeDef](./type_defs.md#creatememberoutputtypedef).

<a id="create\_network"></a>

### create_network

Creates a new blockchain network using Amazon Managed Blockchain.

Type annotations for
`session.create_client("managedblockchain").create_network` method.

Boto3 documentation:
[ManagedBlockchain.Client.create_network](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_network)

Asynchronous method. Use `await create_network(...)` for a synchronous call.

Arguments mapping described in
[CreateNetworkInputRequestTypeDef](./type_defs.md#createnetworkinputrequesttypedef).

Keyword-only arguments:

- `ClientRequestToken`: `str` *(required)*
- `Name`: `str` *(required)*
- `Framework`: [FrameworkType](./literals.md#frameworktype) *(required)*
- `FrameworkVersion`: `str` *(required)*
- `VotingPolicy`: [VotingPolicyTypeDef](./type_defs.md#votingpolicytypedef)
  *(required)*
- `MemberConfiguration`:
  [MemberConfigurationTypeDef](./type_defs.md#memberconfigurationtypedef)
  *(required)*
- `Description`: `str`
- `FrameworkConfiguration`:
  [NetworkFrameworkConfigurationTypeDef](./type_defs.md#networkframeworkconfigurationtypedef)
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateNetworkOutputTypeDef](./type_defs.md#createnetworkoutputtypedef).

<a id="create\_node"></a>

### create_node

Creates a node on the specified blockchain network.

Type annotations for `session.create_client("managedblockchain").create_node`
method.

Boto3 documentation:
[ManagedBlockchain.Client.create_node](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_node)

Asynchronous method. Use `await create_node(...)` for a synchronous call.

Arguments mapping described in
[CreateNodeInputRequestTypeDef](./type_defs.md#createnodeinputrequesttypedef).

Keyword-only arguments:

- `ClientRequestToken`: `str` *(required)*
- `NetworkId`: `str` *(required)*
- `NodeConfiguration`:
  [NodeConfigurationTypeDef](./type_defs.md#nodeconfigurationtypedef)
  *(required)*
- `MemberId`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateNodeOutputTypeDef](./type_defs.md#createnodeoutputtypedef).

<a id="create\_proposal"></a>

### create_proposal

Creates a proposal for a change to the network that other members of the
network can vote on, for example, a proposal to add a new member to the
network.

Type annotations for
`session.create_client("managedblockchain").create_proposal` method.

Boto3 documentation:
[ManagedBlockchain.Client.create_proposal](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.create_proposal)

Asynchronous method. Use `await create_proposal(...)` for a synchronous call.

Arguments mapping described in
[CreateProposalInputRequestTypeDef](./type_defs.md#createproposalinputrequesttypedef).

Keyword-only arguments:

- `ClientRequestToken`: `str` *(required)*
- `NetworkId`: `str` *(required)*
- `MemberId`: `str` *(required)*
- `Actions`: [ProposalActionsTypeDef](./type_defs.md#proposalactionstypedef)
  *(required)*
- `Description`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateProposalOutputTypeDef](./type_defs.md#createproposaloutputtypedef).

<a id="delete\_member"></a>

### delete_member

Deletes a member.

Type annotations for `session.create_client("managedblockchain").delete_member`
method.

Boto3 documentation:
[ManagedBlockchain.Client.delete_member](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.delete_member)

Asynchronous method. Use `await delete_member(...)` for a synchronous call.

Arguments mapping described in
[DeleteMemberInputRequestTypeDef](./type_defs.md#deletememberinputrequesttypedef).

Keyword-only arguments:

- `NetworkId`: `str` *(required)*
- `MemberId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_node"></a>

### delete_node

Deletes a node that your AWS account owns.

Type annotations for `session.create_client("managedblockchain").delete_node`
method.

Boto3 documentation:
[ManagedBlockchain.Client.delete_node](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.delete_node)

Asynchronous method. Use `await delete_node(...)` for a synchronous call.

Arguments mapping described in
[DeleteNodeInputRequestTypeDef](./type_defs.md#deletenodeinputrequesttypedef).

Keyword-only arguments:

- `NetworkId`: `str` *(required)*
- `NodeId`: `str` *(required)*
- `MemberId`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("managedblockchain").generate_presigned_url` method.

Boto3 documentation:
[ManagedBlockchain.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_member"></a>

### get_member

Returns detailed information about a member.

Type annotations for `session.create_client("managedblockchain").get_member`
method.

Boto3 documentation:
[ManagedBlockchain.Client.get_member](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_member)

Asynchronous method. Use `await get_member(...)` for a synchronous call.

Arguments mapping described in
[GetMemberInputRequestTypeDef](./type_defs.md#getmemberinputrequesttypedef).

Keyword-only arguments:

- `NetworkId`: `str` *(required)*
- `MemberId`: `str` *(required)*

Returns a `Coroutine` for
[GetMemberOutputTypeDef](./type_defs.md#getmemberoutputtypedef).

<a id="get\_network"></a>

### get_network

Returns detailed information about a network.

Type annotations for `session.create_client("managedblockchain").get_network`
method.

Boto3 documentation:
[ManagedBlockchain.Client.get_network](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_network)

Asynchronous method. Use `await get_network(...)` for a synchronous call.

Arguments mapping described in
[GetNetworkInputRequestTypeDef](./type_defs.md#getnetworkinputrequesttypedef).

Keyword-only arguments:

- `NetworkId`: `str` *(required)*

Returns a `Coroutine` for
[GetNetworkOutputTypeDef](./type_defs.md#getnetworkoutputtypedef).

<a id="get\_node"></a>

### get_node

Returns detailed information about a node.

Type annotations for `session.create_client("managedblockchain").get_node`
method.

Boto3 documentation:
[ManagedBlockchain.Client.get_node](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_node)

Asynchronous method. Use `await get_node(...)` for a synchronous call.

Arguments mapping described in
[GetNodeInputRequestTypeDef](./type_defs.md#getnodeinputrequesttypedef).

Keyword-only arguments:

- `NetworkId`: `str` *(required)*
- `NodeId`: `str` *(required)*
- `MemberId`: `str`

Returns a `Coroutine` for
[GetNodeOutputTypeDef](./type_defs.md#getnodeoutputtypedef).

<a id="get\_proposal"></a>

### get_proposal

Returns detailed information about a proposal.

Type annotations for `session.create_client("managedblockchain").get_proposal`
method.

Boto3 documentation:
[ManagedBlockchain.Client.get_proposal](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.get_proposal)

Asynchronous method. Use `await get_proposal(...)` for a synchronous call.

Arguments mapping described in
[GetProposalInputRequestTypeDef](./type_defs.md#getproposalinputrequesttypedef).

Keyword-only arguments:

- `NetworkId`: `str` *(required)*
- `ProposalId`: `str` *(required)*

Returns a `Coroutine` for
[GetProposalOutputTypeDef](./type_defs.md#getproposaloutputtypedef).

<a id="list\_invitations"></a>

### list_invitations

Returns a list of all invitations for the current AWS account.

Type annotations for
`session.create_client("managedblockchain").list_invitations` method.

Boto3 documentation:
[ManagedBlockchain.Client.list_invitations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_invitations)

Asynchronous method. Use `await list_invitations(...)` for a synchronous call.

Arguments mapping described in
[ListInvitationsInputRequestTypeDef](./type_defs.md#listinvitationsinputrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListInvitationsOutputTypeDef](./type_defs.md#listinvitationsoutputtypedef).

<a id="list\_members"></a>

### list_members

Returns a list of the members in a network and properties of their
configurations.

Type annotations for `session.create_client("managedblockchain").list_members`
method.

Boto3 documentation:
[ManagedBlockchain.Client.list_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_members)

Asynchronous method. Use `await list_members(...)` for a synchronous call.

Arguments mapping described in
[ListMembersInputRequestTypeDef](./type_defs.md#listmembersinputrequesttypedef).

Keyword-only arguments:

- `NetworkId`: `str` *(required)*
- `Name`: `str`
- `Status`: [MemberStatusType](./literals.md#memberstatustype)
- `IsOwned`: `bool`
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListMembersOutputTypeDef](./type_defs.md#listmembersoutputtypedef).

<a id="list\_networks"></a>

### list_networks

Returns information about the networks in which the current AWS account
participates.

Type annotations for `session.create_client("managedblockchain").list_networks`
method.

Boto3 documentation:
[ManagedBlockchain.Client.list_networks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_networks)

Asynchronous method. Use `await list_networks(...)` for a synchronous call.

Arguments mapping described in
[ListNetworksInputRequestTypeDef](./type_defs.md#listnetworksinputrequesttypedef).

Keyword-only arguments:

- `Name`: `str`
- `Framework`: [FrameworkType](./literals.md#frameworktype)
- `Status`: [NetworkStatusType](./literals.md#networkstatustype)
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListNetworksOutputTypeDef](./type_defs.md#listnetworksoutputtypedef).

<a id="list\_nodes"></a>

### list_nodes

Returns information about the nodes within a network.

Type annotations for `session.create_client("managedblockchain").list_nodes`
method.

Boto3 documentation:
[ManagedBlockchain.Client.list_nodes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_nodes)

Asynchronous method. Use `await list_nodes(...)` for a synchronous call.

Arguments mapping described in
[ListNodesInputRequestTypeDef](./type_defs.md#listnodesinputrequesttypedef).

Keyword-only arguments:

- `NetworkId`: `str` *(required)*
- `MemberId`: `str`
- `Status`: [NodeStatusType](./literals.md#nodestatustype)
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListNodesOutputTypeDef](./type_defs.md#listnodesoutputtypedef).

<a id="list\_proposal\_votes"></a>

### list_proposal_votes

Returns the list of votes for a specified proposal, including the value of each
vote and the unique identifier of the member that cast the vote.

Type annotations for
`session.create_client("managedblockchain").list_proposal_votes` method.

Boto3 documentation:
[ManagedBlockchain.Client.list_proposal_votes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_proposal_votes)

Asynchronous method. Use `await list_proposal_votes(...)` for a synchronous
call.

Arguments mapping described in
[ListProposalVotesInputRequestTypeDef](./type_defs.md#listproposalvotesinputrequesttypedef).

Keyword-only arguments:

- `NetworkId`: `str` *(required)*
- `ProposalId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListProposalVotesOutputTypeDef](./type_defs.md#listproposalvotesoutputtypedef).

<a id="list\_proposals"></a>

### list_proposals

Returns a list of proposals for the network.

Type annotations for
`session.create_client("managedblockchain").list_proposals` method.

Boto3 documentation:
[ManagedBlockchain.Client.list_proposals](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_proposals)

Asynchronous method. Use `await list_proposals(...)` for a synchronous call.

Arguments mapping described in
[ListProposalsInputRequestTypeDef](./type_defs.md#listproposalsinputrequesttypedef).

Keyword-only arguments:

- `NetworkId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListProposalsOutputTypeDef](./type_defs.md#listproposalsoutputtypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Returns a list of tags for the specified resource.

Type annotations for
`session.create_client("managedblockchain").list_tags_for_resource` method.

Boto3 documentation:
[ManagedBlockchain.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="reject\_invitation"></a>

### reject_invitation

Rejects an invitation to join a network.

Type annotations for
`session.create_client("managedblockchain").reject_invitation` method.

Boto3 documentation:
[ManagedBlockchain.Client.reject_invitation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.reject_invitation)

Asynchronous method. Use `await reject_invitation(...)` for a synchronous call.

Arguments mapping described in
[RejectInvitationInputRequestTypeDef](./type_defs.md#rejectinvitationinputrequesttypedef).

Keyword-only arguments:

- `InvitationId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="tag\_resource"></a>

### tag_resource

Adds or overwrites the specified tags for the specified Amazon Managed
Blockchain resource.

Type annotations for `session.create_client("managedblockchain").tag_resource`
method.

Boto3 documentation:
[ManagedBlockchain.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Removes the specified tags from the Amazon Managed Blockchain resource.

Type annotations for
`session.create_client("managedblockchain").untag_resource` method.

Boto3 documentation:
[ManagedBlockchain.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_member"></a>

### update_member

Updates a member configuration with new parameters.

Type annotations for `session.create_client("managedblockchain").update_member`
method.

Boto3 documentation:
[ManagedBlockchain.Client.update_member](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_member)

Asynchronous method. Use `await update_member(...)` for a synchronous call.

Arguments mapping described in
[UpdateMemberInputRequestTypeDef](./type_defs.md#updatememberinputrequesttypedef).

Keyword-only arguments:

- `NetworkId`: `str` *(required)*
- `MemberId`: `str` *(required)*
- `LogPublishingConfiguration`:
  [MemberLogPublishingConfigurationTypeDef](./type_defs.md#memberlogpublishingconfigurationtypedef)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_node"></a>

### update_node

Updates a node configuration with new parameters.

Type annotations for `session.create_client("managedblockchain").update_node`
method.

Boto3 documentation:
[ManagedBlockchain.Client.update_node](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.update_node)

Asynchronous method. Use `await update_node(...)` for a synchronous call.

Arguments mapping described in
[UpdateNodeInputRequestTypeDef](./type_defs.md#updatenodeinputrequesttypedef).

Keyword-only arguments:

- `NetworkId`: `str` *(required)*
- `NodeId`: `str` *(required)*
- `MemberId`: `str`
- `LogPublishingConfiguration`:
  [NodeLogPublishingConfigurationTypeDef](./type_defs.md#nodelogpublishingconfigurationtypedef)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="vote\_on\_proposal"></a>

### vote_on_proposal

Casts a vote for a specified `ProposalId` on behalf of a member.

Type annotations for
`session.create_client("managedblockchain").vote_on_proposal` method.

Boto3 documentation:
[ManagedBlockchain.Client.vote_on_proposal](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.vote_on_proposal)

Asynchronous method. Use `await vote_on_proposal(...)` for a synchronous call.

Arguments mapping described in
[VoteOnProposalInputRequestTypeDef](./type_defs.md#voteonproposalinputrequesttypedef).

Keyword-only arguments:

- `NetworkId`: `str` *(required)*
- `ProposalId`: `str` *(required)*
- `VoterMemberId`: `str` *(required)*
- `Vote`: [VoteValueType](./literals.md#votevaluetype) *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("managedblockchain").__aenter__`
method.

Boto3 documentation:
[ManagedBlockchain.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [ManagedBlockchainClient](#managedblockchainclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("managedblockchain").__aexit__`
method.

Boto3 documentation:
[ManagedBlockchain.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
