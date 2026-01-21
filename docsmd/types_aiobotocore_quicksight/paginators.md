# Paginators

> [Index](../README.md) > [QuickSight](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [QuickSight](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#quicksight)
    type annotations stubs module [types-aiobotocore-quicksight](https://pypi.org/project/types-aiobotocore-quicksight/).

## DescribeFolderPermissionsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("describe_folder_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/DescribeFolderPermissions.html#QuickSight.Paginator.DescribeFolderPermissions)

```python
# DescribeFolderPermissionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import DescribeFolderPermissionsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: DescribeFolderPermissionsPaginator = client.get_paginator("describe_folder_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFolderPermissionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [DescribeFolderPermissionsPaginator](./paginators.md#describefolderpermissionspaginator)
3. item: `AioPageIterator[DescribeFolderPermissionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeFolderPermissionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
    Namespace: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeFolderPermissionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeFolderPermissionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFolderPermissionsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFolderPermissionsRequestPaginateTypeDef](./type_defs.md#describefolderpermissionsrequestpaginatetypedef)
## DescribeFolderResolvedPermissionsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("describe_folder_resolved_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/DescribeFolderResolvedPermissions.html#QuickSight.Paginator.DescribeFolderResolvedPermissions)

```python
# DescribeFolderResolvedPermissionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import DescribeFolderResolvedPermissionsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: DescribeFolderResolvedPermissionsPaginator = client.get_paginator("describe_folder_resolved_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFolderResolvedPermissionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [DescribeFolderResolvedPermissionsPaginator](./paginators.md#describefolderresolvedpermissionspaginator)
3. item: `AioPageIterator[DescribeFolderResolvedPermissionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeFolderResolvedPermissionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
    Namespace: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeFolderResolvedPermissionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeFolderResolvedPermissionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFolderResolvedPermissionsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFolderResolvedPermissionsRequestPaginateTypeDef](./type_defs.md#describefolderresolvedpermissionsrequestpaginatetypedef)
## ListActionConnectorsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_action_connectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListActionConnectors.html#QuickSight.Paginator.ListActionConnectors)

```python
# ListActionConnectorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListActionConnectorsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListActionConnectorsPaginator = client.get_paginator("list_action_connectors")  # (2)
    async for item in paginator.paginate(...):
        item: ListActionConnectorsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListActionConnectorsPaginator](./paginators.md#listactionconnectorspaginator)
3. item: `AioPageIterator[ListActionConnectorsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListActionConnectorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListActionConnectorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListActionConnectorsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListActionConnectorsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListActionConnectorsRequestPaginateTypeDef](./type_defs.md#listactionconnectorsrequestpaginatetypedef)
## ListAnalysesPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_analyses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListAnalyses.html#QuickSight.Paginator.ListAnalyses)

```python
# ListAnalysesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListAnalysesPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListAnalysesPaginator = client.get_paginator("list_analyses")  # (2)
    async for item in paginator.paginate(...):
        item: ListAnalysesResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListAnalysesPaginator](./paginators.md#listanalysespaginator)
3. item: `AioPageIterator[ListAnalysesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAnalysesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAnalysesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAnalysesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAnalysesRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAnalysesRequestPaginateTypeDef](./type_defs.md#listanalysesrequestpaginatetypedef)
## ListAssetBundleExportJobsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_asset_bundle_export_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListAssetBundleExportJobs.html#QuickSight.Paginator.ListAssetBundleExportJobs)

```python
# ListAssetBundleExportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListAssetBundleExportJobsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListAssetBundleExportJobsPaginator = client.get_paginator("list_asset_bundle_export_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetBundleExportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListAssetBundleExportJobsPaginator](./paginators.md#listassetbundleexportjobspaginator)
3. item: `AioPageIterator[ListAssetBundleExportJobsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAssetBundleExportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAssetBundleExportJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAssetBundleExportJobsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAssetBundleExportJobsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetBundleExportJobsRequestPaginateTypeDef](./type_defs.md#listassetbundleexportjobsrequestpaginatetypedef)
## ListAssetBundleImportJobsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_asset_bundle_import_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListAssetBundleImportJobs.html#QuickSight.Paginator.ListAssetBundleImportJobs)

```python
# ListAssetBundleImportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListAssetBundleImportJobsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListAssetBundleImportJobsPaginator = client.get_paginator("list_asset_bundle_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetBundleImportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListAssetBundleImportJobsPaginator](./paginators.md#listassetbundleimportjobspaginator)
3. item: `AioPageIterator[ListAssetBundleImportJobsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAssetBundleImportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAssetBundleImportJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAssetBundleImportJobsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAssetBundleImportJobsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetBundleImportJobsRequestPaginateTypeDef](./type_defs.md#listassetbundleimportjobsrequestpaginatetypedef)
## ListBrandsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_brands")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListBrands.html#QuickSight.Paginator.ListBrands)

```python
# ListBrandsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListBrandsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListBrandsPaginator = client.get_paginator("list_brands")  # (2)
    async for item in paginator.paginate(...):
        item: ListBrandsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListBrandsPaginator](./paginators.md#listbrandspaginator)
3. item: `AioPageIterator[ListBrandsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBrandsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBrandsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBrandsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBrandsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBrandsRequestPaginateTypeDef](./type_defs.md#listbrandsrequestpaginatetypedef)
## ListCustomPermissionsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_custom_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListCustomPermissions.html#QuickSight.Paginator.ListCustomPermissions)

```python
# ListCustomPermissionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListCustomPermissionsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListCustomPermissionsPaginator = client.get_paginator("list_custom_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomPermissionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListCustomPermissionsPaginator](./paginators.md#listcustompermissionspaginator)
3. item: `AioPageIterator[ListCustomPermissionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCustomPermissionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCustomPermissionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCustomPermissionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomPermissionsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomPermissionsRequestPaginateTypeDef](./type_defs.md#listcustompermissionsrequestpaginatetypedef)
## ListDashboardVersionsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_dashboard_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListDashboardVersions.html#QuickSight.Paginator.ListDashboardVersions)

```python
# ListDashboardVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListDashboardVersionsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListDashboardVersionsPaginator = client.get_paginator("list_dashboard_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDashboardVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListDashboardVersionsPaginator](./paginators.md#listdashboardversionspaginator)
3. item: `AioPageIterator[ListDashboardVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDashboardVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDashboardVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDashboardVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDashboardVersionsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDashboardVersionsRequestPaginateTypeDef](./type_defs.md#listdashboardversionsrequestpaginatetypedef)
## ListDashboardsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_dashboards")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListDashboards.html#QuickSight.Paginator.ListDashboards)

```python
# ListDashboardsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListDashboardsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListDashboardsPaginator = client.get_paginator("list_dashboards")  # (2)
    async for item in paginator.paginate(...):
        item: ListDashboardsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListDashboardsPaginator](./paginators.md#listdashboardspaginator)
3. item: `AioPageIterator[ListDashboardsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDashboardsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDashboardsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDashboardsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDashboardsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDashboardsRequestPaginateTypeDef](./type_defs.md#listdashboardsrequestpaginatetypedef)
## ListDataSetsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_data_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListDataSets.html#QuickSight.Paginator.ListDataSets)

```python
# ListDataSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListDataSetsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListDataSetsPaginator = client.get_paginator("list_data_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListDataSetsPaginator](./paginators.md#listdatasetspaginator)
3. item: `AioPageIterator[ListDataSetsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDataSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataSetsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSetsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSetsRequestPaginateTypeDef](./type_defs.md#listdatasetsrequestpaginatetypedef)
## ListDataSourcesPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_data_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListDataSources.html#QuickSight.Paginator.ListDataSources)

```python
# ListDataSourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListDataSourcesPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListDataSourcesPaginator = client.get_paginator("list_data_sources")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
3. item: `AioPageIterator[ListDataSourcesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataSourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDataSourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataSourcesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSourcesRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesRequestPaginateTypeDef](./type_defs.md#listdatasourcesrequestpaginatetypedef)
## ListFlowsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_flows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListFlows.html#QuickSight.Paginator.ListFlows)

```python
# ListFlowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListFlowsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListFlowsPaginator = client.get_paginator("list_flows")  # (2)
    async for item in paginator.paginate(...):
        item: ListFlowsOutputTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListFlowsPaginator](./paginators.md#listflowspaginator)
3. item: `AioPageIterator[ListFlowsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFlowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFlowsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFlowsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFlowsInputPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowsInputPaginateTypeDef](./type_defs.md#listflowsinputpaginatetypedef)
## ListFolderMembersPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_folder_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListFolderMembers.html#QuickSight.Paginator.ListFolderMembers)

```python
# ListFolderMembersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListFolderMembersPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListFolderMembersPaginator = client.get_paginator("list_folder_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListFolderMembersResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListFolderMembersPaginator](./paginators.md#listfoldermemberspaginator)
3. item: `AioPageIterator[ListFolderMembersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFolderMembersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFolderMembersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFolderMembersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFolderMembersRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFolderMembersRequestPaginateTypeDef](./type_defs.md#listfoldermembersrequestpaginatetypedef)
## ListFoldersForResourcePaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_folders_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListFoldersForResource.html#QuickSight.Paginator.ListFoldersForResource)

```python
# ListFoldersForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListFoldersForResourcePaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListFoldersForResourcePaginator = client.get_paginator("list_folders_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListFoldersForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListFoldersForResourcePaginator](./paginators.md#listfoldersforresourcepaginator)
3. item: `AioPageIterator[ListFoldersForResourceResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFoldersForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFoldersForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFoldersForResourceResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFoldersForResourceRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFoldersForResourceRequestPaginateTypeDef](./type_defs.md#listfoldersforresourcerequestpaginatetypedef)
## ListFoldersPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_folders")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListFolders.html#QuickSight.Paginator.ListFolders)

```python
# ListFoldersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListFoldersPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListFoldersPaginator = client.get_paginator("list_folders")  # (2)
    async for item in paginator.paginate(...):
        item: ListFoldersResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListFoldersPaginator](./paginators.md#listfolderspaginator)
3. item: `AioPageIterator[ListFoldersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFoldersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFoldersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFoldersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFoldersRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFoldersRequestPaginateTypeDef](./type_defs.md#listfoldersrequestpaginatetypedef)
## ListGroupMembershipsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_group_memberships")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListGroupMemberships.html#QuickSight.Paginator.ListGroupMemberships)

```python
# ListGroupMembershipsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListGroupMembershipsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListGroupMembershipsPaginator = client.get_paginator("list_group_memberships")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupMembershipsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListGroupMembershipsPaginator](./paginators.md#listgroupmembershipspaginator)
3. item: `AioPageIterator[ListGroupMembershipsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGroupMembershipsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListGroupMembershipsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListGroupMembershipsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupMembershipsRequestPaginateTypeDef = {  # (1)
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupMembershipsRequestPaginateTypeDef](./type_defs.md#listgroupmembershipsrequestpaginatetypedef)
## ListGroupsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListGroups.html#QuickSight.Paginator.ListGroups)

```python
# ListGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListGroupsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListGroupsPaginator](./paginators.md#listgroupspaginator)
3. item: `AioPageIterator[ListGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    Namespace: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestPaginateTypeDef](./type_defs.md#listgroupsrequestpaginatetypedef)
## ListIAMPolicyAssignmentsForUserPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_iam_policy_assignments_for_user")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListIAMPolicyAssignmentsForUser.html#QuickSight.Paginator.ListIAMPolicyAssignmentsForUser)

```python
# ListIAMPolicyAssignmentsForUserPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListIAMPolicyAssignmentsForUserPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListIAMPolicyAssignmentsForUserPaginator = client.get_paginator("list_iam_policy_assignments_for_user")  # (2)
    async for item in paginator.paginate(...):
        item: ListIAMPolicyAssignmentsForUserResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListIAMPolicyAssignmentsForUserPaginator](./paginators.md#listiampolicyassignmentsforuserpaginator)
3. item: `AioPageIterator[ListIAMPolicyAssignmentsForUserResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIAMPolicyAssignmentsForUserPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    UserName: str,
    Namespace: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListIAMPolicyAssignmentsForUserResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListIAMPolicyAssignmentsForUserResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIAMPolicyAssignmentsForUserRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "UserName": ...,
    "Namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIAMPolicyAssignmentsForUserRequestPaginateTypeDef](./type_defs.md#listiampolicyassignmentsforuserrequestpaginatetypedef)
## ListIAMPolicyAssignmentsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_iam_policy_assignments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListIAMPolicyAssignments.html#QuickSight.Paginator.ListIAMPolicyAssignments)

```python
# ListIAMPolicyAssignmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListIAMPolicyAssignmentsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListIAMPolicyAssignmentsPaginator = client.get_paginator("list_iam_policy_assignments")  # (2)
    async for item in paginator.paginate(...):
        item: ListIAMPolicyAssignmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListIAMPolicyAssignmentsPaginator](./paginators.md#listiampolicyassignmentspaginator)
3. item: `AioPageIterator[ListIAMPolicyAssignmentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIAMPolicyAssignmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    Namespace: str,
    AssignmentStatus: AssignmentStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListIAMPolicyAssignmentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListIAMPolicyAssignmentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIAMPolicyAssignmentsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIAMPolicyAssignmentsRequestPaginateTypeDef](./type_defs.md#listiampolicyassignmentsrequestpaginatetypedef)
## ListIngestionsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_ingestions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListIngestions.html#QuickSight.Paginator.ListIngestions)

```python
# ListIngestionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListIngestionsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListIngestionsPaginator = client.get_paginator("list_ingestions")  # (2)
    async for item in paginator.paginate(...):
        item: ListIngestionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListIngestionsPaginator](./paginators.md#listingestionspaginator)
3. item: `AioPageIterator[ListIngestionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIngestionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DataSetId: str,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListIngestionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListIngestionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIngestionsRequestPaginateTypeDef = {  # (1)
    "DataSetId": ...,
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIngestionsRequestPaginateTypeDef](./type_defs.md#listingestionsrequestpaginatetypedef)
## ListNamespacesPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_namespaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListNamespaces.html#QuickSight.Paginator.ListNamespaces)

```python
# ListNamespacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListNamespacesPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListNamespacesPaginator = client.get_paginator("list_namespaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListNamespacesResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListNamespacesPaginator](./paginators.md#listnamespacespaginator)
3. item: `AioPageIterator[ListNamespacesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListNamespacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListNamespacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListNamespacesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListNamespacesRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNamespacesRequestPaginateTypeDef](./type_defs.md#listnamespacesrequestpaginatetypedef)
## ListRoleMembershipsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_role_memberships")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListRoleMemberships.html#QuickSight.Paginator.ListRoleMemberships)

```python
# ListRoleMembershipsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListRoleMembershipsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListRoleMembershipsPaginator = client.get_paginator("list_role_memberships")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoleMembershipsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListRoleMembershipsPaginator](./paginators.md#listrolemembershipspaginator)
3. item: `AioPageIterator[ListRoleMembershipsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRoleMembershipsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Role: RoleType,  # (1)
    AwsAccountId: str,
    Namespace: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListRoleMembershipsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListRoleMembershipsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRoleMembershipsRequestPaginateTypeDef = {  # (1)
    "Role": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoleMembershipsRequestPaginateTypeDef](./type_defs.md#listrolemembershipsrequestpaginatetypedef)
## ListTemplateAliasesPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_template_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListTemplateAliases.html#QuickSight.Paginator.ListTemplateAliases)

```python
# ListTemplateAliasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListTemplateAliasesPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListTemplateAliasesPaginator = client.get_paginator("list_template_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListTemplateAliasesResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListTemplateAliasesPaginator](./paginators.md#listtemplatealiasespaginator)
3. item: `AioPageIterator[ListTemplateAliasesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTemplateAliasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTemplateAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTemplateAliasesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTemplateAliasesRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTemplateAliasesRequestPaginateTypeDef](./type_defs.md#listtemplatealiasesrequestpaginatetypedef)
## ListTemplateVersionsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_template_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListTemplateVersions.html#QuickSight.Paginator.ListTemplateVersions)

```python
# ListTemplateVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListTemplateVersionsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListTemplateVersionsPaginator = client.get_paginator("list_template_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListTemplateVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListTemplateVersionsPaginator](./paginators.md#listtemplateversionspaginator)
3. item: `AioPageIterator[ListTemplateVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTemplateVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTemplateVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTemplateVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTemplateVersionsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTemplateVersionsRequestPaginateTypeDef](./type_defs.md#listtemplateversionsrequestpaginatetypedef)
## ListTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListTemplates.html#QuickSight.Paginator.ListTemplates)

```python
# ListTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListTemplatesPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListTemplatesPaginator = client.get_paginator("list_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListTemplatesPaginator](./paginators.md#listtemplatespaginator)
3. item: `AioPageIterator[ListTemplatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTemplatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTemplatesRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTemplatesRequestPaginateTypeDef](./type_defs.md#listtemplatesrequestpaginatetypedef)
## ListThemeVersionsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_theme_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListThemeVersions.html#QuickSight.Paginator.ListThemeVersions)

```python
# ListThemeVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListThemeVersionsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListThemeVersionsPaginator = client.get_paginator("list_theme_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListThemeVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListThemeVersionsPaginator](./paginators.md#listthemeversionspaginator)
3. item: `AioPageIterator[ListThemeVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThemeVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListThemeVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListThemeVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThemeVersionsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThemeVersionsRequestPaginateTypeDef](./type_defs.md#listthemeversionsrequestpaginatetypedef)
## ListThemesPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_themes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListThemes.html#QuickSight.Paginator.ListThemes)

```python
# ListThemesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListThemesPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListThemesPaginator = client.get_paginator("list_themes")  # (2)
    async for item in paginator.paginate(...):
        item: ListThemesResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListThemesPaginator](./paginators.md#listthemespaginator)
3. item: `AioPageIterator[ListThemesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThemesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    Type: ThemeTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListThemesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ThemeTypeType](./literals.md#themetypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListThemesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThemesRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThemesRequestPaginateTypeDef](./type_defs.md#listthemesrequestpaginatetypedef)
## ListUserGroupsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_user_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListUserGroups.html#QuickSight.Paginator.ListUserGroups)

```python
# ListUserGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListUserGroupsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListUserGroupsPaginator = client.get_paginator("list_user_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListUserGroupsPaginator](./paginators.md#listusergroupspaginator)
3. item: `AioPageIterator[ListUserGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListUserGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserName: str,
    AwsAccountId: str,
    Namespace: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListUserGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListUserGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListUserGroupsRequestPaginateTypeDef = {  # (1)
    "UserName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserGroupsRequestPaginateTypeDef](./type_defs.md#listusergroupsrequestpaginatetypedef)
## ListUsersPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/ListUsers.html#QuickSight.Paginator.ListUsers)

```python
# ListUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: `AioPageIterator[ListUsersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    Namespace: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListUsersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListUsersRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestPaginateTypeDef](./type_defs.md#listusersrequestpaginatetypedef)
## SearchActionConnectorsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("search_action_connectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/SearchActionConnectors.html#QuickSight.Paginator.SearchActionConnectors)

```python
# SearchActionConnectorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import SearchActionConnectorsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: SearchActionConnectorsPaginator = client.get_paginator("search_action_connectors")  # (2)
    async for item in paginator.paginate(...):
        item: SearchActionConnectorsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [SearchActionConnectorsPaginator](./paginators.md#searchactionconnectorspaginator)
3. item: `AioPageIterator[SearchActionConnectorsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchActionConnectorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[ActionConnectorSearchFilterTypeDef],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchActionConnectorsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[ActionConnectorSearchFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchActionConnectorsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchActionConnectorsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchActionConnectorsRequestPaginateTypeDef](./type_defs.md#searchactionconnectorsrequestpaginatetypedef)
## SearchAnalysesPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("search_analyses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/SearchAnalyses.html#QuickSight.Paginator.SearchAnalyses)

```python
# SearchAnalysesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import SearchAnalysesPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: SearchAnalysesPaginator = client.get_paginator("search_analyses")  # (2)
    async for item in paginator.paginate(...):
        item: SearchAnalysesResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [SearchAnalysesPaginator](./paginators.md#searchanalysespaginator)
3. item: `AioPageIterator[SearchAnalysesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchAnalysesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[AnalysisSearchFilterTypeDef],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchAnalysesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[AnalysisSearchFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchAnalysesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchAnalysesRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchAnalysesRequestPaginateTypeDef](./type_defs.md#searchanalysesrequestpaginatetypedef)
## SearchDashboardsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("search_dashboards")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/SearchDashboards.html#QuickSight.Paginator.SearchDashboards)

```python
# SearchDashboardsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import SearchDashboardsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: SearchDashboardsPaginator = client.get_paginator("search_dashboards")  # (2)
    async for item in paginator.paginate(...):
        item: SearchDashboardsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [SearchDashboardsPaginator](./paginators.md#searchdashboardspaginator)
3. item: `AioPageIterator[SearchDashboardsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchDashboardsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[DashboardSearchFilterTypeDef],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchDashboardsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[DashboardSearchFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchDashboardsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchDashboardsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchDashboardsRequestPaginateTypeDef](./type_defs.md#searchdashboardsrequestpaginatetypedef)
## SearchDataSetsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("search_data_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/SearchDataSets.html#QuickSight.Paginator.SearchDataSets)

```python
# SearchDataSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import SearchDataSetsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: SearchDataSetsPaginator = client.get_paginator("search_data_sets")  # (2)
    async for item in paginator.paginate(...):
        item: SearchDataSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [SearchDataSetsPaginator](./paginators.md#searchdatasetspaginator)
3. item: `AioPageIterator[SearchDataSetsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchDataSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[DataSetSearchFilterTypeDef],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchDataSetsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[DataSetSearchFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchDataSetsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchDataSetsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchDataSetsRequestPaginateTypeDef](./type_defs.md#searchdatasetsrequestpaginatetypedef)
## SearchDataSourcesPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("search_data_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/SearchDataSources.html#QuickSight.Paginator.SearchDataSources)

```python
# SearchDataSourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import SearchDataSourcesPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: SearchDataSourcesPaginator = client.get_paginator("search_data_sources")  # (2)
    async for item in paginator.paginate(...):
        item: SearchDataSourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [SearchDataSourcesPaginator](./paginators.md#searchdatasourcespaginator)
3. item: `AioPageIterator[SearchDataSourcesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchDataSourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[DataSourceSearchFilterTypeDef],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchDataSourcesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[DataSourceSearchFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchDataSourcesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchDataSourcesRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchDataSourcesRequestPaginateTypeDef](./type_defs.md#searchdatasourcesrequestpaginatetypedef)
## SearchFlowsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("search_flows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/SearchFlows.html#QuickSight.Paginator.SearchFlows)

```python
# SearchFlowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import SearchFlowsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: SearchFlowsPaginator = client.get_paginator("search_flows")  # (2)
    async for item in paginator.paginate(...):
        item: SearchFlowsOutputTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [SearchFlowsPaginator](./paginators.md#searchflowspaginator)
3. item: `AioPageIterator[SearchFlowsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchFlowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[SearchFlowsFilterTypeDef],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchFlowsOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[SearchFlowsFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchFlowsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchFlowsInputPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchFlowsInputPaginateTypeDef](./type_defs.md#searchflowsinputpaginatetypedef)
## SearchFoldersPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("search_folders")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/SearchFolders.html#QuickSight.Paginator.SearchFolders)

```python
# SearchFoldersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import SearchFoldersPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: SearchFoldersPaginator = client.get_paginator("search_folders")  # (2)
    async for item in paginator.paginate(...):
        item: SearchFoldersResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [SearchFoldersPaginator](./paginators.md#searchfolderspaginator)
3. item: `AioPageIterator[SearchFoldersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchFoldersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[FolderSearchFilterTypeDef],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchFoldersResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[FolderSearchFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchFoldersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchFoldersRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchFoldersRequestPaginateTypeDef](./type_defs.md#searchfoldersrequestpaginatetypedef)
## SearchGroupsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("search_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/SearchGroups.html#QuickSight.Paginator.SearchGroups)

```python
# SearchGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import SearchGroupsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: SearchGroupsPaginator = client.get_paginator("search_groups")  # (2)
    async for item in paginator.paginate(...):
        item: SearchGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [SearchGroupsPaginator](./paginators.md#searchgroupspaginator)
3. item: `AioPageIterator[SearchGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    Namespace: str,
    Filters: Sequence[GroupSearchFilterTypeDef],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchGroupsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[GroupSearchFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchGroupsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchGroupsRequestPaginateTypeDef](./type_defs.md#searchgroupsrequestpaginatetypedef)
## SearchTopicsPaginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator("search_topics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/paginator/SearchTopics.html#QuickSight.Paginator.SearchTopics)

```python
# SearchTopicsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_quicksight.paginator import SearchTopicsPaginator

session = get_session()
async with session.create_client("quicksight") as client:  # (1)
    paginator: SearchTopicsPaginator = client.get_paginator("search_topics")  # (2)
    async for item in paginator.paginate(...):
        item: SearchTopicsResponseTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [SearchTopicsPaginator](./paginators.md#searchtopicspaginator)
3. item: `AioPageIterator[SearchTopicsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchTopicsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[TopicSearchFilterTypeDef],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchTopicsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[TopicSearchFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchTopicsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchTopicsRequestPaginateTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchTopicsRequestPaginateTypeDef](./type_defs.md#searchtopicsrequestpaginatetypedef)
