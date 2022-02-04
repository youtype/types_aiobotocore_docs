<a id="waiters-for-aiobotocore-codegurureviewer-module"></a>

# Waiters for aiobotocore CodeGuruReviewer module

> [Index](..) > [CodeGuruReviewer](.) > Waiters

Auto-generated documentation for
[CodeGuruReviewer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
type annotations stubs module
[types-aiobotocore-codeguru-reviewer](https://pypi.org/project/types-aiobotocore-codeguru-reviewer/).

- [Waiters for aiobotocore CodeGuruReviewer module](#waiters-for-aiobotocore-codegurureviewer-module)
  - [CodeReviewCompletedWaiter](#codereviewcompletedwaiter)
  - [RepositoryAssociationSucceededWaiter](#repositoryassociationsucceededwaiter)

<a id="codereviewcompletedwaiter"></a>

## CodeReviewCompletedWaiter

Type annotations for
`aiobotocore.create_client("codeguru-reviewer").get_waiter("code_review_completed")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_codeguru_reviewer.waiter import CodeReviewCompletedWaiter

def get_code_review_completed_waiter() -> CodeReviewCompletedWaiter:
    return Session().create_client("codeguru-reviewer").get_waiter("code_review_completed")
```

Boto3 documentation:
[CodeGuruReviewer.Waiter.code_review_completed](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Waiter.CodeReviewCompleted)

Arguments for `CodeReviewCompletedWaiter.wait` method:

- `CodeReviewArn`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="repositoryassociationsucceededwaiter"></a>

## RepositoryAssociationSucceededWaiter

Type annotations for
`aiobotocore.create_client("codeguru-reviewer").get_waiter("repository_association_succeeded")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_codeguru_reviewer.waiter import RepositoryAssociationSucceededWaiter

def get_repository_association_succeeded_waiter() -> RepositoryAssociationSucceededWaiter:
    return Session().create_client("codeguru-reviewer").get_waiter("repository_association_succeeded")
```

Boto3 documentation:
[CodeGuruReviewer.Waiter.repository_association_succeeded](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Waiter.RepositoryAssociationSucceeded)

Arguments for `RepositoryAssociationSucceededWaiter.wait` method:

- `AssociationArn`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
