# Paginators

> [Index](../README.md) > [PartnerCentralSellingAPI](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [PartnerCentralSellingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#partnercentralsellingapi)
    type annotations stubs module [types-aiobotocore-partnercentral-selling](https://pypi.org/project/types-aiobotocore-partnercentral-selling/).

## ListEngagementByAcceptingInvitationTasksPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_paginator("list_engagement_by_accepting_invitation_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/paginator/ListEngagementByAcceptingInvitationTasks.html#PartnerCentralSellingAPI.Paginator.ListEngagementByAcceptingInvitationTasks)

```python
# ListEngagementByAcceptingInvitationTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_selling.paginator import ListEngagementByAcceptingInvitationTasksPaginator

session = get_session()
async with session.create_client("partnercentral-selling") as client:  # (1)
    paginator: ListEngagementByAcceptingInvitationTasksPaginator = client.get_paginator("list_engagement_by_accepting_invitation_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListEngagementByAcceptingInvitationTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. paginator: [ListEngagementByAcceptingInvitationTasksPaginator](./paginators.md#listengagementbyacceptinginvitationtaskspaginator)
3. item: [:material-code-braces: ListEngagementByAcceptingInvitationTasksResponseTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEngagementByAcceptingInvitationTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    EngagementInvitationIdentifier: Sequence[str] = ...,
    OpportunityIdentifier: Sequence[str] = ...,
    Sort: ListTasksSortBaseTypeDef = ...,  # (1)
    TaskIdentifier: Sequence[str] = ...,
    TaskStatus: Sequence[TaskStatusType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListEngagementByAcceptingInvitationTasksResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ListTasksSortBaseTypeDef](./type_defs.md#listtaskssortbasetypedef) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListEngagementByAcceptingInvitationTasksResponseTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEngagementByAcceptingInvitationTasksRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEngagementByAcceptingInvitationTasksRequestPaginateTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksrequestpaginatetypedef) 
## ListEngagementFromOpportunityTasksPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_paginator("list_engagement_from_opportunity_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/paginator/ListEngagementFromOpportunityTasks.html#PartnerCentralSellingAPI.Paginator.ListEngagementFromOpportunityTasks)

```python
# ListEngagementFromOpportunityTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_selling.paginator import ListEngagementFromOpportunityTasksPaginator

session = get_session()
async with session.create_client("partnercentral-selling") as client:  # (1)
    paginator: ListEngagementFromOpportunityTasksPaginator = client.get_paginator("list_engagement_from_opportunity_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListEngagementFromOpportunityTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. paginator: [ListEngagementFromOpportunityTasksPaginator](./paginators.md#listengagementfromopportunitytaskspaginator)
3. item: [:material-code-braces: ListEngagementFromOpportunityTasksResponseTypeDef](./type_defs.md#listengagementfromopportunitytasksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEngagementFromOpportunityTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    EngagementIdentifier: Sequence[str] = ...,
    OpportunityIdentifier: Sequence[str] = ...,
    Sort: ListTasksSortBaseTypeDef = ...,  # (1)
    TaskIdentifier: Sequence[str] = ...,
    TaskStatus: Sequence[TaskStatusType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListEngagementFromOpportunityTasksResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ListTasksSortBaseTypeDef](./type_defs.md#listtaskssortbasetypedef) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListEngagementFromOpportunityTasksResponseTypeDef](./type_defs.md#listengagementfromopportunitytasksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEngagementFromOpportunityTasksRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEngagementFromOpportunityTasksRequestPaginateTypeDef](./type_defs.md#listengagementfromopportunitytasksrequestpaginatetypedef) 
## ListEngagementInvitationsPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_paginator("list_engagement_invitations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/paginator/ListEngagementInvitations.html#PartnerCentralSellingAPI.Paginator.ListEngagementInvitations)

```python
# ListEngagementInvitationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_selling.paginator import ListEngagementInvitationsPaginator

session = get_session()
async with session.create_client("partnercentral-selling") as client:  # (1)
    paginator: ListEngagementInvitationsPaginator = client.get_paginator("list_engagement_invitations")  # (2)
    async for item in paginator.paginate(...):
        item: ListEngagementInvitationsResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. paginator: [ListEngagementInvitationsPaginator](./paginators.md#listengagementinvitationspaginator)
3. item: [:material-code-braces: ListEngagementInvitationsResponseTypeDef](./type_defs.md#listengagementinvitationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEngagementInvitationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    ParticipantType: ParticipantTypeType,  # (1)
    EngagementIdentifier: Sequence[str] = ...,
    PayloadType: Sequence[EngagementInvitationPayloadTypeType] = ...,  # (2)
    SenderAwsAccountId: Sequence[str] = ...,
    Sort: OpportunityEngagementInvitationSortTypeDef = ...,  # (3)
    Status: Sequence[InvitationStatusType] = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AioPageIterator[ListEngagementInvitationsResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: ParticipantTypeType](./literals.md#participanttypetype) 
2. See [:material-code-brackets: EngagementInvitationPayloadTypeType](./literals.md#engagementinvitationpayloadtypetype) 
3. See [:material-code-braces: OpportunityEngagementInvitationSortTypeDef](./type_defs.md#opportunityengagementinvitationsorttypedef) 
4. See [:material-code-brackets: InvitationStatusType](./literals.md#invitationstatustype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: ListEngagementInvitationsResponseTypeDef](./type_defs.md#listengagementinvitationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEngagementInvitationsRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
    "ParticipantType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEngagementInvitationsRequestPaginateTypeDef](./type_defs.md#listengagementinvitationsrequestpaginatetypedef) 
## ListEngagementMembersPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_paginator("list_engagement_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/paginator/ListEngagementMembers.html#PartnerCentralSellingAPI.Paginator.ListEngagementMembers)

```python
# ListEngagementMembersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_selling.paginator import ListEngagementMembersPaginator

session = get_session()
async with session.create_client("partnercentral-selling") as client:  # (1)
    paginator: ListEngagementMembersPaginator = client.get_paginator("list_engagement_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListEngagementMembersResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. paginator: [ListEngagementMembersPaginator](./paginators.md#listengagementmemberspaginator)
3. item: [:material-code-braces: ListEngagementMembersResponseTypeDef](./type_defs.md#listengagementmembersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEngagementMembersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    Identifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEngagementMembersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEngagementMembersResponseTypeDef](./type_defs.md#listengagementmembersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEngagementMembersRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEngagementMembersRequestPaginateTypeDef](./type_defs.md#listengagementmembersrequestpaginatetypedef) 
## ListEngagementResourceAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_paginator("list_engagement_resource_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/paginator/ListEngagementResourceAssociations.html#PartnerCentralSellingAPI.Paginator.ListEngagementResourceAssociations)

```python
# ListEngagementResourceAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_selling.paginator import ListEngagementResourceAssociationsPaginator

session = get_session()
async with session.create_client("partnercentral-selling") as client:  # (1)
    paginator: ListEngagementResourceAssociationsPaginator = client.get_paginator("list_engagement_resource_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListEngagementResourceAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. paginator: [ListEngagementResourceAssociationsPaginator](./paginators.md#listengagementresourceassociationspaginator)
3. item: [:material-code-braces: ListEngagementResourceAssociationsResponseTypeDef](./type_defs.md#listengagementresourceassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEngagementResourceAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    CreatedBy: str = ...,
    EngagementIdentifier: str = ...,
    ResourceIdentifier: str = ...,
    ResourceType: ResourceTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListEngagementResourceAssociationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEngagementResourceAssociationsResponseTypeDef](./type_defs.md#listengagementresourceassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEngagementResourceAssociationsRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEngagementResourceAssociationsRequestPaginateTypeDef](./type_defs.md#listengagementresourceassociationsrequestpaginatetypedef) 
## ListEngagementsPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_paginator("list_engagements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/paginator/ListEngagements.html#PartnerCentralSellingAPI.Paginator.ListEngagements)

```python
# ListEngagementsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_selling.paginator import ListEngagementsPaginator

session = get_session()
async with session.create_client("partnercentral-selling") as client:  # (1)
    paginator: ListEngagementsPaginator = client.get_paginator("list_engagements")  # (2)
    async for item in paginator.paginate(...):
        item: ListEngagementsResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. paginator: [ListEngagementsPaginator](./paginators.md#listengagementspaginator)
3. item: [:material-code-braces: ListEngagementsResponseTypeDef](./type_defs.md#listengagementsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEngagementsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    CreatedBy: Sequence[str] = ...,
    EngagementIdentifier: Sequence[str] = ...,
    ExcludeCreatedBy: Sequence[str] = ...,
    Sort: EngagementSortTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListEngagementsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EngagementSortTypeDef](./type_defs.md#engagementsorttypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEngagementsResponseTypeDef](./type_defs.md#listengagementsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEngagementsRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEngagementsRequestPaginateTypeDef](./type_defs.md#listengagementsrequestpaginatetypedef) 
## ListOpportunitiesPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_paginator("list_opportunities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/paginator/ListOpportunities.html#PartnerCentralSellingAPI.Paginator.ListOpportunities)

```python
# ListOpportunitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_selling.paginator import ListOpportunitiesPaginator

session = get_session()
async with session.create_client("partnercentral-selling") as client:  # (1)
    paginator: ListOpportunitiesPaginator = client.get_paginator("list_opportunities")  # (2)
    async for item in paginator.paginate(...):
        item: ListOpportunitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. paginator: [ListOpportunitiesPaginator](./paginators.md#listopportunitiespaginator)
3. item: [:material-code-braces: ListOpportunitiesResponseTypeDef](./type_defs.md#listopportunitiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOpportunitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    CustomerCompanyName: Sequence[str] = ...,
    Identifier: Sequence[str] = ...,
    LastModifiedDate: LastModifiedDateTypeDef = ...,  # (1)
    LifeCycleReviewStatus: Sequence[ReviewStatusType] = ...,  # (2)
    LifeCycleStage: Sequence[StageType] = ...,  # (3)
    Sort: OpportunitySortTypeDef = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AioPageIterator[ListOpportunitiesResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-braces: LastModifiedDateTypeDef](./type_defs.md#lastmodifieddatetypedef) 
2. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
3. See [:material-code-brackets: StageType](./literals.md#stagetype) 
4. See [:material-code-braces: OpportunitySortTypeDef](./type_defs.md#opportunitysorttypedef) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: ListOpportunitiesResponseTypeDef](./type_defs.md#listopportunitiesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOpportunitiesRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOpportunitiesRequestPaginateTypeDef](./type_defs.md#listopportunitiesrequestpaginatetypedef) 
## ListResourceSnapshotJobsPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_paginator("list_resource_snapshot_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/paginator/ListResourceSnapshotJobs.html#PartnerCentralSellingAPI.Paginator.ListResourceSnapshotJobs)

```python
# ListResourceSnapshotJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_selling.paginator import ListResourceSnapshotJobsPaginator

session = get_session()
async with session.create_client("partnercentral-selling") as client:  # (1)
    paginator: ListResourceSnapshotJobsPaginator = client.get_paginator("list_resource_snapshot_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceSnapshotJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. paginator: [ListResourceSnapshotJobsPaginator](./paginators.md#listresourcesnapshotjobspaginator)
3. item: [:material-code-braces: ListResourceSnapshotJobsResponseTypeDef](./type_defs.md#listresourcesnapshotjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceSnapshotJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    EngagementIdentifier: str = ...,
    Sort: SortObjectTypeDef = ...,  # (1)
    Status: ResourceSnapshotJobStatusType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListResourceSnapshotJobsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: SortObjectTypeDef](./type_defs.md#sortobjecttypedef) 
2. See [:material-code-brackets: ResourceSnapshotJobStatusType](./literals.md#resourcesnapshotjobstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListResourceSnapshotJobsResponseTypeDef](./type_defs.md#listresourcesnapshotjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceSnapshotJobsRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceSnapshotJobsRequestPaginateTypeDef](./type_defs.md#listresourcesnapshotjobsrequestpaginatetypedef) 
## ListResourceSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_paginator("list_resource_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/paginator/ListResourceSnapshots.html#PartnerCentralSellingAPI.Paginator.ListResourceSnapshots)

```python
# ListResourceSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_selling.paginator import ListResourceSnapshotsPaginator

session = get_session()
async with session.create_client("partnercentral-selling") as client:  # (1)
    paginator: ListResourceSnapshotsPaginator = client.get_paginator("list_resource_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceSnapshotsResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. paginator: [ListResourceSnapshotsPaginator](./paginators.md#listresourcesnapshotspaginator)
3. item: [:material-code-braces: ListResourceSnapshotsResponseTypeDef](./type_defs.md#listresourcesnapshotsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    EngagementIdentifier: str,
    CreatedBy: str = ...,
    ResourceIdentifier: str = ...,
    ResourceSnapshotTemplateIdentifier: str = ...,
    ResourceType: ResourceTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListResourceSnapshotsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListResourceSnapshotsResponseTypeDef](./type_defs.md#listresourcesnapshotsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceSnapshotsRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
    "EngagementIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceSnapshotsRequestPaginateTypeDef](./type_defs.md#listresourcesnapshotsrequestpaginatetypedef) 
## ListSolutionsPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_paginator("list_solutions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/paginator/ListSolutions.html#PartnerCentralSellingAPI.Paginator.ListSolutions)

```python
# ListSolutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_selling.paginator import ListSolutionsPaginator

session = get_session()
async with session.create_client("partnercentral-selling") as client:  # (1)
    paginator: ListSolutionsPaginator = client.get_paginator("list_solutions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSolutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. paginator: [ListSolutionsPaginator](./paginators.md#listsolutionspaginator)
3. item: [:material-code-braces: ListSolutionsResponseTypeDef](./type_defs.md#listsolutionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSolutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    Category: Sequence[str] = ...,
    Identifier: Sequence[str] = ...,
    Sort: SolutionSortTypeDef = ...,  # (1)
    Status: Sequence[SolutionStatusType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListSolutionsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: SolutionSortTypeDef](./type_defs.md#solutionsorttypedef) 
2. See [:material-code-brackets: SolutionStatusType](./literals.md#solutionstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListSolutionsResponseTypeDef](./type_defs.md#listsolutionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSolutionsRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSolutionsRequestPaginateTypeDef](./type_defs.md#listsolutionsrequestpaginatetypedef) 
