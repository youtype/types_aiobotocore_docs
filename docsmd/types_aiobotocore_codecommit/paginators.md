# Paginators

> [Index](../README.md) > [CodeCommit](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeCommit](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
    type annotations stubs module [types-aiobotocore-codecommit](https://pypi.org/project/types-aiobotocore-codecommit/).

## DescribePullRequestEventsPaginator

Type annotations and code completion for `#!python session.create_client("codecommit").get_paginator("describe_pull_request_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codecommit.paginator import DescribePullRequestEventsPaginator

session = get_session()
async with session.create_client("codecommit") as client:  # (1)
    paginator: DescribePullRequestEventsPaginator = client.get_paginator("describe_pull_request_events")  # (2)
    async for item in paginator.paginate(...):
        item: DescribePullRequestEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeCommitClient](./client.md)
2. paginator: [DescribePullRequestEventsPaginator](./paginators.md#describepullrequesteventspaginator)
3. item: [:material-code-braces: DescribePullRequestEventsOutputTypeDef](./type_defs.md#describepullrequesteventsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribePullRequestEventsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    pullRequestId: str,
    pullRequestEventType: PullRequestEventTypeType = ...,  # (1)
    actorArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribePullRequestEventsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PullRequestEventTypeType](./literals.md#pullrequesteventtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribePullRequestEventsOutputTypeDef](./type_defs.md#describepullrequesteventsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = {  # (1)
    "pullRequestId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef](./type_defs.md#describepullrequesteventsinputdescribepullrequesteventspaginatetypedef) 
## GetCommentsForComparedCommitPaginator

Type annotations and code completion for `#!python session.create_client("codecommit").get_paginator("get_comments_for_compared_commit")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codecommit.paginator import GetCommentsForComparedCommitPaginator

session = get_session()
async with session.create_client("codecommit") as client:  # (1)
    paginator: GetCommentsForComparedCommitPaginator = client.get_paginator("get_comments_for_compared_commit")  # (2)
    async for item in paginator.paginate(...):
        item: GetCommentsForComparedCommitOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeCommitClient](./client.md)
2. paginator: [GetCommentsForComparedCommitPaginator](./paginators.md#getcommentsforcomparedcommitpaginator)
3. item: [:material-code-braces: GetCommentsForComparedCommitOutputTypeDef](./type_defs.md#getcommentsforcomparedcommitoutputtypedef) 


### paginate

Type annotations and code completion for `#!python GetCommentsForComparedCommitPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    repositoryName: str,
    afterCommitId: str,
    beforeCommitId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetCommentsForComparedCommitOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetCommentsForComparedCommitOutputTypeDef](./type_defs.md#getcommentsforcomparedcommitoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = {  # (1)
    "repositoryName": ...,
    "afterCommitId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef](./type_defs.md#getcommentsforcomparedcommitinputgetcommentsforcomparedcommitpaginatetypedef) 
## GetCommentsForPullRequestPaginator

Type annotations and code completion for `#!python session.create_client("codecommit").get_paginator("get_comments_for_pull_request")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codecommit.paginator import GetCommentsForPullRequestPaginator

session = get_session()
async with session.create_client("codecommit") as client:  # (1)
    paginator: GetCommentsForPullRequestPaginator = client.get_paginator("get_comments_for_pull_request")  # (2)
    async for item in paginator.paginate(...):
        item: GetCommentsForPullRequestOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeCommitClient](./client.md)
2. paginator: [GetCommentsForPullRequestPaginator](./paginators.md#getcommentsforpullrequestpaginator)
3. item: [:material-code-braces: GetCommentsForPullRequestOutputTypeDef](./type_defs.md#getcommentsforpullrequestoutputtypedef) 


### paginate

Type annotations and code completion for `#!python GetCommentsForPullRequestPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    pullRequestId: str,
    repositoryName: str = ...,
    beforeCommitId: str = ...,
    afterCommitId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetCommentsForPullRequestOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetCommentsForPullRequestOutputTypeDef](./type_defs.md#getcommentsforpullrequestoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = {  # (1)
    "pullRequestId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef](./type_defs.md#getcommentsforpullrequestinputgetcommentsforpullrequestpaginatetypedef) 
## GetDifferencesPaginator

Type annotations and code completion for `#!python session.create_client("codecommit").get_paginator("get_differences")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codecommit.paginator import GetDifferencesPaginator

session = get_session()
async with session.create_client("codecommit") as client:  # (1)
    paginator: GetDifferencesPaginator = client.get_paginator("get_differences")  # (2)
    async for item in paginator.paginate(...):
        item: GetDifferencesOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeCommitClient](./client.md)
2. paginator: [GetDifferencesPaginator](./paginators.md#getdifferencespaginator)
3. item: [:material-code-braces: GetDifferencesOutputTypeDef](./type_defs.md#getdifferencesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python GetDifferencesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    repositoryName: str,
    afterCommitSpecifier: str,
    beforeCommitSpecifier: str = ...,
    beforePath: str = ...,
    afterPath: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetDifferencesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetDifferencesOutputTypeDef](./type_defs.md#getdifferencesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: GetDifferencesInputGetDifferencesPaginateTypeDef = {  # (1)
    "repositoryName": ...,
    "afterCommitSpecifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDifferencesInputGetDifferencesPaginateTypeDef](./type_defs.md#getdifferencesinputgetdifferencespaginatetypedef) 
## ListBranchesPaginator

Type annotations and code completion for `#!python session.create_client("codecommit").get_paginator("list_branches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codecommit.paginator import ListBranchesPaginator

session = get_session()
async with session.create_client("codecommit") as client:  # (1)
    paginator: ListBranchesPaginator = client.get_paginator("list_branches")  # (2)
    async for item in paginator.paginate(...):
        item: ListBranchesOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeCommitClient](./client.md)
2. paginator: [ListBranchesPaginator](./paginators.md#listbranchespaginator)
3. item: [:material-code-braces: ListBranchesOutputTypeDef](./type_defs.md#listbranchesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBranchesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    repositoryName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBranchesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBranchesOutputTypeDef](./type_defs.md#listbranchesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListBranchesInputListBranchesPaginateTypeDef = {  # (1)
    "repositoryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBranchesInputListBranchesPaginateTypeDef](./type_defs.md#listbranchesinputlistbranchespaginatetypedef) 
## ListPullRequestsPaginator

Type annotations and code completion for `#!python session.create_client("codecommit").get_paginator("list_pull_requests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codecommit.paginator import ListPullRequestsPaginator

session = get_session()
async with session.create_client("codecommit") as client:  # (1)
    paginator: ListPullRequestsPaginator = client.get_paginator("list_pull_requests")  # (2)
    async for item in paginator.paginate(...):
        item: ListPullRequestsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeCommitClient](./client.md)
2. paginator: [ListPullRequestsPaginator](./paginators.md#listpullrequestspaginator)
3. item: [:material-code-braces: ListPullRequestsOutputTypeDef](./type_defs.md#listpullrequestsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListPullRequestsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    repositoryName: str,
    authorArn: str = ...,
    pullRequestStatus: PullRequestStatusEnumType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPullRequestsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PullRequestStatusEnumType](./literals.md#pullrequeststatusenumtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPullRequestsOutputTypeDef](./type_defs.md#listpullrequestsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListPullRequestsInputListPullRequestsPaginateTypeDef = {  # (1)
    "repositoryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPullRequestsInputListPullRequestsPaginateTypeDef](./type_defs.md#listpullrequestsinputlistpullrequestspaginatetypedef) 
## ListRepositoriesPaginator

Type annotations and code completion for `#!python session.create_client("codecommit").get_paginator("list_repositories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codecommit.paginator import ListRepositoriesPaginator

session = get_session()
async with session.create_client("codecommit") as client:  # (1)
    paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")  # (2)
    async for item in paginator.paginate(...):
        item: ListRepositoriesOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeCommitClient](./client.md)
2. paginator: [ListRepositoriesPaginator](./paginators.md#listrepositoriespaginator)
3. item: [:material-code-braces: ListRepositoriesOutputTypeDef](./type_defs.md#listrepositoriesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListRepositoriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    sortBy: SortByEnumType = ...,  # (1)
    order: OrderEnumType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListRepositoriesOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortByEnumType](./literals.md#sortbyenumtype) 
2. See [:material-code-brackets: OrderEnumType](./literals.md#orderenumtype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListRepositoriesOutputTypeDef](./type_defs.md#listrepositoriesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListRepositoriesInputListRepositoriesPaginateTypeDef = {  # (1)
    "sortBy": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRepositoriesInputListRepositoriesPaginateTypeDef](./type_defs.md#listrepositoriesinputlistrepositoriespaginatetypedef) 
