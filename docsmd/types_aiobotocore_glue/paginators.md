# Paginators

> [Index](../README.md) > [Glue](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Glue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
    type annotations stubs module [types-aiobotocore-glue](https://pypi.org/project/types-aiobotocore-glue/).

## GetClassifiersPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_classifiers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetClassifiers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetClassifiersPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetClassifiersPaginator = client.get_paginator("get_classifiers")  # (2)
    async for item in paginator.paginate(...):
        item: GetClassifiersResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetClassifiersPaginator](./paginators.md#getclassifierspaginator)
3. item: [:material-code-braces: GetClassifiersResponseTypeDef](./type_defs.md#getclassifiersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetClassifiersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetClassifiersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetClassifiersResponseTypeDef](./type_defs.md#getclassifiersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetClassifiersRequestGetClassifiersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetClassifiersRequestGetClassifiersPaginateTypeDef](./type_defs.md#getclassifiersrequestgetclassifierspaginatetypedef) 
## GetConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetConnections)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetConnectionsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetConnectionsPaginator = client.get_paginator("get_connections")  # (2)
    async for item in paginator.paginate(...):
        item: GetConnectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetConnectionsPaginator](./paginators.md#getconnectionspaginator)
3. item: [:material-code-braces: GetConnectionsResponseTypeDef](./type_defs.md#getconnectionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetConnectionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CatalogId: str = ...,
    Filter: GetConnectionsFilterTypeDef = ...,  # (1)
    HidePassword: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetConnectionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: GetConnectionsFilterTypeDef](./type_defs.md#getconnectionsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetConnectionsResponseTypeDef](./type_defs.md#getconnectionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetConnectionsRequestGetConnectionsPaginateTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetConnectionsRequestGetConnectionsPaginateTypeDef](./type_defs.md#getconnectionsrequestgetconnectionspaginatetypedef) 
## GetCrawlerMetricsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_crawler_metrics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetCrawlerMetrics)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetCrawlerMetricsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetCrawlerMetricsPaginator = client.get_paginator("get_crawler_metrics")  # (2)
    async for item in paginator.paginate(...):
        item: GetCrawlerMetricsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetCrawlerMetricsPaginator](./paginators.md#getcrawlermetricspaginator)
3. item: [:material-code-braces: GetCrawlerMetricsResponseTypeDef](./type_defs.md#getcrawlermetricsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetCrawlerMetricsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CrawlerNameList: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetCrawlerMetricsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetCrawlerMetricsResponseTypeDef](./type_defs.md#getcrawlermetricsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef = {  # (1)
    "CrawlerNameList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef](./type_defs.md#getcrawlermetricsrequestgetcrawlermetricspaginatetypedef) 
## GetCrawlersPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_crawlers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetCrawlers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetCrawlersPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetCrawlersPaginator = client.get_paginator("get_crawlers")  # (2)
    async for item in paginator.paginate(...):
        item: GetCrawlersResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetCrawlersPaginator](./paginators.md#getcrawlerspaginator)
3. item: [:material-code-braces: GetCrawlersResponseTypeDef](./type_defs.md#getcrawlersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetCrawlersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetCrawlersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetCrawlersResponseTypeDef](./type_defs.md#getcrawlersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetCrawlersRequestGetCrawlersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCrawlersRequestGetCrawlersPaginateTypeDef](./type_defs.md#getcrawlersrequestgetcrawlerspaginatetypedef) 
## GetDatabasesPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_databases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetDatabases)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetDatabasesPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetDatabasesPaginator = client.get_paginator("get_databases")  # (2)
    async for item in paginator.paginate(...):
        item: GetDatabasesResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetDatabasesPaginator](./paginators.md#getdatabasespaginator)
3. item: [:material-code-braces: GetDatabasesResponseTypeDef](./type_defs.md#getdatabasesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetDatabasesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CatalogId: str = ...,
    ResourceShareType: ResourceShareTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetDatabasesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetDatabasesResponseTypeDef](./type_defs.md#getdatabasesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetDatabasesRequestGetDatabasesPaginateTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDatabasesRequestGetDatabasesPaginateTypeDef](./type_defs.md#getdatabasesrequestgetdatabasespaginatetypedef) 
## GetDevEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_dev_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetDevEndpoints)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetDevEndpointsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetDevEndpointsPaginator = client.get_paginator("get_dev_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: GetDevEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetDevEndpointsPaginator](./paginators.md#getdevendpointspaginator)
3. item: [:material-code-braces: GetDevEndpointsResponseTypeDef](./type_defs.md#getdevendpointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetDevEndpointsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetDevEndpointsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetDevEndpointsResponseTypeDef](./type_defs.md#getdevendpointsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef](./type_defs.md#getdevendpointsrequestgetdevendpointspaginatetypedef) 
## GetJobRunsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_job_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetJobRuns)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetJobRunsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetJobRunsPaginator = client.get_paginator("get_job_runs")  # (2)
    async for item in paginator.paginate(...):
        item: GetJobRunsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetJobRunsPaginator](./paginators.md#getjobrunspaginator)
3. item: [:material-code-braces: GetJobRunsResponseTypeDef](./type_defs.md#getjobrunsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetJobRunsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    JobName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetJobRunsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetJobRunsResponseTypeDef](./type_defs.md#getjobrunsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetJobRunsRequestGetJobRunsPaginateTypeDef = {  # (1)
    "JobName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetJobRunsRequestGetJobRunsPaginateTypeDef](./type_defs.md#getjobrunsrequestgetjobrunspaginatetypedef) 
## GetJobsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetJobsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetJobsPaginator = client.get_paginator("get_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: GetJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetJobsPaginator](./paginators.md#getjobspaginator)
3. item: [:material-code-braces: GetJobsResponseTypeDef](./type_defs.md#getjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetJobsResponseTypeDef](./type_defs.md#getjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetJobsRequestGetJobsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetJobsRequestGetJobsPaginateTypeDef](./type_defs.md#getjobsrequestgetjobspaginatetypedef) 
## GetPartitionIndexesPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_partition_indexes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetPartitionIndexes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetPartitionIndexesPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetPartitionIndexesPaginator = client.get_paginator("get_partition_indexes")  # (2)
    async for item in paginator.paginate(...):
        item: GetPartitionIndexesResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetPartitionIndexesPaginator](./paginators.md#getpartitionindexespaginator)
3. item: [:material-code-braces: GetPartitionIndexesResponseTypeDef](./type_defs.md#getpartitionindexesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetPartitionIndexesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    CatalogId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetPartitionIndexesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetPartitionIndexesResponseTypeDef](./type_defs.md#getpartitionindexesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef](./type_defs.md#getpartitionindexesrequestgetpartitionindexespaginatetypedef) 
## GetPartitionsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_partitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetPartitions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetPartitionsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetPartitionsPaginator = client.get_paginator("get_partitions")  # (2)
    async for item in paginator.paginate(...):
        item: GetPartitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetPartitionsPaginator](./paginators.md#getpartitionspaginator)
3. item: [:material-code-braces: GetPartitionsResponseTypeDef](./type_defs.md#getpartitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetPartitionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    CatalogId: str = ...,
    Expression: str = ...,
    Segment: SegmentTypeDef = ...,  # (1)
    ExcludeColumnSchema: bool = ...,
    TransactionId: str = ...,
    QueryAsOfTime: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetPartitionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetPartitionsResponseTypeDef](./type_defs.md#getpartitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetPartitionsRequestGetPartitionsPaginateTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetPartitionsRequestGetPartitionsPaginateTypeDef](./type_defs.md#getpartitionsrequestgetpartitionspaginatetypedef) 
## GetResourcePoliciesPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_resource_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetResourcePolicies)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetResourcePoliciesPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetResourcePoliciesPaginator = client.get_paginator("get_resource_policies")  # (2)
    async for item in paginator.paginate(...):
        item: GetResourcePoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetResourcePoliciesPaginator](./paginators.md#getresourcepoliciespaginator)
3. item: [:material-code-braces: GetResourcePoliciesResponseTypeDef](./type_defs.md#getresourcepoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetResourcePoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetResourcePoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetResourcePoliciesResponseTypeDef](./type_defs.md#getresourcepoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef](./type_defs.md#getresourcepoliciesrequestgetresourcepoliciespaginatetypedef) 
## GetSecurityConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_security_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetSecurityConfigurations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetSecurityConfigurationsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetSecurityConfigurationsPaginator = client.get_paginator("get_security_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: GetSecurityConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetSecurityConfigurationsPaginator](./paginators.md#getsecurityconfigurationspaginator)
3. item: [:material-code-braces: GetSecurityConfigurationsResponseTypeDef](./type_defs.md#getsecurityconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetSecurityConfigurationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetSecurityConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetSecurityConfigurationsResponseTypeDef](./type_defs.md#getsecurityconfigurationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef](./type_defs.md#getsecurityconfigurationsrequestgetsecurityconfigurationspaginatetypedef) 
## GetTableVersionsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_table_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTableVersions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetTableVersionsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetTableVersionsPaginator = client.get_paginator("get_table_versions")  # (2)
    async for item in paginator.paginate(...):
        item: GetTableVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetTableVersionsPaginator](./paginators.md#gettableversionspaginator)
3. item: [:material-code-braces: GetTableVersionsResponseTypeDef](./type_defs.md#gettableversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetTableVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    CatalogId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetTableVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetTableVersionsResponseTypeDef](./type_defs.md#gettableversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetTableVersionsRequestGetTableVersionsPaginateTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTableVersionsRequestGetTableVersionsPaginateTypeDef](./type_defs.md#gettableversionsrequestgettableversionspaginatetypedef) 
## GetTablesPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTables)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetTablesPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetTablesPaginator = client.get_paginator("get_tables")  # (2)
    async for item in paginator.paginate(...):
        item: GetTablesResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetTablesPaginator](./paginators.md#gettablespaginator)
3. item: [:material-code-braces: GetTablesResponseTypeDef](./type_defs.md#gettablesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetTablesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DatabaseName: str,
    CatalogId: str = ...,
    Expression: str = ...,
    TransactionId: str = ...,
    QueryAsOfTime: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetTablesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetTablesResponseTypeDef](./type_defs.md#gettablesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetTablesRequestGetTablesPaginateTypeDef = {  # (1)
    "DatabaseName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTablesRequestGetTablesPaginateTypeDef](./type_defs.md#gettablesrequestgettablespaginatetypedef) 
## GetTriggersPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_triggers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTriggers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetTriggersPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetTriggersPaginator = client.get_paginator("get_triggers")  # (2)
    async for item in paginator.paginate(...):
        item: GetTriggersResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetTriggersPaginator](./paginators.md#gettriggerspaginator)
3. item: [:material-code-braces: GetTriggersResponseTypeDef](./type_defs.md#gettriggersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetTriggersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DependentJobName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetTriggersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetTriggersResponseTypeDef](./type_defs.md#gettriggersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetTriggersRequestGetTriggersPaginateTypeDef = {  # (1)
    "DependentJobName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTriggersRequestGetTriggersPaginateTypeDef](./type_defs.md#gettriggersrequestgettriggerspaginatetypedef) 
## GetUserDefinedFunctionsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_user_defined_functions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetUserDefinedFunctions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetUserDefinedFunctionsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetUserDefinedFunctionsPaginator = client.get_paginator("get_user_defined_functions")  # (2)
    async for item in paginator.paginate(...):
        item: GetUserDefinedFunctionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetUserDefinedFunctionsPaginator](./paginators.md#getuserdefinedfunctionspaginator)
3. item: [:material-code-braces: GetUserDefinedFunctionsResponseTypeDef](./type_defs.md#getuserdefinedfunctionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetUserDefinedFunctionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Pattern: str,
    CatalogId: str = ...,
    DatabaseName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetUserDefinedFunctionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetUserDefinedFunctionsResponseTypeDef](./type_defs.md#getuserdefinedfunctionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef = {  # (1)
    "Pattern": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef](./type_defs.md#getuserdefinedfunctionsrequestgetuserdefinedfunctionspaginatetypedef) 
## ListRegistriesPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_registries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListRegistries)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListRegistriesPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: ListRegistriesPaginator = client.get_paginator("list_registries")  # (2)
    async for item in paginator.paginate(...):
        item: ListRegistriesResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [ListRegistriesPaginator](./paginators.md#listregistriespaginator)
3. item: [:material-code-braces: ListRegistriesResponseTypeDef](./type_defs.md#listregistriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRegistriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRegistriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRegistriesResponseTypeDef](./type_defs.md#listregistriesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRegistriesInputListRegistriesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRegistriesInputListRegistriesPaginateTypeDef](./type_defs.md#listregistriesinputlistregistriespaginatetypedef) 
## ListSchemaVersionsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_schema_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListSchemaVersions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListSchemaVersionsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: ListSchemaVersionsPaginator = client.get_paginator("list_schema_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemaVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [ListSchemaVersionsPaginator](./paginators.md#listschemaversionspaginator)
3. item: [:material-code-braces: ListSchemaVersionsResponseTypeDef](./type_defs.md#listschemaversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSchemaVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SchemaId: SchemaIdTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListSchemaVersionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSchemaVersionsResponseTypeDef](./type_defs.md#listschemaversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef = {  # (1)
    "SchemaId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef](./type_defs.md#listschemaversionsinputlistschemaversionspaginatetypedef) 
## ListSchemasPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListSchemas)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListSchemasPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: ListSchemasPaginator = client.get_paginator("list_schemas")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemasResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [ListSchemasPaginator](./paginators.md#listschemaspaginator)
3. item: [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSchemasPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RegistryId: RegistryIdTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListSchemasResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSchemasInputListSchemasPaginateTypeDef = {  # (1)
    "RegistryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemasInputListSchemasPaginateTypeDef](./type_defs.md#listschemasinputlistschemaspaginatetypedef) 
