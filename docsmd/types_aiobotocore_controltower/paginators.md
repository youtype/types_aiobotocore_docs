# Paginators

> [Index](../README.md) > [ControlTower](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#controltower)
    type annotations stubs module [types-aiobotocore-controltower](https://pypi.org/project/types-aiobotocore-controltower/).

## ListBaselinesPaginator

Type annotations and code completion for `#!python session.create_client("controltower").get_paginator("list_baselines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower/paginator/ListBaselines.html#ControlTower.Paginator.ListBaselines)

```python
# ListBaselinesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_controltower.paginator import ListBaselinesPaginator

session = get_session()
async with session.create_client("controltower") as client:  # (1)
    paginator: ListBaselinesPaginator = client.get_paginator("list_baselines")  # (2)
    async for item in paginator.paginate(...):
        item: ListBaselinesOutputTypeDef
        print(item)  # (3)
```

1. client: [ControlTowerClient](./client.md)
2. paginator: [ListBaselinesPaginator](./paginators.md#listbaselinespaginator)
3. item: `AioPageIterator[ListBaselinesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBaselinesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBaselinesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBaselinesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBaselinesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBaselinesInputPaginateTypeDef](./type_defs.md#listbaselinesinputpaginatetypedef)
## ListControlOperationsPaginator

Type annotations and code completion for `#!python session.create_client("controltower").get_paginator("list_control_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower/paginator/ListControlOperations.html#ControlTower.Paginator.ListControlOperations)

```python
# ListControlOperationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_controltower.paginator import ListControlOperationsPaginator

session = get_session()
async with session.create_client("controltower") as client:  # (1)
    paginator: ListControlOperationsPaginator = client.get_paginator("list_control_operations")  # (2)
    async for item in paginator.paginate(...):
        item: ListControlOperationsOutputTypeDef
        print(item)  # (3)
```

1. client: [ControlTowerClient](./client.md)
2. paginator: [ListControlOperationsPaginator](./paginators.md#listcontroloperationspaginator)
3. item: `AioPageIterator[ListControlOperationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListControlOperationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filter: ControlOperationFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListControlOperationsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ControlOperationFilterTypeDef](./type_defs.md#controloperationfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListControlOperationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListControlOperationsInputPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListControlOperationsInputPaginateTypeDef](./type_defs.md#listcontroloperationsinputpaginatetypedef)
## ListEnabledBaselinesPaginator

Type annotations and code completion for `#!python session.create_client("controltower").get_paginator("list_enabled_baselines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower/paginator/ListEnabledBaselines.html#ControlTower.Paginator.ListEnabledBaselines)

```python
# ListEnabledBaselinesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_controltower.paginator import ListEnabledBaselinesPaginator

session = get_session()
async with session.create_client("controltower") as client:  # (1)
    paginator: ListEnabledBaselinesPaginator = client.get_paginator("list_enabled_baselines")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnabledBaselinesOutputTypeDef
        print(item)  # (3)
```

1. client: [ControlTowerClient](./client.md)
2. paginator: [ListEnabledBaselinesPaginator](./paginators.md#listenabledbaselinespaginator)
3. item: `AioPageIterator[ListEnabledBaselinesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEnabledBaselinesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filter: EnabledBaselineFilterTypeDef = ...,  # (1)
    includeChildren: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListEnabledBaselinesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EnabledBaselineFilterTypeDef](./type_defs.md#enabledbaselinefiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListEnabledBaselinesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEnabledBaselinesInputPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnabledBaselinesInputPaginateTypeDef](./type_defs.md#listenabledbaselinesinputpaginatetypedef)
## ListEnabledControlsPaginator

Type annotations and code completion for `#!python session.create_client("controltower").get_paginator("list_enabled_controls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower/paginator/ListEnabledControls.html#ControlTower.Paginator.ListEnabledControls)

```python
# ListEnabledControlsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_controltower.paginator import ListEnabledControlsPaginator

session = get_session()
async with session.create_client("controltower") as client:  # (1)
    paginator: ListEnabledControlsPaginator = client.get_paginator("list_enabled_controls")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnabledControlsOutputTypeDef
        print(item)  # (3)
```

1. client: [ControlTowerClient](./client.md)
2. paginator: [ListEnabledControlsPaginator](./paginators.md#listenabledcontrolspaginator)
3. item: `AioPageIterator[ListEnabledControlsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEnabledControlsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    targetIdentifier: str = ...,
    filter: EnabledControlFilterTypeDef = ...,  # (1)
    includeChildren: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListEnabledControlsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EnabledControlFilterTypeDef](./type_defs.md#enabledcontrolfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListEnabledControlsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEnabledControlsInputPaginateTypeDef = {  # (1)
    "targetIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnabledControlsInputPaginateTypeDef](./type_defs.md#listenabledcontrolsinputpaginatetypedef)
## ListLandingZoneOperationsPaginator

Type annotations and code completion for `#!python session.create_client("controltower").get_paginator("list_landing_zone_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower/paginator/ListLandingZoneOperations.html#ControlTower.Paginator.ListLandingZoneOperations)

```python
# ListLandingZoneOperationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_controltower.paginator import ListLandingZoneOperationsPaginator

session = get_session()
async with session.create_client("controltower") as client:  # (1)
    paginator: ListLandingZoneOperationsPaginator = client.get_paginator("list_landing_zone_operations")  # (2)
    async for item in paginator.paginate(...):
        item: ListLandingZoneOperationsOutputTypeDef
        print(item)  # (3)
```

1. client: [ControlTowerClient](./client.md)
2. paginator: [ListLandingZoneOperationsPaginator](./paginators.md#listlandingzoneoperationspaginator)
3. item: `AioPageIterator[ListLandingZoneOperationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLandingZoneOperationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filter: LandingZoneOperationFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListLandingZoneOperationsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: LandingZoneOperationFilterTypeDef](./type_defs.md#landingzoneoperationfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListLandingZoneOperationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLandingZoneOperationsInputPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLandingZoneOperationsInputPaginateTypeDef](./type_defs.md#listlandingzoneoperationsinputpaginatetypedef)
## ListLandingZonesPaginator

Type annotations and code completion for `#!python session.create_client("controltower").get_paginator("list_landing_zones")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower/paginator/ListLandingZones.html#ControlTower.Paginator.ListLandingZones)

```python
# ListLandingZonesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_controltower.paginator import ListLandingZonesPaginator

session = get_session()
async with session.create_client("controltower") as client:  # (1)
    paginator: ListLandingZonesPaginator = client.get_paginator("list_landing_zones")  # (2)
    async for item in paginator.paginate(...):
        item: ListLandingZonesOutputTypeDef
        print(item)  # (3)
```

1. client: [ControlTowerClient](./client.md)
2. paginator: [ListLandingZonesPaginator](./paginators.md#listlandingzonespaginator)
3. item: `AioPageIterator[ListLandingZonesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLandingZonesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListLandingZonesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListLandingZonesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLandingZonesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLandingZonesInputPaginateTypeDef](./type_defs.md#listlandingzonesinputpaginatetypedef)
