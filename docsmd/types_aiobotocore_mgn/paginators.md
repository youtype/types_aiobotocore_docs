# Paginators

> [Index](../README.md) > [Mgn](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Mgn](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
    type annotations stubs module [types-aiobotocore-mgn](https://pypi.org/project/types-aiobotocore-mgn/).

## DescribeJobLogItemsPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("describe_job_log_items")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/DescribeJobLogItems.html#Mgn.Paginator.DescribeJobLogItems)

```python
# DescribeJobLogItemsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import DescribeJobLogItemsPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeJobLogItemsResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
3. item: [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeJobLogItemsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    jobID: str,
    accountID: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeJobLogItemsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeJobLogItemsRequestPaginateTypeDef = {  # (1)
    "jobID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeJobLogItemsRequestPaginateTypeDef](./type_defs.md#describejoblogitemsrequestpaginatetypedef) 
## DescribeJobsPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("describe_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/DescribeJobs.html#Mgn.Paginator.DescribeJobs)

```python
# DescribeJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import DescribeJobsPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: DescribeJobsPaginator = client.get_paginator("describe_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [DescribeJobsPaginator](./paginators.md#describejobspaginator)
3. item: [:material-code-braces: DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accountID: str = ...,
    filters: DescribeJobsRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeJobsRequestPaginateTypeDef = {  # (1)
    "accountID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeJobsRequestPaginateTypeDef](./type_defs.md#describejobsrequestpaginatetypedef) 
## DescribeLaunchConfigurationTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("describe_launch_configuration_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/DescribeLaunchConfigurationTemplates.html#Mgn.Paginator.DescribeLaunchConfigurationTemplates)

```python
# DescribeLaunchConfigurationTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import DescribeLaunchConfigurationTemplatesPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: DescribeLaunchConfigurationTemplatesPaginator = client.get_paginator("describe_launch_configuration_templates")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLaunchConfigurationTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [DescribeLaunchConfigurationTemplatesPaginator](./paginators.md#describelaunchconfigurationtemplatespaginator)
3. item: [:material-code-braces: DescribeLaunchConfigurationTemplatesResponseTypeDef](./type_defs.md#describelaunchconfigurationtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLaunchConfigurationTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    launchConfigurationTemplateIDs: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeLaunchConfigurationTemplatesResponseTypeDef](./type_defs.md#describelaunchconfigurationtemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef = {  # (1)
    "launchConfigurationTemplateIDs": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef](./type_defs.md#describelaunchconfigurationtemplatesrequestpaginatetypedef) 
## DescribeReplicationConfigurationTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("describe_replication_configuration_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/DescribeReplicationConfigurationTemplates.html#Mgn.Paginator.DescribeReplicationConfigurationTemplates)

```python
# DescribeReplicationConfigurationTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import DescribeReplicationConfigurationTemplatesPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: DescribeReplicationConfigurationTemplatesPaginator = client.get_paginator("describe_replication_configuration_templates")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReplicationConfigurationTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [DescribeReplicationConfigurationTemplatesPaginator](./paginators.md#describereplicationconfigurationtemplatespaginator)
3. item: [:material-code-braces: DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReplicationConfigurationTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    replicationConfigurationTemplateIDs: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReplicationConfigurationTemplatesRequestPaginateTypeDef = {  # (1)
    "replicationConfigurationTemplateIDs": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationConfigurationTemplatesRequestPaginateTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequestpaginatetypedef) 
## DescribeSourceServersPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("describe_source_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/DescribeSourceServers.html#Mgn.Paginator.DescribeSourceServers)

```python
# DescribeSourceServersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import DescribeSourceServersPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSourceServersResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [DescribeSourceServersPaginator](./paginators.md#describesourceserverspaginator)
3. item: [:material-code-braces: DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSourceServersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accountID: str = ...,
    filters: DescribeSourceServersRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeSourceServersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSourceServersRequestPaginateTypeDef = {  # (1)
    "accountID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSourceServersRequestPaginateTypeDef](./type_defs.md#describesourceserversrequestpaginatetypedef) 
## DescribeVcenterClientsPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("describe_vcenter_clients")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/DescribeVcenterClients.html#Mgn.Paginator.DescribeVcenterClients)

```python
# DescribeVcenterClientsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import DescribeVcenterClientsPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: DescribeVcenterClientsPaginator = client.get_paginator("describe_vcenter_clients")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVcenterClientsResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [DescribeVcenterClientsPaginator](./paginators.md#describevcenterclientspaginator)
3. item: [:material-code-braces: DescribeVcenterClientsResponseTypeDef](./type_defs.md#describevcenterclientsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVcenterClientsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeVcenterClientsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeVcenterClientsResponseTypeDef](./type_defs.md#describevcenterclientsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVcenterClientsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVcenterClientsRequestPaginateTypeDef](./type_defs.md#describevcenterclientsrequestpaginatetypedef) 
## ListApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/ListApplications.html#Mgn.Paginator.ListApplications)

```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accountID: str = ...,
    filters: ListApplicationsRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListApplicationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListApplicationsRequestFiltersTypeDef](./type_defs.md#listapplicationsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationsRequestPaginateTypeDef = {  # (1)
    "accountID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestPaginateTypeDef](./type_defs.md#listapplicationsrequestpaginatetypedef) 
## ListConnectorsPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("list_connectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/ListConnectors.html#Mgn.Paginator.ListConnectors)

```python
# ListConnectorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import ListConnectorsPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: ListConnectorsPaginator = client.get_paginator("list_connectors")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectorsResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
3. item: [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConnectorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: ListConnectorsRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListConnectorsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListConnectorsRequestFiltersTypeDef](./type_defs.md#listconnectorsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConnectorsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectorsRequestPaginateTypeDef](./type_defs.md#listconnectorsrequestpaginatetypedef) 
## ListExportErrorsPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("list_export_errors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/ListExportErrors.html#Mgn.Paginator.ListExportErrors)

```python
# ListExportErrorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import ListExportErrorsPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: ListExportErrorsPaginator = client.get_paginator("list_export_errors")  # (2)
    async for item in paginator.paginate(...):
        item: ListExportErrorsResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [ListExportErrorsPaginator](./paginators.md#listexporterrorspaginator)
3. item: [:material-code-braces: ListExportErrorsResponseTypeDef](./type_defs.md#listexporterrorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListExportErrorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    exportID: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListExportErrorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListExportErrorsResponseTypeDef](./type_defs.md#listexporterrorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListExportErrorsRequestPaginateTypeDef = {  # (1)
    "exportID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExportErrorsRequestPaginateTypeDef](./type_defs.md#listexporterrorsrequestpaginatetypedef) 
## ListExportsPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("list_exports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/ListExports.html#Mgn.Paginator.ListExports)

```python
# ListExportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import ListExportsPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: ListExportsPaginator = client.get_paginator("list_exports")  # (2)
    async for item in paginator.paginate(...):
        item: ListExportsResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [ListExportsPaginator](./paginators.md#listexportspaginator)
3. item: [:material-code-braces: ListExportsResponseTypeDef](./type_defs.md#listexportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListExportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: ListExportsRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListExportsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListExportsRequestFiltersTypeDef](./type_defs.md#listexportsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListExportsResponseTypeDef](./type_defs.md#listexportsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListExportsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExportsRequestPaginateTypeDef](./type_defs.md#listexportsrequestpaginatetypedef) 
## ListImportErrorsPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("list_import_errors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/ListImportErrors.html#Mgn.Paginator.ListImportErrors)

```python
# ListImportErrorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import ListImportErrorsPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: ListImportErrorsPaginator = client.get_paginator("list_import_errors")  # (2)
    async for item in paginator.paginate(...):
        item: ListImportErrorsResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [ListImportErrorsPaginator](./paginators.md#listimporterrorspaginator)
3. item: [:material-code-braces: ListImportErrorsResponseTypeDef](./type_defs.md#listimporterrorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListImportErrorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    importID: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListImportErrorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListImportErrorsResponseTypeDef](./type_defs.md#listimporterrorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListImportErrorsRequestPaginateTypeDef = {  # (1)
    "importID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImportErrorsRequestPaginateTypeDef](./type_defs.md#listimporterrorsrequestpaginatetypedef) 
## ListImportsPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("list_imports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/ListImports.html#Mgn.Paginator.ListImports)

```python
# ListImportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import ListImportsPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: ListImportsPaginator = client.get_paginator("list_imports")  # (2)
    async for item in paginator.paginate(...):
        item: ListImportsResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [ListImportsPaginator](./paginators.md#listimportspaginator)
3. item: [:material-code-braces: ListImportsResponseTypeDef](./type_defs.md#listimportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListImportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: ListImportsRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListImportsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListImportsRequestFiltersTypeDef](./type_defs.md#listimportsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListImportsResponseTypeDef](./type_defs.md#listimportsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListImportsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImportsRequestPaginateTypeDef](./type_defs.md#listimportsrequestpaginatetypedef) 
## ListManagedAccountsPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("list_managed_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/ListManagedAccounts.html#Mgn.Paginator.ListManagedAccounts)

```python
# ListManagedAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import ListManagedAccountsPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: ListManagedAccountsPaginator = client.get_paginator("list_managed_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [ListManagedAccountsPaginator](./paginators.md#listmanagedaccountspaginator)
3. item: [:material-code-braces: ListManagedAccountsResponseTypeDef](./type_defs.md#listmanagedaccountsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListManagedAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListManagedAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListManagedAccountsResponseTypeDef](./type_defs.md#listmanagedaccountsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedAccountsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedAccountsRequestPaginateTypeDef](./type_defs.md#listmanagedaccountsrequestpaginatetypedef) 
## ListSourceServerActionsPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("list_source_server_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/ListSourceServerActions.html#Mgn.Paginator.ListSourceServerActions)

```python
# ListSourceServerActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import ListSourceServerActionsPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: ListSourceServerActionsPaginator = client.get_paginator("list_source_server_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSourceServerActionsResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [ListSourceServerActionsPaginator](./paginators.md#listsourceserveractionspaginator)
3. item: [:material-code-braces: ListSourceServerActionsResponseTypeDef](./type_defs.md#listsourceserveractionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSourceServerActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sourceServerID: str,
    accountID: str = ...,
    filters: SourceServerActionsRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSourceServerActionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SourceServerActionsRequestFiltersTypeDef](./type_defs.md#sourceserveractionsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSourceServerActionsResponseTypeDef](./type_defs.md#listsourceserveractionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSourceServerActionsRequestPaginateTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSourceServerActionsRequestPaginateTypeDef](./type_defs.md#listsourceserveractionsrequestpaginatetypedef) 
## ListTemplateActionsPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("list_template_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/ListTemplateActions.html#Mgn.Paginator.ListTemplateActions)

```python
# ListTemplateActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import ListTemplateActionsPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: ListTemplateActionsPaginator = client.get_paginator("list_template_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListTemplateActionsResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [ListTemplateActionsPaginator](./paginators.md#listtemplateactionspaginator)
3. item: [:material-code-braces: ListTemplateActionsResponseTypeDef](./type_defs.md#listtemplateactionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTemplateActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    launchConfigurationTemplateID: str,
    filters: TemplateActionsRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListTemplateActionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TemplateActionsRequestFiltersTypeDef](./type_defs.md#templateactionsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTemplateActionsResponseTypeDef](./type_defs.md#listtemplateactionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTemplateActionsRequestPaginateTypeDef = {  # (1)
    "launchConfigurationTemplateID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTemplateActionsRequestPaginateTypeDef](./type_defs.md#listtemplateactionsrequestpaginatetypedef) 
## ListWavesPaginator

Type annotations and code completion for `#!python session.create_client("mgn").get_paginator("list_waves")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn/paginator/ListWaves.html#Mgn.Paginator.ListWaves)

```python
# ListWavesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import ListWavesPaginator

session = get_session()
async with session.create_client("mgn") as client:  # (1)
    paginator: ListWavesPaginator = client.get_paginator("list_waves")  # (2)
    async for item in paginator.paginate(...):
        item: ListWavesResponseTypeDef
        print(item)  # (3)
```

1. client: [MgnClient](./client.md)
2. paginator: [ListWavesPaginator](./paginators.md#listwavespaginator)
3. item: [:material-code-braces: ListWavesResponseTypeDef](./type_defs.md#listwavesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWavesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accountID: str = ...,
    filters: ListWavesRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListWavesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListWavesRequestFiltersTypeDef](./type_defs.md#listwavesrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListWavesResponseTypeDef](./type_defs.md#listwavesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWavesRequestPaginateTypeDef = {  # (1)
    "accountID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWavesRequestPaginateTypeDef](./type_defs.md#listwavesrequestpaginatetypedef) 
