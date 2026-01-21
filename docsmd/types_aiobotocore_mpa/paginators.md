# Paginators

> [Index](../README.md) > [MultipartyApproval](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MultipartyApproval](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mpa.html#multipartyapproval)
    type annotations stubs module [types-aiobotocore-mpa](https://pypi.org/project/types-aiobotocore-mpa/).

## ListApprovalTeamsPaginator

Type annotations and code completion for `#!python session.create_client("mpa").get_paginator("list_approval_teams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mpa/paginator/ListApprovalTeams.html#MultipartyApproval.Paginator.ListApprovalTeams)

```python
# ListApprovalTeamsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mpa.paginator import ListApprovalTeamsPaginator

session = get_session()
async with session.create_client("mpa") as client:  # (1)
    paginator: ListApprovalTeamsPaginator = client.get_paginator("list_approval_teams")  # (2)
    async for item in paginator.paginate(...):
        item: ListApprovalTeamsResponseTypeDef
        print(item)  # (3)
```

1. client: [MultipartyApprovalClient](./client.md)
2. paginator: [ListApprovalTeamsPaginator](./paginators.md#listapprovalteamspaginator)
3. item: `AioPageIterator[ListApprovalTeamsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListApprovalTeamsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListApprovalTeamsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListApprovalTeamsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListApprovalTeamsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApprovalTeamsRequestPaginateTypeDef](./type_defs.md#listapprovalteamsrequestpaginatetypedef)
## ListIdentitySourcesPaginator

Type annotations and code completion for `#!python session.create_client("mpa").get_paginator("list_identity_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mpa/paginator/ListIdentitySources.html#MultipartyApproval.Paginator.ListIdentitySources)

```python
# ListIdentitySourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mpa.paginator import ListIdentitySourcesPaginator

session = get_session()
async with session.create_client("mpa") as client:  # (1)
    paginator: ListIdentitySourcesPaginator = client.get_paginator("list_identity_sources")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdentitySourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [MultipartyApprovalClient](./client.md)
2. paginator: [ListIdentitySourcesPaginator](./paginators.md#listidentitysourcespaginator)
3. item: `AioPageIterator[ListIdentitySourcesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIdentitySourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListIdentitySourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListIdentitySourcesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIdentitySourcesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdentitySourcesRequestPaginateTypeDef](./type_defs.md#listidentitysourcesrequestpaginatetypedef)
## ListPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("mpa").get_paginator("list_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mpa/paginator/ListPolicies.html#MultipartyApproval.Paginator.ListPolicies)

```python
# ListPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mpa.paginator import ListPoliciesPaginator

session = get_session()
async with session.create_client("mpa") as client:  # (1)
    paginator: ListPoliciesPaginator = client.get_paginator("list_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [MultipartyApprovalClient](./client.md)
2. paginator: [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
3. item: `AioPageIterator[ListPoliciesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPoliciesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPoliciesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoliciesRequestPaginateTypeDef](./type_defs.md#listpoliciesrequestpaginatetypedef)
## ListPolicyVersionsPaginator

Type annotations and code completion for `#!python session.create_client("mpa").get_paginator("list_policy_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mpa/paginator/ListPolicyVersions.html#MultipartyApproval.Paginator.ListPolicyVersions)

```python
# ListPolicyVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mpa.paginator import ListPolicyVersionsPaginator

session = get_session()
async with session.create_client("mpa") as client:  # (1)
    paginator: ListPolicyVersionsPaginator = client.get_paginator("list_policy_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPolicyVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [MultipartyApprovalClient](./client.md)
2. paginator: [ListPolicyVersionsPaginator](./paginators.md#listpolicyversionspaginator)
3. item: `AioPageIterator[ListPolicyVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPolicyVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PolicyArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPolicyVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPolicyVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPolicyVersionsRequestPaginateTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPolicyVersionsRequestPaginateTypeDef](./type_defs.md#listpolicyversionsrequestpaginatetypedef)
## ListResourcePoliciesPaginator

Type annotations and code completion for `#!python session.create_client("mpa").get_paginator("list_resource_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mpa/paginator/ListResourcePolicies.html#MultipartyApproval.Paginator.ListResourcePolicies)

```python
# ListResourcePoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mpa.paginator import ListResourcePoliciesPaginator

session = get_session()
async with session.create_client("mpa") as client:  # (1)
    paginator: ListResourcePoliciesPaginator = client.get_paginator("list_resource_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourcePoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [MultipartyApprovalClient](./client.md)
2. paginator: [ListResourcePoliciesPaginator](./paginators.md#listresourcepoliciespaginator)
3. item: `AioPageIterator[ListResourcePoliciesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListResourcePoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListResourcePoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListResourcePoliciesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListResourcePoliciesRequestPaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourcePoliciesRequestPaginateTypeDef](./type_defs.md#listresourcepoliciesrequestpaginatetypedef)
## ListSessionsPaginator

Type annotations and code completion for `#!python session.create_client("mpa").get_paginator("list_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mpa/paginator/ListSessions.html#MultipartyApproval.Paginator.ListSessions)

```python
# ListSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mpa.paginator import ListSessionsPaginator

session = get_session()
async with session.create_client("mpa") as client:  # (1)
    paginator: ListSessionsPaginator = client.get_paginator("list_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSessionsResponseTypeDef
        print(item)  # (3)
```

1. client: [MultipartyApprovalClient](./client.md)
2. paginator: [ListSessionsPaginator](./paginators.md#listsessionspaginator)
3. item: `AioPageIterator[ListSessionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApprovalTeamArn: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListSessionsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListSessionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSessionsRequestPaginateTypeDef = {  # (1)
    "ApprovalTeamArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSessionsRequestPaginateTypeDef](./type_defs.md#listsessionsrequestpaginatetypedef)
