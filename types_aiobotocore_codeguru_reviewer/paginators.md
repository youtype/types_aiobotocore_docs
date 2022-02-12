<a id="paginators-for-aiobotocore-codegurureviewer-module"></a>

# Paginators for aiobotocore CodeGuruReviewer module

> [Index](..) > [CodeGuruReviewer](.) > Paginators

Auto-generated documentation for
[CodeGuruReviewer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
type annotations stubs module
[types-aiobotocore-codeguru-reviewer](https://pypi.org/project/types-aiobotocore-codeguru-reviewer/).

- [Paginators for aiobotocore CodeGuruReviewer module](#paginators-for-aiobotocore-codegurureviewer-module)
  - [ListRepositoryAssociationsPaginator](#listrepositoryassociationspaginator)

<a id="listrepositoryassociationspaginator"></a>

## ListRepositoryAssociationsPaginator

Type annotations for
`session.create_client("codeguru-reviewer").get_paginator("list_repository_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codeguru_reviewer.paginator import ListRepositoryAssociationsPaginator

session = get_session()
async with session.create_client("codeguru-reviewer") as client:
    client: CodeGuruReviewerClient
    paginator: ListRepositoryAssociationsPaginator = client.get_paginator("list_repository_associations")
```

Boto3 documentation:
[CodeGuruReviewer.Paginator.ListRepositoryAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Paginator.ListRepositoryAssociations)

Arguments for `ListRepositoryAssociationsPaginator.paginate` method:

- `ProviderTypes`:
  `Sequence`\[[ProviderTypeType](./literals.md#providertypetype)\]
- `States`:
  `Sequence`\[[RepositoryAssociationStateType](./literals.md#repositoryassociationstatetype)\]
- `Names`: `Sequence`\[`str`\]
- `Owners`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRepositoryAssociationsPaginator.paginate` returns
`AsyncIterable`\[[ListRepositoryAssociationsResponseTypeDef](./type_defs.md#listrepositoryassociationsresponsetypedef)\].
