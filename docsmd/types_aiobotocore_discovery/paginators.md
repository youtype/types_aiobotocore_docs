# Paginators

> [Index](../README.md) > [ApplicationDiscoveryService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ApplicationDiscoveryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#applicationdiscoveryservice)
    type annotations stubs module [types-aiobotocore-discovery](https://pypi.org/project/types-aiobotocore-discovery/).

## DescribeAgentsPaginator

Type annotations and code completion for `#!python session.create_client("discovery").get_paginator("describe_agents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/paginator/DescribeAgents.html#ApplicationDiscoveryService.Paginator.DescribeAgents)

```python
# DescribeAgentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_discovery.paginator import DescribeAgentsPaginator

session = get_session()
async with session.create_client("discovery") as client:  # (1)
    paginator: DescribeAgentsPaginator = client.get_paginator("describe_agents")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAgentsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [DescribeAgentsPaginator](./paginators.md#describeagentspaginator)
3. item: [:material-code-braces: DescribeAgentsResponseTypeDef](./type_defs.md#describeagentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAgentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    agentIds: Sequence[str] = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeAgentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeAgentsResponseTypeDef](./type_defs.md#describeagentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAgentsRequestPaginateTypeDef = {  # (1)
    "agentIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAgentsRequestPaginateTypeDef](./type_defs.md#describeagentsrequestpaginatetypedef) 
## DescribeContinuousExportsPaginator

Type annotations and code completion for `#!python session.create_client("discovery").get_paginator("describe_continuous_exports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/paginator/DescribeContinuousExports.html#ApplicationDiscoveryService.Paginator.DescribeContinuousExports)

```python
# DescribeContinuousExportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_discovery.paginator import DescribeContinuousExportsPaginator

session = get_session()
async with session.create_client("discovery") as client:  # (1)
    paginator: DescribeContinuousExportsPaginator = client.get_paginator("describe_continuous_exports")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeContinuousExportsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [DescribeContinuousExportsPaginator](./paginators.md#describecontinuousexportspaginator)
3. item: [:material-code-braces: DescribeContinuousExportsResponseTypeDef](./type_defs.md#describecontinuousexportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeContinuousExportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    exportIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeContinuousExportsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeContinuousExportsResponseTypeDef](./type_defs.md#describecontinuousexportsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeContinuousExportsRequestPaginateTypeDef = {  # (1)
    "exportIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeContinuousExportsRequestPaginateTypeDef](./type_defs.md#describecontinuousexportsrequestpaginatetypedef) 
## DescribeExportConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("discovery").get_paginator("describe_export_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/paginator/DescribeExportConfigurations.html#ApplicationDiscoveryService.Paginator.DescribeExportConfigurations)

```python
# DescribeExportConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_discovery.paginator import DescribeExportConfigurationsPaginator

session = get_session()
async with session.create_client("discovery") as client:  # (1)
    paginator: DescribeExportConfigurationsPaginator = client.get_paginator("describe_export_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeExportConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [DescribeExportConfigurationsPaginator](./paginators.md#describeexportconfigurationspaginator)
3. item: [:material-code-braces: DescribeExportConfigurationsResponseTypeDef](./type_defs.md#describeexportconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeExportConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    exportIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeExportConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeExportConfigurationsResponseTypeDef](./type_defs.md#describeexportconfigurationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeExportConfigurationsRequestPaginateTypeDef = {  # (1)
    "exportIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeExportConfigurationsRequestPaginateTypeDef](./type_defs.md#describeexportconfigurationsrequestpaginatetypedef) 
## DescribeExportTasksPaginator

Type annotations and code completion for `#!python session.create_client("discovery").get_paginator("describe_export_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/paginator/DescribeExportTasks.html#ApplicationDiscoveryService.Paginator.DescribeExportTasks)

```python
# DescribeExportTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_discovery.paginator import DescribeExportTasksPaginator

session = get_session()
async with session.create_client("discovery") as client:  # (1)
    paginator: DescribeExportTasksPaginator = client.get_paginator("describe_export_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeExportTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [DescribeExportTasksPaginator](./paginators.md#describeexporttaskspaginator)
3. item: [:material-code-braces: DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeExportTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    exportIds: Sequence[str] = ...,
    filters: Sequence[ExportFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeExportTasksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ExportFilterTypeDef](./type_defs.md#exportfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeExportTasksRequestPaginateTypeDef = {  # (1)
    "exportIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeExportTasksRequestPaginateTypeDef](./type_defs.md#describeexporttasksrequestpaginatetypedef) 
## DescribeImportTasksPaginator

Type annotations and code completion for `#!python session.create_client("discovery").get_paginator("describe_import_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/paginator/DescribeImportTasks.html#ApplicationDiscoveryService.Paginator.DescribeImportTasks)

```python
# DescribeImportTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_discovery.paginator import DescribeImportTasksPaginator

session = get_session()
async with session.create_client("discovery") as client:  # (1)
    paginator: DescribeImportTasksPaginator = client.get_paginator("describe_import_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImportTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [DescribeImportTasksPaginator](./paginators.md#describeimporttaskspaginator)
3. item: [:material-code-braces: DescribeImportTasksResponseTypeDef](./type_defs.md#describeimporttasksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeImportTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[ImportTaskFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeImportTasksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ImportTaskFilterTypeDef](./type_defs.md#importtaskfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeImportTasksResponseTypeDef](./type_defs.md#describeimporttasksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeImportTasksRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImportTasksRequestPaginateTypeDef](./type_defs.md#describeimporttasksrequestpaginatetypedef) 
## DescribeTagsPaginator

Type annotations and code completion for `#!python session.create_client("discovery").get_paginator("describe_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/paginator/DescribeTags.html#ApplicationDiscoveryService.Paginator.DescribeTags)

```python
# DescribeTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_discovery.paginator import DescribeTagsPaginator

session = get_session()
async with session.create_client("discovery") as client:  # (1)
    paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [DescribeTagsPaginator](./paginators.md#describetagspaginator)
3. item: [:material-code-braces: DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[TagFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeTagsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTagsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTagsRequestPaginateTypeDef](./type_defs.md#describetagsrequestpaginatetypedef) 
## ListConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("discovery").get_paginator("list_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery/paginator/ListConfigurations.html#ApplicationDiscoveryService.Paginator.ListConfigurations)

```python
# ListConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_discovery.paginator import ListConfigurationsPaginator

session = get_session()
async with session.create_client("discovery") as client:  # (1)
    paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [ListConfigurationsPaginator](./paginators.md#listconfigurationspaginator)
3. item: [:material-code-braces: ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    configurationType: ConfigurationItemTypeType,  # (1)
    filters: Sequence[FilterTypeDef] = ...,  # (2)
    orderBy: Sequence[OrderByElementTypeDef] = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListConfigurationsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ConfigurationItemTypeType](./literals.md#configurationitemtypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: OrderByElementTypeDef](./type_defs.md#orderbyelementtypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConfigurationsRequestPaginateTypeDef = {  # (1)
    "configurationType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigurationsRequestPaginateTypeDef](./type_defs.md#listconfigurationsrequestpaginatetypedef) 
