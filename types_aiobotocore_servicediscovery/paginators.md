<a id="paginators-for-aiobotocore-servicediscovery-module"></a>

# Paginators for aiobotocore ServiceDiscovery module

> [Index](..) > [ServiceDiscovery](.) > Paginators

Auto-generated documentation for
[ServiceDiscovery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
type annotations stubs module
[types-aiobotocore-servicediscovery](https://pypi.org/project/types-aiobotocore-servicediscovery/).

- [Paginators for aiobotocore ServiceDiscovery module](#paginators-for-aiobotocore-servicediscovery-module)
  - [ListInstancesPaginator](#listinstancespaginator)
  - [ListNamespacesPaginator](#listnamespacespaginator)
  - [ListOperationsPaginator](#listoperationspaginator)
  - [ListServicesPaginator](#listservicespaginator)

<a id="listinstancespaginator"></a>

## ListInstancesPaginator

Type annotations for
`aiobotocore.create_client("servicediscovery").get_paginator("list_instances")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_servicediscovery.paginator import ListInstancesPaginator

def get_list_instances_paginator() -> ListInstancesPaginator:
    return Session().create_client("servicediscovery").get_paginator("list_instances")
```

Boto3 documentation:
[ServiceDiscovery.Paginator.ListInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListInstances)

Arguments for `ListInstancesPaginator.paginate` method:

- `ServiceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInstancesPaginator.paginate` returns
`_PageIterator`\[[ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef)\].

<a id="listnamespacespaginator"></a>

## ListNamespacesPaginator

Type annotations for
`aiobotocore.create_client("servicediscovery").get_paginator("list_namespaces")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_servicediscovery.paginator import ListNamespacesPaginator

def get_list_namespaces_paginator() -> ListNamespacesPaginator:
    return Session().create_client("servicediscovery").get_paginator("list_namespaces")
```

Boto3 documentation:
[ServiceDiscovery.Paginator.ListNamespaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListNamespaces)

Arguments for `ListNamespacesPaginator.paginate` method:

- `Filters`:
  `Sequence`\[[NamespaceFilterTypeDef](./type_defs.md#namespacefiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListNamespacesPaginator.paginate` returns
`_PageIterator`\[[ListNamespacesResponseTypeDef](./type_defs.md#listnamespacesresponsetypedef)\].

<a id="listoperationspaginator"></a>

## ListOperationsPaginator

Type annotations for
`aiobotocore.create_client("servicediscovery").get_paginator("list_operations")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_servicediscovery.paginator import ListOperationsPaginator

def get_list_operations_paginator() -> ListOperationsPaginator:
    return Session().create_client("servicediscovery").get_paginator("list_operations")
```

Boto3 documentation:
[ServiceDiscovery.Paginator.ListOperations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListOperations)

Arguments for `ListOperationsPaginator.paginate` method:

- `Filters`:
  `Sequence`\[[OperationFilterTypeDef](./type_defs.md#operationfiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOperationsPaginator.paginate` returns
`_PageIterator`\[[ListOperationsResponseTypeDef](./type_defs.md#listoperationsresponsetypedef)\].

<a id="listservicespaginator"></a>

## ListServicesPaginator

Type annotations for
`aiobotocore.create_client("servicediscovery").get_paginator("list_services")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_servicediscovery.paginator import ListServicesPaginator

def get_list_services_paginator() -> ListServicesPaginator:
    return Session().create_client("servicediscovery").get_paginator("list_services")
```

Boto3 documentation:
[ServiceDiscovery.Paginator.ListServices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListServices)

Arguments for `ListServicesPaginator.paginate` method:

- `Filters`:
  `Sequence`\[[ServiceFilterTypeDef](./type_defs.md#servicefiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListServicesPaginator.paginate` returns
`_PageIterator`\[[ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef)\].
