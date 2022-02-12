<a id="paginators-for-aiobotocore-iotfleethub-module"></a>

# Paginators for aiobotocore IoTFleetHub module

> [Index](..) > [IoTFleetHub](.) > Paginators

Auto-generated documentation for
[IoTFleetHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
type annotations stubs module
[types-aiobotocore-iotfleethub](https://pypi.org/project/types-aiobotocore-iotfleethub/).

- [Paginators for aiobotocore IoTFleetHub module](#paginators-for-aiobotocore-iotfleethub-module)
  - [ListApplicationsPaginator](#listapplicationspaginator)

<a id="listapplicationspaginator"></a>

## ListApplicationsPaginator

Type annotations for
`session.create_client("iotfleethub").get_paginator("list_applications")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotfleethub.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("iotfleethub") as client:
    client: IoTFleetHubClient
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
```

Boto3 documentation:
[IoTFleetHub.Paginator.ListApplications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Paginator.ListApplications)

Arguments for `ListApplicationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListApplicationsPaginator.paginate` returns
`AsyncIterable`\[[ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)\].
