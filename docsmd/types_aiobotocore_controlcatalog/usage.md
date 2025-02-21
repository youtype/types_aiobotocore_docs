# Examples

> [Index](../README.md) > [ControlCatalog](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ControlCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog.html#controlcatalog)
    type annotations stubs module [types-aiobotocore-controlcatalog](https://pypi.org/project/types-aiobotocore-controlcatalog/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[controlcatalog]` package installed.

Write your `ControlCatalog` code as usual,
type checking and code completion should work out of the box.



```python
# ControlCatalogClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("controlcatalog") as client:  # (1)
    result = await client.get_control()  # (2)
```

1. client: [ControlCatalogClient](./client.md)
2. result: [:material-code-braces: GetControlResponseTypeDef](./type_defs.md#getcontrolresponsetypedef) 



```python
# ListCommonControlsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("controlcatalog") as client:  # (1)
    paginator = client.get_paginator("list_common_controls")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ControlCatalogClient](./client.md)
2. paginator: [ListCommonControlsPaginator](./paginators.md#listcommoncontrolspaginator)
3. item: [:material-code-braces: ListCommonControlsResponseTypeDef](./type_defs.md#listcommoncontrolsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[controlcatalog]`
or a standalone `types_aiobotocore_controlcatalog` package, you have to explicitly specify
`client: ControlCatalogClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ControlCatalogClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_controlcatalog.client import ControlCatalogClient
from types_aiobotocore_controlcatalog.type_defs import GetControlResponseTypeDef
from types_aiobotocore_controlcatalog.type_defs import GetControlRequestTypeDef


session = get_session()

async with session.create_client("controlcatalog") as client:
    client: ControlCatalogClient
    kwargs: GetControlRequestTypeDef = {...}
    result: GetControlResponseTypeDef = await client.get_control(**kwargs)
```



```python
# ListCommonControlsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_controlcatalog.client import ControlCatalogClient
from types_aiobotocore_controlcatalog.paginator import ListCommonControlsPaginator
from types_aiobotocore_controlcatalog.type_defs import ListCommonControlsResponseTypeDef


session = get_session()

async with session.create_client("controlcatalog") as client:
    client: ControlCatalogClient
    paginator: ListCommonControlsPaginator = client.get_paginator("list_common_controls")
    async for item in paginator.paginate(...):
        item: ListCommonControlsResponseTypeDef
        print(item)
```


