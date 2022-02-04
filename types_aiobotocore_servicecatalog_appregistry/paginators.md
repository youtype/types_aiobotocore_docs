<a id="paginators-for-aiobotocore-appregistry-module"></a>

# Paginators for aiobotocore AppRegistry module

> [Index](..) > [AppRegistry](.) > Paginators

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
`aiobotocore.create_client("servicecatalog-appregistry").get_paginator("list_applications")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListApplicationsPaginator

def get_list_applications_paginator() -> ListApplicationsPaginator:
    return Session().create_client("servicecatalog-appregistry").get_paginator("list_applications")
```

Boto3 documentation:
[AppRegistry.Paginator.ListApplications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications)

Arguments for `ListApplicationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListApplicationsPaginator.paginate` returns
`_PageIterator`\[[ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)\].

<a id="listassociatedattributegroupspaginator"></a>

## ListAssociatedAttributeGroupsPaginator

Type annotations for
`aiobotocore.create_client("servicecatalog-appregistry").get_paginator("list_associated_attribute_groups")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListAssociatedAttributeGroupsPaginator

def get_list_associated_attribute_groups_paginator() -> ListAssociatedAttributeGroupsPaginator:
    return Session().create_client("servicecatalog-appregistry").get_paginator("list_associated_attribute_groups")
```

Boto3 documentation:
[AppRegistry.Paginator.ListAssociatedAttributeGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups)

Arguments for `ListAssociatedAttributeGroupsPaginator.paginate` method:

- `application`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAssociatedAttributeGroupsPaginator.paginate` returns
`_PageIterator`\[[ListAssociatedAttributeGroupsResponseTypeDef](./type_defs.md#listassociatedattributegroupsresponsetypedef)\].

<a id="listassociatedresourcespaginator"></a>

## ListAssociatedResourcesPaginator

Type annotations for
`aiobotocore.create_client("servicecatalog-appregistry").get_paginator("list_associated_resources")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListAssociatedResourcesPaginator

def get_list_associated_resources_paginator() -> ListAssociatedResourcesPaginator:
    return Session().create_client("servicecatalog-appregistry").get_paginator("list_associated_resources")
```

Boto3 documentation:
[AppRegistry.Paginator.ListAssociatedResources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources)

Arguments for `ListAssociatedResourcesPaginator.paginate` method:

- `application`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAssociatedResourcesPaginator.paginate` returns
`_PageIterator`\[[ListAssociatedResourcesResponseTypeDef](./type_defs.md#listassociatedresourcesresponsetypedef)\].

<a id="listattributegroupspaginator"></a>

## ListAttributeGroupsPaginator

Type annotations for
`aiobotocore.create_client("servicecatalog-appregistry").get_paginator("list_attribute_groups")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_servicecatalog_appregistry.paginator import ListAttributeGroupsPaginator

def get_list_attribute_groups_paginator() -> ListAttributeGroupsPaginator:
    return Session().create_client("servicecatalog-appregistry").get_paginator("list_attribute_groups")
```

Boto3 documentation:
[AppRegistry.Paginator.ListAttributeGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups)

Arguments for `ListAttributeGroupsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAttributeGroupsPaginator.paginate` returns
`_PageIterator`\[[ListAttributeGroupsResponseTypeDef](./type_defs.md#listattributegroupsresponsetypedef)\].
