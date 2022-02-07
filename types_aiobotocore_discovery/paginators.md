<a id="paginators-for-aiobotocore-applicationdiscoveryservice-module"></a>

# Paginators for aiobotocore ApplicationDiscoveryService module

> [Index](..) > [ApplicationDiscoveryService](.) > Paginators

Auto-generated documentation for
[ApplicationDiscoveryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
type annotations stubs module
[types-aiobotocore-discovery](https://pypi.org/project/types-aiobotocore-discovery/).

- [Paginators for aiobotocore ApplicationDiscoveryService module](#paginators-for-aiobotocore-applicationdiscoveryservice-module)
  - [DescribeAgentsPaginator](#describeagentspaginator)
  - [DescribeContinuousExportsPaginator](#describecontinuousexportspaginator)
  - [DescribeExportConfigurationsPaginator](#describeexportconfigurationspaginator)
  - [DescribeExportTasksPaginator](#describeexporttaskspaginator)
  - [DescribeTagsPaginator](#describetagspaginator)
  - [ListConfigurationsPaginator](#listconfigurationspaginator)

<a id="describeagentspaginator"></a>

## DescribeAgentsPaginator

Type annotations for
`session.create_client("discovery").get_paginator("describe_agents")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_discovery.paginator import DescribeAgentsPaginator

session = get_session()
async with session.create_client("discovery") as client:
    client: ApplicationDiscoveryServiceClient
    paginator: DescribeAgentsPaginator = client.get_paginator("describe_agents")
```

Boto3 documentation:
[ApplicationDiscoveryService.Paginator.DescribeAgents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeAgents)

Arguments for `DescribeAgentsPaginator.paginate` method:

- `agentIds`: `Sequence`\[`str`\]
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeAgentsPaginator.paginate` returns
`_PageIterator`\[[DescribeAgentsResponseTypeDef](./type_defs.md#describeagentsresponsetypedef)\].

<a id="describecontinuousexportspaginator"></a>

## DescribeContinuousExportsPaginator

Type annotations for
`session.create_client("discovery").get_paginator("describe_continuous_exports")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_discovery.paginator import DescribeContinuousExportsPaginator

session = get_session()
async with session.create_client("discovery") as client:
    client: ApplicationDiscoveryServiceClient
    paginator: DescribeContinuousExportsPaginator = client.get_paginator("describe_continuous_exports")
```

Boto3 documentation:
[ApplicationDiscoveryService.Paginator.DescribeContinuousExports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeContinuousExports)

Arguments for `DescribeContinuousExportsPaginator.paginate` method:

- `exportIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeContinuousExportsPaginator.paginate` returns
`_PageIterator`\[[DescribeContinuousExportsResponseTypeDef](./type_defs.md#describecontinuousexportsresponsetypedef)\].

<a id="describeexportconfigurationspaginator"></a>

## DescribeExportConfigurationsPaginator

Type annotations for
`session.create_client("discovery").get_paginator("describe_export_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_discovery.paginator import DescribeExportConfigurationsPaginator

session = get_session()
async with session.create_client("discovery") as client:
    client: ApplicationDiscoveryServiceClient
    paginator: DescribeExportConfigurationsPaginator = client.get_paginator("describe_export_configurations")
```

Boto3 documentation:
[ApplicationDiscoveryService.Paginator.DescribeExportConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportConfigurations)

Arguments for `DescribeExportConfigurationsPaginator.paginate` method:

- `exportIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeExportConfigurationsPaginator.paginate` returns
`_PageIterator`\[[DescribeExportConfigurationsResponseTypeDef](./type_defs.md#describeexportconfigurationsresponsetypedef)\].

<a id="describeexporttaskspaginator"></a>

## DescribeExportTasksPaginator

Type annotations for
`session.create_client("discovery").get_paginator("describe_export_tasks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_discovery.paginator import DescribeExportTasksPaginator

session = get_session()
async with session.create_client("discovery") as client:
    client: ApplicationDiscoveryServiceClient
    paginator: DescribeExportTasksPaginator = client.get_paginator("describe_export_tasks")
```

Boto3 documentation:
[ApplicationDiscoveryService.Paginator.DescribeExportTasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportTasks)

Arguments for `DescribeExportTasksPaginator.paginate` method:

- `exportIds`: `Sequence`\[`str`\]
- `filters`:
  `Sequence`\[[ExportFilterTypeDef](./type_defs.md#exportfiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeExportTasksPaginator.paginate` returns
`_PageIterator`\[[DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef)\].

<a id="describetagspaginator"></a>

## DescribeTagsPaginator

Type annotations for
`session.create_client("discovery").get_paginator("describe_tags")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_discovery.paginator import DescribeTagsPaginator

session = get_session()
async with session.create_client("discovery") as client:
    client: ApplicationDiscoveryServiceClient
    paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
```

Boto3 documentation:
[ApplicationDiscoveryService.Paginator.DescribeTags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeTags)

Arguments for `DescribeTagsPaginator.paginate` method:

- `filters`: `Sequence`\[[TagFilterTypeDef](./type_defs.md#tagfiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeTagsPaginator.paginate` returns
`_PageIterator`\[[DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef)\].

<a id="listconfigurationspaginator"></a>

## ListConfigurationsPaginator

Type annotations for
`session.create_client("discovery").get_paginator("list_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_discovery.paginator import ListConfigurationsPaginator

session = get_session()
async with session.create_client("discovery") as client:
    client: ApplicationDiscoveryServiceClient
    paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
```

Boto3 documentation:
[ApplicationDiscoveryService.Paginator.ListConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.ListConfigurations)

Arguments for `ListConfigurationsPaginator.paginate` method:

- `configurationType`:
  [ConfigurationItemTypeType](./literals.md#configurationitemtypetype)
  *(required)*
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `orderBy`:
  `Sequence`\[[OrderByElementTypeDef](./type_defs.md#orderbyelementtypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListConfigurationsPaginator.paginate` returns
`_PageIterator`\[[ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef)\].
