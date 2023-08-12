# ResourceExplorer module

> [Index](../README.md) > ResourceExplorer


!!! note ""

    Auto-generated documentation for [ResourceExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
    type annotations stubs module [types-aiobotocore-resource-explorer-2](https://pypi.org/project/types-aiobotocore-resource-explorer-2/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ResourceExplorer` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[resource-explorer-2]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[resource-explorer-2]'


# standalone installation
python -m pip install types-aiobotocore-resource-explorer-2
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-resource-explorer-2
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ResourceExplorerClient

Type annotations and code completion for  `#!python session.create_client("resource-explorer-2")` as [ResourceExplorerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Client)

```python
# ResourceExplorerClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_resource_explorer_2.client import ResourceExplorerClient


session = get_session()
async with session.create_client("resource-explorer-2") as client:
    client: ResourceExplorerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("resource-explorer-2").get_paginator("...")`.

```python
# ListIndexesPaginator usage example

from types_aiobotocore_resource_explorer_2.paginator import ListIndexesPaginator

def get_list_indexes_paginator() -> ListIndexesPaginator:
    return client.get_paginator("list_indexes"))
```

- [ListIndexesPaginator](./paginators.md#listindexespaginator)
- [ListSupportedResourceTypesPaginator](./paginators.md#listsupportedresourcetypespaginator)
- [ListViewsPaginator](./paginators.md#listviewspaginator)
- [SearchPaginator](./paginators.md#searchpaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# IndexStateType usage example

from types_aiobotocore_resource_explorer_2.literals import IndexStateType

def get_value() -> IndexStateType:
    return "ACTIVE"
```

- [IndexStateType](./literals.md#indexstatetype)
- [IndexTypeType](./literals.md#indextypetype)
- [ListIndexesPaginatorName](./literals.md#listindexespaginatorname)
- [ListSupportedResourceTypesPaginatorName](./literals.md#listsupportedresourcetypespaginatorname)
- [ListViewsPaginatorName](./literals.md#listviewspaginatorname)
- [SearchPaginatorName](./literals.md#searchpaginatorname)
- [ResourceExplorerServiceName](./literals.md#resourceexplorerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AssociateDefaultViewInputRequestTypeDef](./type_defs.md#associatedefaultviewinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchGetViewErrorTypeDef](./type_defs.md#batchgetviewerrortypedef)
- [BatchGetViewInputRequestTypeDef](./type_defs.md#batchgetviewinputrequesttypedef)
- [CreateIndexInputRequestTypeDef](./type_defs.md#createindexinputrequesttypedef)
- [IncludedPropertyTypeDef](./type_defs.md#includedpropertytypedef)
- [SearchFilterTypeDef](./type_defs.md#searchfiltertypedef)
- [DeleteIndexInputRequestTypeDef](./type_defs.md#deleteindexinputrequesttypedef)
- [DeleteViewInputRequestTypeDef](./type_defs.md#deleteviewinputrequesttypedef)
- [GetViewInputRequestTypeDef](./type_defs.md#getviewinputrequesttypedef)
- [IndexTypeDef](./type_defs.md#indextypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListIndexesInputRequestTypeDef](./type_defs.md#listindexesinputrequesttypedef)
- [ListSupportedResourceTypesInputRequestTypeDef](./type_defs.md#listsupportedresourcetypesinputrequesttypedef)
- [SupportedResourceTypeTypeDef](./type_defs.md#supportedresourcetypetypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ListViewsInputRequestTypeDef](./type_defs.md#listviewsinputrequesttypedef)
- [ResourceCountTypeDef](./type_defs.md#resourcecounttypedef)
- [ResourcePropertyTypeDef](./type_defs.md#resourcepropertytypedef)
- [SearchInputRequestTypeDef](./type_defs.md#searchinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateIndexTypeInputRequestTypeDef](./type_defs.md#updateindextypeinputrequesttypedef)
- [AssociateDefaultViewOutputTypeDef](./type_defs.md#associatedefaultviewoutputtypedef)
- [CreateIndexOutputTypeDef](./type_defs.md#createindexoutputtypedef)
- [DeleteIndexOutputTypeDef](./type_defs.md#deleteindexoutputtypedef)
- [DeleteViewOutputTypeDef](./type_defs.md#deleteviewoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetDefaultViewOutputTypeDef](./type_defs.md#getdefaultviewoutputtypedef)
- [GetIndexOutputTypeDef](./type_defs.md#getindexoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [ListViewsOutputTypeDef](./type_defs.md#listviewsoutputtypedef)
- [UpdateIndexTypeOutputTypeDef](./type_defs.md#updateindextypeoutputtypedef)
- [CreateViewInputRequestTypeDef](./type_defs.md#createviewinputrequesttypedef)
- [UpdateViewInputRequestTypeDef](./type_defs.md#updateviewinputrequesttypedef)
- [ViewTypeDef](./type_defs.md#viewtypedef)
- [ListIndexesOutputTypeDef](./type_defs.md#listindexesoutputtypedef)
- [ListIndexesInputListIndexesPaginateTypeDef](./type_defs.md#listindexesinputlistindexespaginatetypedef)
- [ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef](./type_defs.md#listsupportedresourcetypesinputlistsupportedresourcetypespaginatetypedef)
- [ListViewsInputListViewsPaginateTypeDef](./type_defs.md#listviewsinputlistviewspaginatetypedef)
- [SearchInputSearchPaginateTypeDef](./type_defs.md#searchinputsearchpaginatetypedef)
- [ListSupportedResourceTypesOutputTypeDef](./type_defs.md#listsupportedresourcetypesoutputtypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [BatchGetViewOutputTypeDef](./type_defs.md#batchgetviewoutputtypedef)
- [CreateViewOutputTypeDef](./type_defs.md#createviewoutputtypedef)
- [GetViewOutputTypeDef](./type_defs.md#getviewoutputtypedef)
- [UpdateViewOutputTypeDef](./type_defs.md#updateviewoutputtypedef)
- [SearchOutputTypeDef](./type_defs.md#searchoutputtypedef)

