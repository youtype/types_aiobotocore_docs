# Paginators

> [Index](../README.md) > [CloudControlApi](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudControlApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
    type annotations stubs module [types-aiobotocore-cloudcontrol](https://pypi.org/project/types-aiobotocore-cloudcontrol/).

## ListResourceRequestsPaginator

Type annotations and code completion for `#!python session.create_client("cloudcontrol").get_paginator("list_resource_requests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResourceRequests)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudcontrol.paginator import ListResourceRequestsPaginator

session = get_session()
async with session.create_client("cloudcontrol") as client:  # (1)
    paginator: ListResourceRequestsPaginator = client.get_paginator("list_resource_requests")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceRequestsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudControlApiClient](./client.md)
2. paginator: [ListResourceRequestsPaginator](./paginators.md#listresourcerequestspaginator)
3. item: [:material-code-braces: ListResourceRequestsOutputTypeDef](./type_defs.md#listresourcerequestsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceRequestsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListResourceRequestsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ResourceRequestStatusFilterTypeDef](./type_defs.md#resourcerequeststatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListResourceRequestsOutputTypeDef](./type_defs.md#listresourcerequestsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListResourceRequestsInputListResourceRequestsPaginateTypeDef = {  # (1)
    "ResourceRequestStatusFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceRequestsInputListResourceRequestsPaginateTypeDef](./type_defs.md#listresourcerequestsinputlistresourcerequestspaginatetypedef) 
## ListResourcesPaginator

Type annotations and code completion for `#!python session.create_client("cloudcontrol").get_paginator("list_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResources)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudcontrol.paginator import ListResourcesPaginator

session = get_session()
async with session.create_client("cloudcontrol") as client:  # (1)
    paginator: ListResourcesPaginator = client.get_paginator("list_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudControlApiClient](./client.md)
2. paginator: [ListResourcesPaginator](./paginators.md#listresourcespaginator)
3. item: [:material-code-braces: ListResourcesOutputTypeDef](./type_defs.md#listresourcesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListResourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TypeName: str,
    TypeVersionId: str = ...,
    RoleArn: str = ...,
    ResourceModel: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResourcesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourcesOutputTypeDef](./type_defs.md#listresourcesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListResourcesInputListResourcesPaginateTypeDef = {  # (1)
    "TypeName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourcesInputListResourcesPaginateTypeDef](./type_defs.md#listresourcesinputlistresourcespaginatetypedef) 
