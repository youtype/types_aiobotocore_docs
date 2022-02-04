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
`aiobotocore.create_client("amplifybackend").get_paginator("list_backend_jobs")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_amplifybackend.paginator import ListBackendJobsPaginator

def get_list_backend_jobs_paginator() -> ListBackendJobsPaginator:
    return Session().create_client("amplifybackend").get_paginator("list_backend_jobs")
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
`_PageIterator`\[[ListBackendJobsResponseTypeDef](./type_defs.md#listbackendjobsresponsetypedef)\].
