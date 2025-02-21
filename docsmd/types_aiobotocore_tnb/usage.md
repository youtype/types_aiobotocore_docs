# Examples

> [Index](../README.md) > [TelcoNetworkBuilder](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [TelcoNetworkBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#telconetworkbuilder)
    type annotations stubs module [types-aiobotocore-tnb](https://pypi.org/project/types-aiobotocore-tnb/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[tnb]` package installed.

Write your `TelcoNetworkBuilder` code as usual,
type checking and code completion should work out of the box.



```python
# TelcoNetworkBuilderClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("tnb") as client:  # (1)
    result = await client.cancel_sol_network_operation()  # (2)
```

1. client: [TelcoNetworkBuilderClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListSolFunctionInstancesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("tnb") as client:  # (1)
    paginator = client.get_paginator("list_sol_function_instances")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [TelcoNetworkBuilderClient](./client.md)
2. paginator: [ListSolFunctionInstancesPaginator](./paginators.md#listsolfunctioninstancespaginator)
3. item: [:material-code-braces: ListSolFunctionInstancesOutputTypeDef](./type_defs.md#listsolfunctioninstancesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[tnb]`
or a standalone `types_aiobotocore_tnb` package, you have to explicitly specify
`client: TelcoNetworkBuilderClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# TelcoNetworkBuilderClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_tnb.client import TelcoNetworkBuilderClient
from types_aiobotocore_tnb.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_tnb.type_defs import CancelSolNetworkOperationInputTypeDef


session = get_session()

async with session.create_client("tnb") as client:
    client: TelcoNetworkBuilderClient
    kwargs: CancelSolNetworkOperationInputTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.cancel_sol_network_operation(**kwargs)
```



```python
# ListSolFunctionInstancesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_tnb.client import TelcoNetworkBuilderClient
from types_aiobotocore_tnb.paginator import ListSolFunctionInstancesPaginator
from types_aiobotocore_tnb.type_defs import ListSolFunctionInstancesOutputTypeDef


session = get_session()

async with session.create_client("tnb") as client:
    client: TelcoNetworkBuilderClient
    paginator: ListSolFunctionInstancesPaginator = client.get_paginator("list_sol_function_instances")
    async for item in paginator.paginate(...):
        item: ListSolFunctionInstancesOutputTypeDef
        print(item)
```


