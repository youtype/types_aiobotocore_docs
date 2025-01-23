# Paginators

> [Index](../README.md) > [AmplifyBackend](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AmplifyBackend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#amplifybackend)
    type annotations stubs module [types-aiobotocore-amplifybackend](https://pypi.org/project/types-aiobotocore-amplifybackend/).

## ListBackendJobsPaginator

Type annotations and code completion for `#!python session.create_client("amplifybackend").get_paginator("list_backend_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend/paginator/ListBackendJobs.html#AmplifyBackend.Paginator.ListBackendJobs)

```python
# ListBackendJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_amplifybackend.paginator import ListBackendJobsPaginator

session = get_session()
async with session.create_client("amplifybackend") as client:  # (1)
    paginator: ListBackendJobsPaginator = client.get_paginator("list_backend_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListBackendJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [AmplifyBackendClient](./client.md)
2. paginator: [ListBackendJobsPaginator](./paginators.md#listbackendjobspaginator)
3. item: [:material-code-braces: ListBackendJobsResponseTypeDef](./type_defs.md#listbackendjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBackendJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AppId: str,
    BackendEnvironmentName: str,
    JobId: str = ...,
    Operation: str = ...,
    Status: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListBackendJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBackendJobsResponseTypeDef](./type_defs.md#listbackendjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBackendJobsRequestPaginateTypeDef = {  # (1)
    "AppId": ...,
    "BackendEnvironmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackendJobsRequestPaginateTypeDef](./type_defs.md#listbackendjobsrequestpaginatetypedef) 
