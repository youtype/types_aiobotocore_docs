<a id="paginators-for-aiobotocore-glue-module"></a>

# Paginators for aiobotocore Glue module

> [Index](..) > [Glue](.) > Paginators

Auto-generated documentation for
[Glue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
type annotations stubs module
[types-aiobotocore-glue](https://pypi.org/project/types-aiobotocore-glue/).

- [Paginators for aiobotocore Glue module](#paginators-for-aiobotocore-glue-module)
  - [GetClassifiersPaginator](#getclassifierspaginator)
  - [GetConnectionsPaginator](#getconnectionspaginator)
  - [GetCrawlerMetricsPaginator](#getcrawlermetricspaginator)
  - [GetCrawlersPaginator](#getcrawlerspaginator)
  - [GetDatabasesPaginator](#getdatabasespaginator)
  - [GetDevEndpointsPaginator](#getdevendpointspaginator)
  - [GetJobRunsPaginator](#getjobrunspaginator)
  - [GetJobsPaginator](#getjobspaginator)
  - [GetPartitionIndexesPaginator](#getpartitionindexespaginator)
  - [GetPartitionsPaginator](#getpartitionspaginator)
  - [GetResourcePoliciesPaginator](#getresourcepoliciespaginator)
  - [GetSecurityConfigurationsPaginator](#getsecurityconfigurationspaginator)
  - [GetTableVersionsPaginator](#gettableversionspaginator)
  - [GetTablesPaginator](#gettablespaginator)
  - [GetTriggersPaginator](#gettriggerspaginator)
  - [GetUserDefinedFunctionsPaginator](#getuserdefinedfunctionspaginator)
  - [ListRegistriesPaginator](#listregistriespaginator)
  - [ListSchemaVersionsPaginator](#listschemaversionspaginator)
  - [ListSchemasPaginator](#listschemaspaginator)

<a id="getclassifierspaginator"></a>

## GetClassifiersPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_classifiers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetClassifiersPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetClassifiersPaginator = client.get_paginator("get_classifiers")
```

Boto3 documentation:
[Glue.Paginator.GetClassifiers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetClassifiers)

Arguments for `GetClassifiersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetClassifiersPaginator.paginate` returns
`_PageIterator`\[[GetClassifiersResponseTypeDef](./type_defs.md#getclassifiersresponsetypedef)\].

<a id="getconnectionspaginator"></a>

## GetConnectionsPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_connections")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetConnectionsPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetConnectionsPaginator = client.get_paginator("get_connections")
```

Boto3 documentation:
[Glue.Paginator.GetConnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetConnections)

Arguments for `GetConnectionsPaginator.paginate` method:

- `CatalogId`: `str`
- `Filter`:
  [GetConnectionsFilterTypeDef](./type_defs.md#getconnectionsfiltertypedef)
- `HidePassword`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetConnectionsPaginator.paginate` returns
`_PageIterator`\[[GetConnectionsResponseTypeDef](./type_defs.md#getconnectionsresponsetypedef)\].

<a id="getcrawlermetricspaginator"></a>

## GetCrawlerMetricsPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_crawler_metrics")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetCrawlerMetricsPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetCrawlerMetricsPaginator = client.get_paginator("get_crawler_metrics")
```

Boto3 documentation:
[Glue.Paginator.GetCrawlerMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetCrawlerMetrics)

Arguments for `GetCrawlerMetricsPaginator.paginate` method:

- `CrawlerNameList`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetCrawlerMetricsPaginator.paginate` returns
`_PageIterator`\[[GetCrawlerMetricsResponseTypeDef](./type_defs.md#getcrawlermetricsresponsetypedef)\].

<a id="getcrawlerspaginator"></a>

## GetCrawlersPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_crawlers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetCrawlersPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetCrawlersPaginator = client.get_paginator("get_crawlers")
```

Boto3 documentation:
[Glue.Paginator.GetCrawlers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetCrawlers)

Arguments for `GetCrawlersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetCrawlersPaginator.paginate` returns
`_PageIterator`\[[GetCrawlersResponseTypeDef](./type_defs.md#getcrawlersresponsetypedef)\].

<a id="getdatabasespaginator"></a>

## GetDatabasesPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_databases")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetDatabasesPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetDatabasesPaginator = client.get_paginator("get_databases")
```

Boto3 documentation:
[Glue.Paginator.GetDatabases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetDatabases)

Arguments for `GetDatabasesPaginator.paginate` method:

- `CatalogId`: `str`
- `ResourceShareType`:
  [ResourceShareTypeType](./literals.md#resourcesharetypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDatabasesPaginator.paginate` returns
`_PageIterator`\[[GetDatabasesResponseTypeDef](./type_defs.md#getdatabasesresponsetypedef)\].

<a id="getdevendpointspaginator"></a>

## GetDevEndpointsPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_dev_endpoints")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetDevEndpointsPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetDevEndpointsPaginator = client.get_paginator("get_dev_endpoints")
```

Boto3 documentation:
[Glue.Paginator.GetDevEndpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetDevEndpoints)

Arguments for `GetDevEndpointsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDevEndpointsPaginator.paginate` returns
`_PageIterator`\[[GetDevEndpointsResponseTypeDef](./type_defs.md#getdevendpointsresponsetypedef)\].

<a id="getjobrunspaginator"></a>

## GetJobRunsPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_job_runs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetJobRunsPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetJobRunsPaginator = client.get_paginator("get_job_runs")
```

Boto3 documentation:
[Glue.Paginator.GetJobRuns](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetJobRuns)

Arguments for `GetJobRunsPaginator.paginate` method:

- `JobName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetJobRunsPaginator.paginate` returns
`_PageIterator`\[[GetJobRunsResponseTypeDef](./type_defs.md#getjobrunsresponsetypedef)\].

<a id="getjobspaginator"></a>

## GetJobsPaginator

Type annotations for `session.create_client("glue").get_paginator("get_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetJobsPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetJobsPaginator = client.get_paginator("get_jobs")
```

Boto3 documentation:
[Glue.Paginator.GetJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetJobs)

Arguments for `GetJobsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetJobsPaginator.paginate` returns
`_PageIterator`\[[GetJobsResponseTypeDef](./type_defs.md#getjobsresponsetypedef)\].

<a id="getpartitionindexespaginator"></a>

## GetPartitionIndexesPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_partition_indexes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetPartitionIndexesPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetPartitionIndexesPaginator = client.get_paginator("get_partition_indexes")
```

Boto3 documentation:
[Glue.Paginator.GetPartitionIndexes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetPartitionIndexes)

Arguments for `GetPartitionIndexesPaginator.paginate` method:

- `DatabaseName`: `str` *(required)*
- `TableName`: `str` *(required)*
- `CatalogId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetPartitionIndexesPaginator.paginate` returns
`_PageIterator`\[[GetPartitionIndexesResponseTypeDef](./type_defs.md#getpartitionindexesresponsetypedef)\].

<a id="getpartitionspaginator"></a>

## GetPartitionsPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_partitions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetPartitionsPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetPartitionsPaginator = client.get_paginator("get_partitions")
```

Boto3 documentation:
[Glue.Paginator.GetPartitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetPartitions)

Arguments for `GetPartitionsPaginator.paginate` method:

- `DatabaseName`: `str` *(required)*
- `TableName`: `str` *(required)*
- `CatalogId`: `str`
- `Expression`: `str`
- `Segment`: [SegmentTypeDef](./type_defs.md#segmenttypedef)
- `ExcludeColumnSchema`: `bool`
- `TransactionId`: `str`
- `QueryAsOfTime`: `Union`\[`datetime`, `str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetPartitionsPaginator.paginate` returns
`_PageIterator`\[[GetPartitionsResponseTypeDef](./type_defs.md#getpartitionsresponsetypedef)\].

<a id="getresourcepoliciespaginator"></a>

## GetResourcePoliciesPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_resource_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetResourcePoliciesPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetResourcePoliciesPaginator = client.get_paginator("get_resource_policies")
```

Boto3 documentation:
[Glue.Paginator.GetResourcePolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetResourcePolicies)

Arguments for `GetResourcePoliciesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetResourcePoliciesPaginator.paginate` returns
`_PageIterator`\[[GetResourcePoliciesResponseTypeDef](./type_defs.md#getresourcepoliciesresponsetypedef)\].

<a id="getsecurityconfigurationspaginator"></a>

## GetSecurityConfigurationsPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_security_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetSecurityConfigurationsPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetSecurityConfigurationsPaginator = client.get_paginator("get_security_configurations")
```

Boto3 documentation:
[Glue.Paginator.GetSecurityConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetSecurityConfigurations)

Arguments for `GetSecurityConfigurationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetSecurityConfigurationsPaginator.paginate` returns
`_PageIterator`\[[GetSecurityConfigurationsResponseTypeDef](./type_defs.md#getsecurityconfigurationsresponsetypedef)\].

<a id="gettableversionspaginator"></a>

## GetTableVersionsPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_table_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetTableVersionsPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetTableVersionsPaginator = client.get_paginator("get_table_versions")
```

Boto3 documentation:
[Glue.Paginator.GetTableVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTableVersions)

Arguments for `GetTableVersionsPaginator.paginate` method:

- `DatabaseName`: `str` *(required)*
- `TableName`: `str` *(required)*
- `CatalogId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetTableVersionsPaginator.paginate` returns
`_PageIterator`\[[GetTableVersionsResponseTypeDef](./type_defs.md#gettableversionsresponsetypedef)\].

<a id="gettablespaginator"></a>

## GetTablesPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_tables")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetTablesPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetTablesPaginator = client.get_paginator("get_tables")
```

Boto3 documentation:
[Glue.Paginator.GetTables](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTables)

Arguments for `GetTablesPaginator.paginate` method:

- `DatabaseName`: `str` *(required)*
- `CatalogId`: `str`
- `Expression`: `str`
- `TransactionId`: `str`
- `QueryAsOfTime`: `Union`\[`datetime`, `str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetTablesPaginator.paginate` returns
`_PageIterator`\[[GetTablesResponseTypeDef](./type_defs.md#gettablesresponsetypedef)\].

<a id="gettriggerspaginator"></a>

## GetTriggersPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_triggers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetTriggersPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetTriggersPaginator = client.get_paginator("get_triggers")
```

Boto3 documentation:
[Glue.Paginator.GetTriggers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTriggers)

Arguments for `GetTriggersPaginator.paginate` method:

- `DependentJobName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetTriggersPaginator.paginate` returns
`_PageIterator`\[[GetTriggersResponseTypeDef](./type_defs.md#gettriggersresponsetypedef)\].

<a id="getuserdefinedfunctionspaginator"></a>

## GetUserDefinedFunctionsPaginator

Type annotations for
`session.create_client("glue").get_paginator("get_user_defined_functions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetUserDefinedFunctionsPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: GetUserDefinedFunctionsPaginator = client.get_paginator("get_user_defined_functions")
```

Boto3 documentation:
[Glue.Paginator.GetUserDefinedFunctions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetUserDefinedFunctions)

Arguments for `GetUserDefinedFunctionsPaginator.paginate` method:

- `Pattern`: `str` *(required)*
- `CatalogId`: `str`
- `DatabaseName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetUserDefinedFunctionsPaginator.paginate` returns
`_PageIterator`\[[GetUserDefinedFunctionsResponseTypeDef](./type_defs.md#getuserdefinedfunctionsresponsetypedef)\].

<a id="listregistriespaginator"></a>

## ListRegistriesPaginator

Type annotations for
`session.create_client("glue").get_paginator("list_registries")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListRegistriesPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: ListRegistriesPaginator = client.get_paginator("list_registries")
```

Boto3 documentation:
[Glue.Paginator.ListRegistries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListRegistries)

Arguments for `ListRegistriesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRegistriesPaginator.paginate` returns
`_PageIterator`\[[ListRegistriesResponseTypeDef](./type_defs.md#listregistriesresponsetypedef)\].

<a id="listschemaversionspaginator"></a>

## ListSchemaVersionsPaginator

Type annotations for
`session.create_client("glue").get_paginator("list_schema_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListSchemaVersionsPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: ListSchemaVersionsPaginator = client.get_paginator("list_schema_versions")
```

Boto3 documentation:
[Glue.Paginator.ListSchemaVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListSchemaVersions)

Arguments for `ListSchemaVersionsPaginator.paginate` method:

- `SchemaId`: [SchemaIdTypeDef](./type_defs.md#schemaidtypedef) *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSchemaVersionsPaginator.paginate` returns
`_PageIterator`\[[ListSchemaVersionsResponseTypeDef](./type_defs.md#listschemaversionsresponsetypedef)\].

<a id="listschemaspaginator"></a>

## ListSchemasPaginator

Type annotations for
`session.create_client("glue").get_paginator("list_schemas")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListSchemasPaginator

session = get_session()
async with session.create_client("glue") as client:
    client: GlueClient
    paginator: ListSchemasPaginator = client.get_paginator("list_schemas")
```

Boto3 documentation:
[Glue.Paginator.ListSchemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListSchemas)

Arguments for `ListSchemasPaginator.paginate` method:

- `RegistryId`: [RegistryIdTypeDef](./type_defs.md#registryidtypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSchemasPaginator.paginate` returns
`_PageIterator`\[[ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef)\].
