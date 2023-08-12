# Paginators

> [Index](../README.md) > [ControlTower](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
    type annotations stubs module [types-aiobotocore-controltower](https://pypi.org/project/types-aiobotocore-controltower/).

## ListEnabledControlsPaginator

Type annotations and code completion for `#!python session.create_client("controltower").get_paginator("list_enabled_controls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls)

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
3. item: [:material-code-braces: ListEnabledControlsOutputTypeDef](./type_defs.md#listenabledcontrolsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListEnabledControlsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    targetIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEnabledControlsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnabledControlsOutputTypeDef](./type_defs.md#listenabledcontrolsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEnabledControlsInputListEnabledControlsPaginateTypeDef = {  # (1)
    "targetIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnabledControlsInputListEnabledControlsPaginateTypeDef](./type_defs.md#listenabledcontrolsinputlistenabledcontrolspaginatetypedef) 
