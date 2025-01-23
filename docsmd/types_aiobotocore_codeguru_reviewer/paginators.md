# Paginators

> [Index](../README.md) > [CodeGuruReviewer](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeGuruReviewer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#codegurureviewer)
    type annotations stubs module [types-aiobotocore-codeguru-reviewer](https://pypi.org/project/types-aiobotocore-codeguru-reviewer/).

## ListRepositoryAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").get_paginator("list_repository_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer/paginator/ListRepositoryAssociations.html#CodeGuruReviewer.Paginator.ListRepositoryAssociations)

```python
# ListRepositoryAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codeguru_reviewer.paginator import ListRepositoryAssociationsPaginator

session = get_session()
async with session.create_client("codeguru-reviewer") as client:  # (1)
    paginator: ListRepositoryAssociationsPaginator = client.get_paginator("list_repository_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListRepositoryAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeGuruReviewerClient](./client.md)
2. paginator: [ListRepositoryAssociationsPaginator](./paginators.md#listrepositoryassociationspaginator)
3. item: [:material-code-braces: ListRepositoryAssociationsResponseTypeDef](./type_defs.md#listrepositoryassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRepositoryAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProviderTypes: Sequence[ProviderTypeType] = ...,  # (1)
    States: Sequence[RepositoryAssociationStateType] = ...,  # (2)
    Names: Sequence[str] = ...,
    Owners: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListRepositoryAssociationsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-brackets: RepositoryAssociationStateType](./literals.md#repositoryassociationstatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListRepositoryAssociationsResponseTypeDef](./type_defs.md#listrepositoryassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRepositoryAssociationsRequestPaginateTypeDef = {  # (1)
    "ProviderTypes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRepositoryAssociationsRequestPaginateTypeDef](./type_defs.md#listrepositoryassociationsrequestpaginatetypedef) 
