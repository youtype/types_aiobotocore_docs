# Paginators

> [Index](../README.md) > [TelcoNetworkBuilder](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [TelcoNetworkBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
    type annotations stubs module [types-aiobotocore-tnb](https://pypi.org/project/types-aiobotocore-tnb/).

## ListSolFunctionInstancesPaginator

Type annotations and code completion for `#!python session.create_client("tnb").get_paginator("list_sol_function_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionInstances)

```python
# ListSolFunctionInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_tnb.paginator import ListSolFunctionInstancesPaginator

session = get_session()
async with session.create_client("tnb") as client:  # (1)
    paginator: ListSolFunctionInstancesPaginator = client.get_paginator("list_sol_function_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListSolFunctionInstancesOutputTypeDef
        print(item)  # (3)
```

1. client: [TelcoNetworkBuilderClient](./client.md)
2. paginator: [ListSolFunctionInstancesPaginator](./paginators.md#listsolfunctioninstancespaginator)
3. item: [:material-code-braces: ListSolFunctionInstancesOutputTypeDef](./type_defs.md#listsolfunctioninstancesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSolFunctionInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSolFunctionInstancesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSolFunctionInstancesOutputTypeDef](./type_defs.md#listsolfunctioninstancesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef](./type_defs.md#listsolfunctioninstancesinputlistsolfunctioninstancespaginatetypedef) 
## ListSolFunctionPackagesPaginator

Type annotations and code completion for `#!python session.create_client("tnb").get_paginator("list_sol_function_packages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionPackages)

```python
# ListSolFunctionPackagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_tnb.paginator import ListSolFunctionPackagesPaginator

session = get_session()
async with session.create_client("tnb") as client:  # (1)
    paginator: ListSolFunctionPackagesPaginator = client.get_paginator("list_sol_function_packages")  # (2)
    async for item in paginator.paginate(...):
        item: ListSolFunctionPackagesOutputTypeDef
        print(item)  # (3)
```

1. client: [TelcoNetworkBuilderClient](./client.md)
2. paginator: [ListSolFunctionPackagesPaginator](./paginators.md#listsolfunctionpackagespaginator)
3. item: [:material-code-braces: ListSolFunctionPackagesOutputTypeDef](./type_defs.md#listsolfunctionpackagesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSolFunctionPackagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSolFunctionPackagesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSolFunctionPackagesOutputTypeDef](./type_defs.md#listsolfunctionpackagesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef](./type_defs.md#listsolfunctionpackagesinputlistsolfunctionpackagespaginatetypedef) 
## ListSolNetworkInstancesPaginator

Type annotations and code completion for `#!python session.create_client("tnb").get_paginator("list_sol_network_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkInstances)

```python
# ListSolNetworkInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_tnb.paginator import ListSolNetworkInstancesPaginator

session = get_session()
async with session.create_client("tnb") as client:  # (1)
    paginator: ListSolNetworkInstancesPaginator = client.get_paginator("list_sol_network_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListSolNetworkInstancesOutputTypeDef
        print(item)  # (3)
```

1. client: [TelcoNetworkBuilderClient](./client.md)
2. paginator: [ListSolNetworkInstancesPaginator](./paginators.md#listsolnetworkinstancespaginator)
3. item: [:material-code-braces: ListSolNetworkInstancesOutputTypeDef](./type_defs.md#listsolnetworkinstancesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSolNetworkInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSolNetworkInstancesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSolNetworkInstancesOutputTypeDef](./type_defs.md#listsolnetworkinstancesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef](./type_defs.md#listsolnetworkinstancesinputlistsolnetworkinstancespaginatetypedef) 
## ListSolNetworkOperationsPaginator

Type annotations and code completion for `#!python session.create_client("tnb").get_paginator("list_sol_network_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkOperations)

```python
# ListSolNetworkOperationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_tnb.paginator import ListSolNetworkOperationsPaginator

session = get_session()
async with session.create_client("tnb") as client:  # (1)
    paginator: ListSolNetworkOperationsPaginator = client.get_paginator("list_sol_network_operations")  # (2)
    async for item in paginator.paginate(...):
        item: ListSolNetworkOperationsOutputTypeDef
        print(item)  # (3)
```

1. client: [TelcoNetworkBuilderClient](./client.md)
2. paginator: [ListSolNetworkOperationsPaginator](./paginators.md#listsolnetworkoperationspaginator)
3. item: [:material-code-braces: ListSolNetworkOperationsOutputTypeDef](./type_defs.md#listsolnetworkoperationsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSolNetworkOperationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSolNetworkOperationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSolNetworkOperationsOutputTypeDef](./type_defs.md#listsolnetworkoperationsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef](./type_defs.md#listsolnetworkoperationsinputlistsolnetworkoperationspaginatetypedef) 
## ListSolNetworkPackagesPaginator

Type annotations and code completion for `#!python session.create_client("tnb").get_paginator("list_sol_network_packages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkPackages)

```python
# ListSolNetworkPackagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_tnb.paginator import ListSolNetworkPackagesPaginator

session = get_session()
async with session.create_client("tnb") as client:  # (1)
    paginator: ListSolNetworkPackagesPaginator = client.get_paginator("list_sol_network_packages")  # (2)
    async for item in paginator.paginate(...):
        item: ListSolNetworkPackagesOutputTypeDef
        print(item)  # (3)
```

1. client: [TelcoNetworkBuilderClient](./client.md)
2. paginator: [ListSolNetworkPackagesPaginator](./paginators.md#listsolnetworkpackagespaginator)
3. item: [:material-code-braces: ListSolNetworkPackagesOutputTypeDef](./type_defs.md#listsolnetworkpackagesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSolNetworkPackagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSolNetworkPackagesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSolNetworkPackagesOutputTypeDef](./type_defs.md#listsolnetworkpackagesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef](./type_defs.md#listsolnetworkpackagesinputlistsolnetworkpackagespaginatetypedef) 
