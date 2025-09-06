# ResourceExplorer module

> [Index](../README.md) > ResourceExplorer


!!! note ""

    Auto-generated documentation for [ResourceExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#resourceexplorer)
    type annotations stubs module [types-aiobotocore-resource-explorer-2](https://pypi.org/project/types-aiobotocore-resource-explorer-2/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ResourceExplorer` service.
1. Use provided commands to install generated packages.



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
# ListIndexesForMembersPaginator usage example

from types_aiobotocore_resource_explorer_2.paginator import ListIndexesForMembersPaginator

def get_list_indexes_for_members_paginator() -> ListIndexesForMembersPaginator:
    return client.get_paginator("list_indexes_for_members"))
```

- [ListIndexesForMembersPaginator](./paginators.md#listindexesformemberspaginator)
- [ListIndexesPaginator](./paginators.md#listindexespaginator)
- [ListManagedViewsPaginator](./paginators.md#listmanagedviewspaginator)
- [ListResourcesPaginator](./paginators.md#listresourcespaginator)
- [ListSupportedResourceTypesPaginator](./paginators.md#listsupportedresourcetypespaginator)
- [ListViewsPaginator](./paginators.md#listviewspaginator)
- [SearchPaginator](./paginators.md#searchpaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AWSServiceAccessStatusType usage example

from types_aiobotocore_resource_explorer_2.literals import AWSServiceAccessStatusType

def get_value() -> AWSServiceAccessStatusType:
    return "DISABLED"
```

- [AWSServiceAccessStatusType](./literals.md#awsserviceaccessstatustype)
- [IndexStateType](./literals.md#indexstatetype)
- [IndexTypeType](./literals.md#indextypetype)
- [ListIndexesForMembersPaginatorName](./literals.md#listindexesformemberspaginatorname)
- [ListIndexesPaginatorName](./literals.md#listindexespaginatorname)
- [ListManagedViewsPaginatorName](./literals.md#listmanagedviewspaginatorname)
- [ListResourcesPaginatorName](./literals.md#listresourcespaginatorname)
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

- [AssociateDefaultViewInputTypeDef](./type_defs.md#associatedefaultviewinputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchGetViewErrorTypeDef](./type_defs.md#batchgetviewerrortypedef)
- [BatchGetViewInputTypeDef](./type_defs.md#batchgetviewinputtypedef)
- [CreateIndexInputTypeDef](./type_defs.md#createindexinputtypedef)
- [IncludedPropertyTypeDef](./type_defs.md#includedpropertytypedef)
- [SearchFilterTypeDef](./type_defs.md#searchfiltertypedef)
- [DeleteIndexInputTypeDef](./type_defs.md#deleteindexinputtypedef)
- [DeleteViewInputTypeDef](./type_defs.md#deleteviewinputtypedef)
- [OrgConfigurationTypeDef](./type_defs.md#orgconfigurationtypedef)
- [GetManagedViewInputTypeDef](./type_defs.md#getmanagedviewinputtypedef)
- [GetViewInputTypeDef](./type_defs.md#getviewinputtypedef)
- [IndexTypeDef](./type_defs.md#indextypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListIndexesForMembersInputTypeDef](./type_defs.md#listindexesformembersinputtypedef)
- [MemberIndexTypeDef](./type_defs.md#memberindextypedef)
- [ListIndexesInputTypeDef](./type_defs.md#listindexesinputtypedef)
- [ListManagedViewsInputTypeDef](./type_defs.md#listmanagedviewsinputtypedef)
- [ListSupportedResourceTypesInputTypeDef](./type_defs.md#listsupportedresourcetypesinputtypedef)
- [SupportedResourceTypeTypeDef](./type_defs.md#supportedresourcetypetypedef)
- [ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)
- [ListViewsInputTypeDef](./type_defs.md#listviewsinputtypedef)
- [ResourceCountTypeDef](./type_defs.md#resourcecounttypedef)
- [ResourcePropertyTypeDef](./type_defs.md#resourcepropertytypedef)
- [SearchInputTypeDef](./type_defs.md#searchinputtypedef)
- [TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)
- [UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)
- [UpdateIndexTypeInputTypeDef](./type_defs.md#updateindextypeinputtypedef)
- [AssociateDefaultViewOutputTypeDef](./type_defs.md#associatedefaultviewoutputtypedef)
- [CreateIndexOutputTypeDef](./type_defs.md#createindexoutputtypedef)
- [DeleteIndexOutputTypeDef](./type_defs.md#deleteindexoutputtypedef)
- [DeleteViewOutputTypeDef](./type_defs.md#deleteviewoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetDefaultViewOutputTypeDef](./type_defs.md#getdefaultviewoutputtypedef)
- [GetIndexOutputTypeDef](./type_defs.md#getindexoutputtypedef)
- [ListManagedViewsOutputTypeDef](./type_defs.md#listmanagedviewsoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [ListViewsOutputTypeDef](./type_defs.md#listviewsoutputtypedef)
- [UpdateIndexTypeOutputTypeDef](./type_defs.md#updateindextypeoutputtypedef)
- [CreateViewInputTypeDef](./type_defs.md#createviewinputtypedef)
- [ListResourcesInputTypeDef](./type_defs.md#listresourcesinputtypedef)
- [ManagedViewTypeDef](./type_defs.md#managedviewtypedef)
- [UpdateViewInputTypeDef](./type_defs.md#updateviewinputtypedef)
- [ViewTypeDef](./type_defs.md#viewtypedef)
- [GetAccountLevelServiceConfigurationOutputTypeDef](./type_defs.md#getaccountlevelserviceconfigurationoutputtypedef)
- [ListIndexesOutputTypeDef](./type_defs.md#listindexesoutputtypedef)
- [ListIndexesForMembersInputPaginateTypeDef](./type_defs.md#listindexesformembersinputpaginatetypedef)
- [ListIndexesInputPaginateTypeDef](./type_defs.md#listindexesinputpaginatetypedef)
- [ListManagedViewsInputPaginateTypeDef](./type_defs.md#listmanagedviewsinputpaginatetypedef)
- [ListResourcesInputPaginateTypeDef](./type_defs.md#listresourcesinputpaginatetypedef)
- [ListSupportedResourceTypesInputPaginateTypeDef](./type_defs.md#listsupportedresourcetypesinputpaginatetypedef)
- [ListViewsInputPaginateTypeDef](./type_defs.md#listviewsinputpaginatetypedef)
- [SearchInputPaginateTypeDef](./type_defs.md#searchinputpaginatetypedef)
- [ListIndexesForMembersOutputTypeDef](./type_defs.md#listindexesformembersoutputtypedef)
- [ListSupportedResourceTypesOutputTypeDef](./type_defs.md#listsupportedresourcetypesoutputtypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [GetManagedViewOutputTypeDef](./type_defs.md#getmanagedviewoutputtypedef)
- [BatchGetViewOutputTypeDef](./type_defs.md#batchgetviewoutputtypedef)
- [CreateViewOutputTypeDef](./type_defs.md#createviewoutputtypedef)
- [GetViewOutputTypeDef](./type_defs.md#getviewoutputtypedef)
- [UpdateViewOutputTypeDef](./type_defs.md#updateviewoutputtypedef)
- [ListResourcesOutputTypeDef](./type_defs.md#listresourcesoutputtypedef)
- [SearchOutputTypeDef](./type_defs.md#searchoutputtypedef)

