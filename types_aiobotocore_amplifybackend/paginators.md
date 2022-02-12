<a id="paginators-for-aiobotocore-amplifybackend-module"></a>

# Paginators for aiobotocore AmplifyBackend module

> [Index](..) > [AmplifyBackend](.) > Paginators

Auto-generated documentation for
[AmplifyBackend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
type annotations stubs module
[types-aiobotocore-amplifybackend](https://pypi.org/project/types-aiobotocore-amplifybackend/).

- [Paginators for aiobotocore AmplifyBackend module](#paginators-for-aiobotocore-amplifybackend-module)
  - [ListBackendJobsPaginator](#listbackendjobspaginator)

<a id="listbackendjobspaginator"></a>

## ListBackendJobsPaginator

Type annotations for
`session.create_client("amplifybackend").get_paginator("list_backend_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_amplifybackend.paginator import ListBackendJobsPaginator

session = get_session()
async with session.create_client("amplifybackend") as client:
    client: AmplifyBackendClient
    paginator: ListBackendJobsPaginator = client.get_paginator("list_backend_jobs")
```

Boto3 documentation:
[AmplifyBackend.Paginator.ListBackendJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Paginator.ListBackendJobs)

Arguments for `ListBackendJobsPaginator.paginate` method:

- `AppId`: `str` *(required)*
- `BackendEnvironmentName`: `str` *(required)*
- `JobId`: `str`
- `Operation`: `str`
- `Status`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBackendJobsPaginator.paginate` returns
`AsyncIterable`\[[ListBackendJobsResponseTypeDef](./type_defs.md#listbackendjobsresponsetypedef)\].
