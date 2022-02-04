<a id="paginators-for-aiobotocore-codecommit-module"></a>

# Paginators for aiobotocore CodeCommit module

> [Index](..) > [CodeCommit](.) > Paginators

Auto-generated documentation for
[CodeCommit](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
type annotations stubs module
[types-aiobotocore-codecommit](https://pypi.org/project/types-aiobotocore-codecommit/).

- [Paginators for aiobotocore CodeCommit module](#paginators-for-aiobotocore-codecommit-module)
  - [DescribePullRequestEventsPaginator](#describepullrequesteventspaginator)
  - [GetCommentsForComparedCommitPaginator](#getcommentsforcomparedcommitpaginator)
  - [GetCommentsForPullRequestPaginator](#getcommentsforpullrequestpaginator)
  - [GetDifferencesPaginator](#getdifferencespaginator)
  - [ListBranchesPaginator](#listbranchespaginator)
  - [ListPullRequestsPaginator](#listpullrequestspaginator)
  - [ListRepositoriesPaginator](#listrepositoriespaginator)

<a id="describepullrequesteventspaginator"></a>

## DescribePullRequestEventsPaginator

Type annotations for
`aiobotocore.create_client("codecommit").get_paginator("describe_pull_request_events")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_codecommit.paginator import DescribePullRequestEventsPaginator

def get_describe_pull_request_events_paginator() -> DescribePullRequestEventsPaginator:
    return Session().create_client("codecommit").get_paginator("describe_pull_request_events")
```

Boto3 documentation:
[CodeCommit.Paginator.DescribePullRequestEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents)

Arguments for `DescribePullRequestEventsPaginator.paginate` method:

- `pullRequestId`: `str` *(required)*
- `pullRequestEventType`:
  [PullRequestEventTypeType](./literals.md#pullrequesteventtypetype)
- `actorArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribePullRequestEventsPaginator.paginate` returns
`_PageIterator`\[[DescribePullRequestEventsOutputTypeDef](./type_defs.md#describepullrequesteventsoutputtypedef)\].

<a id="getcommentsforcomparedcommitpaginator"></a>

## GetCommentsForComparedCommitPaginator

Type annotations for
`aiobotocore.create_client("codecommit").get_paginator("get_comments_for_compared_commit")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_codecommit.paginator import GetCommentsForComparedCommitPaginator

def get_get_comments_for_compared_commit_paginator() -> GetCommentsForComparedCommitPaginator:
    return Session().create_client("codecommit").get_paginator("get_comments_for_compared_commit")
```

Boto3 documentation:
[CodeCommit.Paginator.GetCommentsForComparedCommit](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit)

Arguments for `GetCommentsForComparedCommitPaginator.paginate` method:

- `repositoryName`: `str` *(required)*
- `afterCommitId`: `str` *(required)*
- `beforeCommitId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetCommentsForComparedCommitPaginator.paginate` returns
`_PageIterator`\[[GetCommentsForComparedCommitOutputTypeDef](./type_defs.md#getcommentsforcomparedcommitoutputtypedef)\].

<a id="getcommentsforpullrequestpaginator"></a>

## GetCommentsForPullRequestPaginator

Type annotations for
`aiobotocore.create_client("codecommit").get_paginator("get_comments_for_pull_request")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_codecommit.paginator import GetCommentsForPullRequestPaginator

def get_get_comments_for_pull_request_paginator() -> GetCommentsForPullRequestPaginator:
    return Session().create_client("codecommit").get_paginator("get_comments_for_pull_request")
```

Boto3 documentation:
[CodeCommit.Paginator.GetCommentsForPullRequest](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest)

Arguments for `GetCommentsForPullRequestPaginator.paginate` method:

- `pullRequestId`: `str` *(required)*
- `repositoryName`: `str`
- `beforeCommitId`: `str`
- `afterCommitId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetCommentsForPullRequestPaginator.paginate` returns
`_PageIterator`\[[GetCommentsForPullRequestOutputTypeDef](./type_defs.md#getcommentsforpullrequestoutputtypedef)\].

<a id="getdifferencespaginator"></a>

## GetDifferencesPaginator

Type annotations for
`aiobotocore.create_client("codecommit").get_paginator("get_differences")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_codecommit.paginator import GetDifferencesPaginator

def get_get_differences_paginator() -> GetDifferencesPaginator:
    return Session().create_client("codecommit").get_paginator("get_differences")
```

Boto3 documentation:
[CodeCommit.Paginator.GetDifferences](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences)

Arguments for `GetDifferencesPaginator.paginate` method:

- `repositoryName`: `str` *(required)*
- `afterCommitSpecifier`: `str` *(required)*
- `beforeCommitSpecifier`: `str`
- `beforePath`: `str`
- `afterPath`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDifferencesPaginator.paginate` returns
`_PageIterator`\[[GetDifferencesOutputTypeDef](./type_defs.md#getdifferencesoutputtypedef)\].

<a id="listbranchespaginator"></a>

## ListBranchesPaginator

Type annotations for
`aiobotocore.create_client("codecommit").get_paginator("list_branches")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_codecommit.paginator import ListBranchesPaginator

def get_list_branches_paginator() -> ListBranchesPaginator:
    return Session().create_client("codecommit").get_paginator("list_branches")
```

Boto3 documentation:
[CodeCommit.Paginator.ListBranches](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches)

Arguments for `ListBranchesPaginator.paginate` method:

- `repositoryName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBranchesPaginator.paginate` returns
`_PageIterator`\[[ListBranchesOutputTypeDef](./type_defs.md#listbranchesoutputtypedef)\].

<a id="listpullrequestspaginator"></a>

## ListPullRequestsPaginator

Type annotations for
`aiobotocore.create_client("codecommit").get_paginator("list_pull_requests")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_codecommit.paginator import ListPullRequestsPaginator

def get_list_pull_requests_paginator() -> ListPullRequestsPaginator:
    return Session().create_client("codecommit").get_paginator("list_pull_requests")
```

Boto3 documentation:
[CodeCommit.Paginator.ListPullRequests](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests)

Arguments for `ListPullRequestsPaginator.paginate` method:

- `repositoryName`: `str` *(required)*
- `authorArn`: `str`
- `pullRequestStatus`:
  [PullRequestStatusEnumType](./literals.md#pullrequeststatusenumtype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPullRequestsPaginator.paginate` returns
`_PageIterator`\[[ListPullRequestsOutputTypeDef](./type_defs.md#listpullrequestsoutputtypedef)\].

<a id="listrepositoriespaginator"></a>

## ListRepositoriesPaginator

Type annotations for
`aiobotocore.create_client("codecommit").get_paginator("list_repositories")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_codecommit.paginator import ListRepositoriesPaginator

def get_list_repositories_paginator() -> ListRepositoriesPaginator:
    return Session().create_client("codecommit").get_paginator("list_repositories")
```

Boto3 documentation:
[CodeCommit.Paginator.ListRepositories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories)

Arguments for `ListRepositoriesPaginator.paginate` method:

- `sortBy`: [SortByEnumType](./literals.md#sortbyenumtype)
- `order`: [OrderEnumType](./literals.md#orderenumtype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRepositoriesPaginator.paginate` returns
`_PageIterator`\[[ListRepositoriesOutputTypeDef](./type_defs.md#listrepositoriesoutputtypedef)\].
