<a id="paginators-for-aiobotocore-appregistry-module"></a>

# Paginators for aiobotocore AppRegistry module

> [Index](../README.md) > [AppRegistry](./README.md) > Paginators

Auto-generated documentation for
[AppRegistry](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
type annotations stubs module
[types-aiobotocore-servicecatalog-appregistry](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry/).

- [Paginators for aiobotocore AppRegistry module](#paginators-for-aiobotocore-appregistry-module)
  - [ListApplicationsPaginator](#listapplicationspaginator)
  - [ListAssociatedAttributeGroupsPaginator](#listassociatedattributegroupspaginator)
  - [ListAssociatedResourcesPaginator](#listassociatedresourcespaginator)
  - [ListAttributeGroupsPaginator](#listattributegroupspaginator)

<a id="listapplicationspaginator"></a>

## ListApplicationsPaginator

Type annotations for
`session.create_client("servicecatalog-appregistry").get_paginator("list_applications")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("servicecatalog-appregistry") as client:
    client: AppRegistryClient
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
```

Boto3 documentation:
[AppRegistry.Paginator.ListApplications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications)

Arguments for `ListApplicationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListApplicationsPaginator.paginate` returns
`AsyncIterator`\[[ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)\].

<a id="listassociatedattributegroupspaginator"></a>

## ListAssociatedAttributeGroupsPaginator

Type annotations for
`session.create_client("servicecatalog-appregistry").get_paginator("list_associated_attribute_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListAssociatedAttributeGroupsPaginator

session = get_session()
async with session.create_client("servicecatalog-appregistry") as client:
    client: AppRegistryClient
    paginator: ListAssociatedAttributeGroupsPaginator = client.get_paginator("list_associated_attribute_groups")
```

Boto3 documentation:
[AppRegistry.Paginator.ListAssociatedAttributeGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups)

Arguments for `ListAssociatedAttributeGroupsPaginator.paginate` method:

- `application`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAssociatedAttributeGroupsPaginator.paginate` returns
`AsyncIterator`\[[ListAssociatedAttributeGroupsResponseTypeDef](./type_defs.md#listassociatedattributegroupsresponsetypedef)\].

<a id="listassociatedresourcespaginator"></a>

## ListAssociatedResourcesPaginator

Type annotations for
`session.create_client("servicecatalog-appregistry").get_paginator("list_associated_resources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListAssociatedResourcesPaginator

session = get_session()
async with session.create_client("servicecatalog-appregistry") as client:
    client: AppRegistryClient
    paginator: ListAssociatedResourcesPaginator = client.get_paginator("list_associated_resources")
```

Boto3 documentation:
[AppRegistry.Paginator.ListAssociatedResources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources)

Arguments for `ListAssociatedResourcesPaginator.paginate` method:

- `application`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAssociatedResourcesPaginator.paginate` returns
`AsyncIterator`\[[ListAssociatedResourcesResponseTypeDef](./type_defs.md#listassociatedresourcesresponsetypedef)\].

<a id="listattributegroupspaginator"></a>

## ListAttributeGroupsPaginator

Type annotations for
`session.create_client("servicecatalog-appregistry").get_paginator("list_attribute_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListAttributeGroupsPaginator

session = get_session()
async with session.create_client("servicecatalog-appregistry") as client:
    client: AppRegistryClient
    paginator: ListAttributeGroupsPaginator = client.get_paginator("list_attribute_groups")
```

Boto3 documentation:
[AppRegistry.Paginator.ListAttributeGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups)

Arguments for `ListAttributeGroupsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAttributeGroupsPaginator.paginate` returns
`AsyncIterator`\[[ListAttributeGroupsResponseTypeDef](./type_defs.md#listattributegroupsresponsetypedef)\].
