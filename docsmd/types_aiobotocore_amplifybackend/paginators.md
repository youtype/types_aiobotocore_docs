# Paginators

> [Index](../README.md) > [AmplifyBackend](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AmplifyBackend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
    type annotations stubs module [types-aiobotocore-amplifybackend](https://pypi.org/project/types-aiobotocore-amplifybackend/).

## ListBackendJobsPaginator

Type annotations and code completion for `#!python session.create_client("amplifybackend").get_paginator("list_backend_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Paginator.ListBackendJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_amplifybackend.paginator import ListBackendJobsPaginator

session = get_session()
async with session.create_client("amplifybackend") as client:
    client: AmplifyBackendClient
    paginator: ListBackendJobsPaginator = client.get_paginator("list_backend_jobs")
```


### paginate

Type annotations and code completion for `#!python ListBackendJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AppId: str,
    BackendEnvironmentName: str,
    JobId: str = ...,
    Operation: str = ...,
    Status: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBackendJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBackendJobsResponseTypeDef](./type_defs.md#listbackendjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListBackendJobsRequestListBackendJobsPaginateTypeDef = {  # (1)
    "AppId": ...,
    "BackendEnvironmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackendJobsRequestListBackendJobsPaginateTypeDef](./type_defs.md#listbackendjobsrequestlistbackendjobspaginatetypedef) 
