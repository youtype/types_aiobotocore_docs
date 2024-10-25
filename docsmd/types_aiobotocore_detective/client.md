# DetectiveClient

> [Index](../README.md) > [Detective](./README.md) > DetectiveClient

!!! note ""

    Auto-generated documentation for [Detective](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
    type annotations stubs module [types-aiobotocore-detective](https://pypi.org/project/types-aiobotocore-detective/).

## DetectiveClient

Type annotations and code completion for `#!python session.create_client("detective")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client)

```python
# DetectiveClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_detective.client import DetectiveClient

session = get_session()
async with session.create_client("detective") as client:
    client: DetectiveClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("detective").exceptions` structure.

```python
# DetectiveClient.exceptions usage example

async with session.create_client("detective") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.TooManyRequestsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# DetectiveClient usage type checking example

from types_aiobotocore_detective.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### accept\_invitation

Accepts an invitation for the member account to contribute data to a behavior
graph.

Type annotations and code completion for `#!python session.create_client("detective").accept_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.accept_invitation)

```python
# accept_invitation method definition

await def accept_invitation(
    self,
    *,
    GraphArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# accept_invitation method usage example with argument unpacking

kwargs: AcceptInvitationRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
}

parent.accept_invitation(**kwargs)
```

1. See [:material-code-braces: AcceptInvitationRequestRequestTypeDef](./type_defs.md#acceptinvitationrequestrequesttypedef) 

### batch\_get\_graph\_member\_datasources

Gets data source package information for the behavior graph.

Type annotations and code completion for `#!python session.create_client("detective").batch_get_graph_member_datasources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.batch_get_graph_member_datasources)

```python
# batch_get_graph_member_datasources method definition

await def batch_get_graph_member_datasources(
    self,
    *,
    GraphArn: str,
    AccountIds: Sequence[str],
) -> BatchGetGraphMemberDatasourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetGraphMemberDatasourcesResponseTypeDef](./type_defs.md#batchgetgraphmemberdatasourcesresponsetypedef) 


```python
# batch_get_graph_member_datasources method usage example with argument unpacking

kwargs: BatchGetGraphMemberDatasourcesRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
    "AccountIds": ...,
}

parent.batch_get_graph_member_datasources(**kwargs)
```

1. See [:material-code-braces: BatchGetGraphMemberDatasourcesRequestRequestTypeDef](./type_defs.md#batchgetgraphmemberdatasourcesrequestrequesttypedef) 

### batch\_get\_membership\_datasources

Gets information on the data source package history for an account.

Type annotations and code completion for `#!python session.create_client("detective").batch_get_membership_datasources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.batch_get_membership_datasources)

```python
# batch_get_membership_datasources method definition

await def batch_get_membership_datasources(
    self,
    *,
    GraphArns: Sequence[str],
) -> BatchGetMembershipDatasourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetMembershipDatasourcesResponseTypeDef](./type_defs.md#batchgetmembershipdatasourcesresponsetypedef) 


```python
# batch_get_membership_datasources method usage example with argument unpacking

kwargs: BatchGetMembershipDatasourcesRequestRequestTypeDef = {  # (1)
    "GraphArns": ...,
}

parent.batch_get_membership_datasources(**kwargs)
```

1. See [:material-code-braces: BatchGetMembershipDatasourcesRequestRequestTypeDef](./type_defs.md#batchgetmembershipdatasourcesrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("detective").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("detective").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_graph

Creates a new behavior graph for the calling account, and sets that account as
the administrator
account.

Type annotations and code completion for `#!python session.create_client("detective").create_graph` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.create_graph)

```python
# create_graph method definition

await def create_graph(
    self,
    *,
    Tags: Mapping[str, str] = ...,
) -> CreateGraphResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateGraphResponseTypeDef](./type_defs.md#creategraphresponsetypedef) 


```python
# create_graph method usage example with argument unpacking

kwargs: CreateGraphRequestRequestTypeDef = {  # (1)
    "Tags": ...,
}

parent.create_graph(**kwargs)
```

1. See [:material-code-braces: CreateGraphRequestRequestTypeDef](./type_defs.md#creategraphrequestrequesttypedef) 

### create\_members

`CreateMembers` is used to send invitations to accounts.

Type annotations and code completion for `#!python session.create_client("detective").create_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.create_members)

```python
# create_members method definition

await def create_members(
    self,
    *,
    GraphArn: str,
    Accounts: Sequence[AccountTypeDef],  # (1)
    Message: str = ...,
    DisableEmailNotification: bool = ...,
) -> CreateMembersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: CreateMembersResponseTypeDef](./type_defs.md#createmembersresponsetypedef) 


```python
# create_members method usage example with argument unpacking

kwargs: CreateMembersRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
    "Accounts": ...,
}

parent.create_members(**kwargs)
```

1. See [:material-code-braces: CreateMembersRequestRequestTypeDef](./type_defs.md#createmembersrequestrequesttypedef) 

### delete\_graph

Disables the specified behavior graph and queues it to be deleted.

Type annotations and code completion for `#!python session.create_client("detective").delete_graph` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.delete_graph)

```python
# delete_graph method definition

await def delete_graph(
    self,
    *,
    GraphArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_graph method usage example with argument unpacking

kwargs: DeleteGraphRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
}

parent.delete_graph(**kwargs)
```

1. See [:material-code-braces: DeleteGraphRequestRequestTypeDef](./type_defs.md#deletegraphrequestrequesttypedef) 

### delete\_members

Removes the specified member accounts from the behavior graph.

Type annotations and code completion for `#!python session.create_client("detective").delete_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.delete_members)

```python
# delete_members method definition

await def delete_members(
    self,
    *,
    GraphArn: str,
    AccountIds: Sequence[str],
) -> DeleteMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMembersResponseTypeDef](./type_defs.md#deletemembersresponsetypedef) 


```python
# delete_members method usage example with argument unpacking

kwargs: DeleteMembersRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
    "AccountIds": ...,
}

parent.delete_members(**kwargs)
```

1. See [:material-code-braces: DeleteMembersRequestRequestTypeDef](./type_defs.md#deletemembersrequestrequesttypedef) 

### describe\_organization\_configuration

Returns information about the configuration for the organization behavior graph.

Type annotations and code completion for `#!python session.create_client("detective").describe_organization_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.describe_organization_configuration)

```python
# describe_organization_configuration method definition

await def describe_organization_configuration(
    self,
    *,
    GraphArn: str,
) -> DescribeOrganizationConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOrganizationConfigurationResponseTypeDef](./type_defs.md#describeorganizationconfigurationresponsetypedef) 


```python
# describe_organization_configuration method usage example with argument unpacking

kwargs: DescribeOrganizationConfigurationRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
}

parent.describe_organization_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#describeorganizationconfigurationrequestrequesttypedef) 

### disable\_organization\_admin\_account

Removes the Detective administrator account in the current Region.

Type annotations and code completion for `#!python session.create_client("detective").disable_organization_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.disable_organization_admin_account)

```python
# disable_organization_admin_account method definition

await def disable_organization_admin_account(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 

### disassociate\_membership

Removes the member account from the specified behavior graph.

Type annotations and code completion for `#!python session.create_client("detective").disassociate_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.disassociate_membership)

```python
# disassociate_membership method definition

await def disassociate_membership(
    self,
    *,
    GraphArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_membership method usage example with argument unpacking

kwargs: DisassociateMembershipRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
}

parent.disassociate_membership(**kwargs)
```

1. See [:material-code-braces: DisassociateMembershipRequestRequestTypeDef](./type_defs.md#disassociatemembershiprequestrequesttypedef) 

### enable\_organization\_admin\_account

Designates the Detective administrator account for the organization in the
current
Region.

Type annotations and code completion for `#!python session.create_client("detective").enable_organization_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.enable_organization_admin_account)

```python
# enable_organization_admin_account method definition

await def enable_organization_admin_account(
    self,
    *,
    AccountId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# enable_organization_admin_account method usage example with argument unpacking

kwargs: EnableOrganizationAdminAccountRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.enable_organization_admin_account(**kwargs)
```

1. See [:material-code-braces: EnableOrganizationAdminAccountRequestRequestTypeDef](./type_defs.md#enableorganizationadminaccountrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("detective").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.generate_presigned_url)

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


### get\_investigation

Detective investigations lets you investigate IAM users and IAM roles using
indicators of
compromise.

Type annotations and code completion for `#!python session.create_client("detective").get_investigation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.get_investigation)

```python
# get_investigation method definition

await def get_investigation(
    self,
    *,
    GraphArn: str,
    InvestigationId: str,
) -> GetInvestigationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInvestigationResponseTypeDef](./type_defs.md#getinvestigationresponsetypedef) 


```python
# get_investigation method usage example with argument unpacking

kwargs: GetInvestigationRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
    "InvestigationId": ...,
}

parent.get_investigation(**kwargs)
```

1. See [:material-code-braces: GetInvestigationRequestRequestTypeDef](./type_defs.md#getinvestigationrequestrequesttypedef) 

### get\_members

Returns the membership details for specified member accounts for a behavior
graph.

Type annotations and code completion for `#!python session.create_client("detective").get_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.get_members)

```python
# get_members method definition

await def get_members(
    self,
    *,
    GraphArn: str,
    AccountIds: Sequence[str],
) -> GetMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMembersResponseTypeDef](./type_defs.md#getmembersresponsetypedef) 


```python
# get_members method usage example with argument unpacking

kwargs: GetMembersRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
    "AccountIds": ...,
}

parent.get_members(**kwargs)
```

1. See [:material-code-braces: GetMembersRequestRequestTypeDef](./type_defs.md#getmembersrequestrequesttypedef) 

### list\_datasource\_packages

Lists data source packages in the behavior graph.

Type annotations and code completion for `#!python session.create_client("detective").list_datasource_packages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_datasource_packages)

```python
# list_datasource_packages method definition

await def list_datasource_packages(
    self,
    *,
    GraphArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDatasourcePackagesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDatasourcePackagesResponseTypeDef](./type_defs.md#listdatasourcepackagesresponsetypedef) 


```python
# list_datasource_packages method usage example with argument unpacking

kwargs: ListDatasourcePackagesRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
}

parent.list_datasource_packages(**kwargs)
```

1. See [:material-code-braces: ListDatasourcePackagesRequestRequestTypeDef](./type_defs.md#listdatasourcepackagesrequestrequesttypedef) 

### list\_graphs

Returns the list of behavior graphs that the calling account is an
administrator account
of.

Type annotations and code completion for `#!python session.create_client("detective").list_graphs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_graphs)

```python
# list_graphs method definition

await def list_graphs(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListGraphsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGraphsResponseTypeDef](./type_defs.md#listgraphsresponsetypedef) 


```python
# list_graphs method usage example with argument unpacking

kwargs: ListGraphsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_graphs(**kwargs)
```

1. See [:material-code-braces: ListGraphsRequestRequestTypeDef](./type_defs.md#listgraphsrequestrequesttypedef) 

### list\_indicators

Gets the indicators from an investigation.

Type annotations and code completion for `#!python session.create_client("detective").list_indicators` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_indicators)

```python
# list_indicators method definition

await def list_indicators(
    self,
    *,
    GraphArn: str,
    InvestigationId: str,
    IndicatorType: IndicatorTypeType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListIndicatorsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: IndicatorTypeType](./literals.md#indicatortypetype) 
2. See [:material-code-braces: ListIndicatorsResponseTypeDef](./type_defs.md#listindicatorsresponsetypedef) 


```python
# list_indicators method usage example with argument unpacking

kwargs: ListIndicatorsRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
    "InvestigationId": ...,
}

parent.list_indicators(**kwargs)
```

1. See [:material-code-braces: ListIndicatorsRequestRequestTypeDef](./type_defs.md#listindicatorsrequestrequesttypedef) 

### list\_investigations

Detective investigations lets you investigate IAM users and IAM roles using
indicators of
compromise.

Type annotations and code completion for `#!python session.create_client("detective").list_investigations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_investigations)

```python
# list_investigations method definition

await def list_investigations(
    self,
    *,
    GraphArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    FilterCriteria: FilterCriteriaTypeDef = ...,  # (1)
    SortCriteria: SortCriteriaTypeDef = ...,  # (2)
) -> ListInvestigationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
3. See [:material-code-braces: ListInvestigationsResponseTypeDef](./type_defs.md#listinvestigationsresponsetypedef) 


```python
# list_investigations method usage example with argument unpacking

kwargs: ListInvestigationsRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
}

parent.list_investigations(**kwargs)
```

1. See [:material-code-braces: ListInvestigationsRequestRequestTypeDef](./type_defs.md#listinvestigationsrequestrequesttypedef) 

### list\_invitations

Retrieves the list of open and accepted behavior graph invitations for the
member
account.

Type annotations and code completion for `#!python session.create_client("detective").list_invitations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_invitations)

```python
# list_invitations method definition

await def list_invitations(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListInvitationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef) 


```python
# list_invitations method usage example with argument unpacking

kwargs: ListInvitationsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_invitations(**kwargs)
```

1. See [:material-code-braces: ListInvitationsRequestRequestTypeDef](./type_defs.md#listinvitationsrequestrequesttypedef) 

### list\_members

Retrieves the list of member accounts for a behavior graph.

Type annotations and code completion for `#!python session.create_client("detective").list_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_members)

```python
# list_members method definition

await def list_members(
    self,
    *,
    GraphArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef) 


```python
# list_members method usage example with argument unpacking

kwargs: ListMembersRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
}

parent.list_members(**kwargs)
```

1. See [:material-code-braces: ListMembersRequestRequestTypeDef](./type_defs.md#listmembersrequestrequesttypedef) 

### list\_organization\_admin\_accounts

Returns information about the Detective administrator account for an
organization.

Type annotations and code completion for `#!python session.create_client("detective").list_organization_admin_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_organization_admin_accounts)

```python
# list_organization_admin_accounts method definition

await def list_organization_admin_accounts(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListOrganizationAdminAccountsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef) 


```python
# list_organization_admin_accounts method usage example with argument unpacking

kwargs: ListOrganizationAdminAccountsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_organization_admin_accounts(**kwargs)
```

1. See [:material-code-braces: ListOrganizationAdminAccountsRequestRequestTypeDef](./type_defs.md#listorganizationadminaccountsrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns the tag values that are assigned to a behavior graph.

Type annotations and code completion for `#!python session.create_client("detective").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_tags_for_resource)

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

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### reject\_invitation

Rejects an invitation to contribute the account data to a behavior graph.

Type annotations and code completion for `#!python session.create_client("detective").reject_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.reject_invitation)

```python
# reject_invitation method definition

await def reject_invitation(
    self,
    *,
    GraphArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# reject_invitation method usage example with argument unpacking

kwargs: RejectInvitationRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
}

parent.reject_invitation(**kwargs)
```

1. See [:material-code-braces: RejectInvitationRequestRequestTypeDef](./type_defs.md#rejectinvitationrequestrequesttypedef) 

### start\_investigation

Detective investigations lets you investigate IAM users and IAM roles using
indicators of
compromise.

Type annotations and code completion for `#!python session.create_client("detective").start_investigation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.start_investigation)

```python
# start_investigation method definition

await def start_investigation(
    self,
    *,
    GraphArn: str,
    EntityArn: str,
    ScopeStartTime: TimestampTypeDef,
    ScopeEndTime: TimestampTypeDef,
) -> StartInvestigationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartInvestigationResponseTypeDef](./type_defs.md#startinvestigationresponsetypedef) 


```python
# start_investigation method usage example with argument unpacking

kwargs: StartInvestigationRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
    "EntityArn": ...,
    "ScopeStartTime": ...,
    "ScopeEndTime": ...,
}

parent.start_investigation(**kwargs)
```

1. See [:material-code-braces: StartInvestigationRequestRequestTypeDef](./type_defs.md#startinvestigationrequestrequesttypedef) 

### start\_monitoring\_member

Sends a request to enable data ingest for a member account that has a status of
`ACCEPTED_BUT_DISABLED`.

Type annotations and code completion for `#!python session.create_client("detective").start_monitoring_member` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.start_monitoring_member)

```python
# start_monitoring_member method definition

await def start_monitoring_member(
    self,
    *,
    GraphArn: str,
    AccountId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_monitoring_member method usage example with argument unpacking

kwargs: StartMonitoringMemberRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
    "AccountId": ...,
}

parent.start_monitoring_member(**kwargs)
```

1. See [:material-code-braces: StartMonitoringMemberRequestRequestTypeDef](./type_defs.md#startmonitoringmemberrequestrequesttypedef) 

### tag\_resource

Applies tag values to a behavior graph.

Type annotations and code completion for `#!python session.create_client("detective").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.tag_resource)

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

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from a behavior graph.

Type annotations and code completion for `#!python session.create_client("detective").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.untag_resource)

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

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_datasource\_packages

Starts a data source packages for the behavior graph.

Type annotations and code completion for `#!python session.create_client("detective").update_datasource_packages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.update_datasource_packages)

```python
# update_datasource_packages method definition

await def update_datasource_packages(
    self,
    *,
    GraphArn: str,
    DatasourcePackages: Sequence[DatasourcePackageType],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DatasourcePackageType](./literals.md#datasourcepackagetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_datasource_packages method usage example with argument unpacking

kwargs: UpdateDatasourcePackagesRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
    "DatasourcePackages": ...,
}

parent.update_datasource_packages(**kwargs)
```

1. See [:material-code-braces: UpdateDatasourcePackagesRequestRequestTypeDef](./type_defs.md#updatedatasourcepackagesrequestrequesttypedef) 

### update\_investigation\_state

Updates the state of an investigation.

Type annotations and code completion for `#!python session.create_client("detective").update_investigation_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.update_investigation_state)

```python
# update_investigation_state method definition

await def update_investigation_state(
    self,
    *,
    GraphArn: str,
    InvestigationId: str,
    State: StateType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_investigation_state method usage example with argument unpacking

kwargs: UpdateInvestigationStateRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
    "InvestigationId": ...,
    "State": ...,
}

parent.update_investigation_state(**kwargs)
```

1. See [:material-code-braces: UpdateInvestigationStateRequestRequestTypeDef](./type_defs.md#updateinvestigationstaterequestrequesttypedef) 

### update\_organization\_configuration

Updates the configuration for the Organizations integration in the current
Region.

Type annotations and code completion for `#!python session.create_client("detective").update_organization_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.update_organization_configuration)

```python
# update_organization_configuration method definition

await def update_organization_configuration(
    self,
    *,
    GraphArn: str,
    AutoEnable: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_organization_configuration method usage example with argument unpacking

kwargs: UpdateOrganizationConfigurationRequestRequestTypeDef = {  # (1)
    "GraphArn": ...,
}

parent.update_organization_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#updateorganizationconfigurationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("detective").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "DetectiveClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("detective").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.__aexit__)

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





