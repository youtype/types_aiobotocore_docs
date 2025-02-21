# Paginators

> [Index](../README.md) > [Glue](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Glue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#glue)
    type annotations stubs module [types-aiobotocore-glue](https://pypi.org/project/types-aiobotocore-glue/).

## DescribeEntityPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("describe_entity")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/DescribeEntity.html#Glue.Paginator.DescribeEntity)

```python
# DescribeEntityPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import DescribeEntityPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: DescribeEntityPaginator = client.get_paginator("describe_entity")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEntityResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [DescribeEntityPaginator](./paginators.md#describeentitypaginator)
3. item: [:material-code-braces: DescribeEntityResponseTypeDef](./type_defs.md#describeentityresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEntityPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConnectionName: str,
    EntityName: str,
    CatalogId: str = ...,
    DataStoreApiVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeEntityResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeEntityResponseTypeDef](./type_defs.md#describeentityresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEntityRequestPaginateTypeDef = {  # (1)
    "ConnectionName": ...,
    "EntityName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEntityRequestPaginateTypeDef](./type_defs.md#describeentityrequestpaginatetypedef) 
## GetClassifiersPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_classifiers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetClassifiers.html#Glue.Paginator.GetClassifiers)

```python
# GetClassifiersPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetClassifiersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetClassifiersResponseTypeDef](./type_defs.md#getclassifiersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetClassifiersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetClassifiersRequestPaginateTypeDef](./type_defs.md#getclassifiersrequestpaginatetypedef) 
## GetConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetConnections.html#Glue.Paginator.GetConnections)

```python
# GetConnectionsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    CatalogId: str = ...,
    Filter: GetConnectionsFilterTypeDef = ...,  # (1)
    HidePassword: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetConnectionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: GetConnectionsFilterTypeDef](./type_defs.md#getconnectionsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetConnectionsResponseTypeDef](./type_defs.md#getconnectionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetConnectionsRequestPaginateTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetConnectionsRequestPaginateTypeDef](./type_defs.md#getconnectionsrequestpaginatetypedef) 
## GetCrawlerMetricsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_crawler_metrics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetCrawlerMetrics.html#Glue.Paginator.GetCrawlerMetrics)

```python
# GetCrawlerMetricsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    CrawlerNameList: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetCrawlerMetricsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetCrawlerMetricsResponseTypeDef](./type_defs.md#getcrawlermetricsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetCrawlerMetricsRequestPaginateTypeDef = {  # (1)
    "CrawlerNameList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCrawlerMetricsRequestPaginateTypeDef](./type_defs.md#getcrawlermetricsrequestpaginatetypedef) 
## GetCrawlersPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_crawlers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetCrawlers.html#Glue.Paginator.GetCrawlers)

```python
# GetCrawlersPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetCrawlersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetCrawlersResponseTypeDef](./type_defs.md#getcrawlersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetCrawlersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCrawlersRequestPaginateTypeDef](./type_defs.md#getcrawlersrequestpaginatetypedef) 
## GetDatabasesPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_databases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetDatabases.html#Glue.Paginator.GetDatabases)

```python
# GetDatabasesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    CatalogId: str = ...,
    ResourceShareType: ResourceShareTypeType = ...,  # (1)
    AttributesToGet: Sequence[DatabaseAttributesType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[GetDatabasesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
2. See [:material-code-brackets: DatabaseAttributesType](./literals.md#databaseattributestype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetDatabasesResponseTypeDef](./type_defs.md#getdatabasesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetDatabasesRequestPaginateTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDatabasesRequestPaginateTypeDef](./type_defs.md#getdatabasesrequestpaginatetypedef) 
## GetDevEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_dev_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetDevEndpoints.html#Glue.Paginator.GetDevEndpoints)

```python
# GetDevEndpointsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetDevEndpointsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetDevEndpointsResponseTypeDef](./type_defs.md#getdevendpointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetDevEndpointsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDevEndpointsRequestPaginateTypeDef](./type_defs.md#getdevendpointsrequestpaginatetypedef) 
## GetJobRunsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_job_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetJobRuns.html#Glue.Paginator.GetJobRuns)

```python
# GetJobRunsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    JobName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetJobRunsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetJobRunsResponseTypeDef](./type_defs.md#getjobrunsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetJobRunsRequestPaginateTypeDef = {  # (1)
    "JobName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetJobRunsRequestPaginateTypeDef](./type_defs.md#getjobrunsrequestpaginatetypedef) 
## GetJobsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetJobs.html#Glue.Paginator.GetJobs)

```python
# GetJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetJobsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetJobsPaginator = client.get_paginator("get_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: GetJobsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetJobsPaginator](./paginators.md#getjobspaginator)
3. item: [:material-code-braces: GetJobsResponsePaginatorTypeDef](./type_defs.md#getjobsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python GetJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetJobsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetJobsResponsePaginatorTypeDef](./type_defs.md#getjobsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetJobsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetJobsRequestPaginateTypeDef](./type_defs.md#getjobsrequestpaginatetypedef) 
## GetPartitionIndexesPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_partition_indexes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetPartitionIndexes.html#Glue.Paginator.GetPartitionIndexes)

```python
# GetPartitionIndexesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    CatalogId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetPartitionIndexesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetPartitionIndexesResponseTypeDef](./type_defs.md#getpartitionindexesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetPartitionIndexesRequestPaginateTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetPartitionIndexesRequestPaginateTypeDef](./type_defs.md#getpartitionindexesrequestpaginatetypedef) 
## GetPartitionsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_partitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetPartitions.html#Glue.Paginator.GetPartitions)

```python
# GetPartitionsPaginator usage example

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

```python
# paginate method definition

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
    QueryAsOfTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetPartitionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetPartitionsResponseTypeDef](./type_defs.md#getpartitionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetPartitionsRequestPaginateTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetPartitionsRequestPaginateTypeDef](./type_defs.md#getpartitionsrequestpaginatetypedef) 
## GetResourcePoliciesPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_resource_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetResourcePolicies.html#Glue.Paginator.GetResourcePolicies)

```python
# GetResourcePoliciesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetResourcePoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetResourcePoliciesResponseTypeDef](./type_defs.md#getresourcepoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetResourcePoliciesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourcePoliciesRequestPaginateTypeDef](./type_defs.md#getresourcepoliciesrequestpaginatetypedef) 
## GetSecurityConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_security_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetSecurityConfigurations.html#Glue.Paginator.GetSecurityConfigurations)

```python
# GetSecurityConfigurationsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetSecurityConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetSecurityConfigurationsResponseTypeDef](./type_defs.md#getsecurityconfigurationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetSecurityConfigurationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSecurityConfigurationsRequestPaginateTypeDef](./type_defs.md#getsecurityconfigurationsrequestpaginatetypedef) 
## GetTableVersionsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_table_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetTableVersions.html#Glue.Paginator.GetTableVersions)

```python
# GetTableVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetTableVersionsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetTableVersionsPaginator = client.get_paginator("get_table_versions")  # (2)
    async for item in paginator.paginate(...):
        item: GetTableVersionsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetTableVersionsPaginator](./paginators.md#gettableversionspaginator)
3. item: [:material-code-braces: GetTableVersionsResponsePaginatorTypeDef](./type_defs.md#gettableversionsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python GetTableVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    CatalogId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetTableVersionsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetTableVersionsResponsePaginatorTypeDef](./type_defs.md#gettableversionsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetTableVersionsRequestPaginateTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTableVersionsRequestPaginateTypeDef](./type_defs.md#gettableversionsrequestpaginatetypedef) 
## GetTablesPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetTables.html#Glue.Paginator.GetTables)

```python
# GetTablesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetTablesPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetTablesPaginator = client.get_paginator("get_tables")  # (2)
    async for item in paginator.paginate(...):
        item: GetTablesResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetTablesPaginator](./paginators.md#gettablespaginator)
3. item: [:material-code-braces: GetTablesResponsePaginatorTypeDef](./type_defs.md#gettablesresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python GetTablesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DatabaseName: str,
    CatalogId: str = ...,
    Expression: str = ...,
    TransactionId: str = ...,
    QueryAsOfTime: TimestampTypeDef = ...,
    IncludeStatusDetails: bool = ...,
    AttributesToGet: Sequence[TableAttributesType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetTablesResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TableAttributesType](./literals.md#tableattributestype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetTablesResponsePaginatorTypeDef](./type_defs.md#gettablesresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetTablesRequestPaginateTypeDef = {  # (1)
    "DatabaseName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTablesRequestPaginateTypeDef](./type_defs.md#gettablesrequestpaginatetypedef) 
## GetTriggersPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_triggers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetTriggers.html#Glue.Paginator.GetTriggers)

```python
# GetTriggersPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    DependentJobName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetTriggersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetTriggersResponseTypeDef](./type_defs.md#gettriggersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetTriggersRequestPaginateTypeDef = {  # (1)
    "DependentJobName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTriggersRequestPaginateTypeDef](./type_defs.md#gettriggersrequestpaginatetypedef) 
## GetUserDefinedFunctionsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_user_defined_functions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetUserDefinedFunctions.html#Glue.Paginator.GetUserDefinedFunctions)

```python
# GetUserDefinedFunctionsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    Pattern: str,
    CatalogId: str = ...,
    DatabaseName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetUserDefinedFunctionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetUserDefinedFunctionsResponseTypeDef](./type_defs.md#getuserdefinedfunctionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetUserDefinedFunctionsRequestPaginateTypeDef = {  # (1)
    "Pattern": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetUserDefinedFunctionsRequestPaginateTypeDef](./type_defs.md#getuserdefinedfunctionsrequestpaginatetypedef) 
## GetWorkflowRunsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("get_workflow_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/GetWorkflowRuns.html#Glue.Paginator.GetWorkflowRuns)

```python
# GetWorkflowRunsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import GetWorkflowRunsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: GetWorkflowRunsPaginator = client.get_paginator("get_workflow_runs")  # (2)
    async for item in paginator.paginate(...):
        item: GetWorkflowRunsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [GetWorkflowRunsPaginator](./paginators.md#getworkflowrunspaginator)
3. item: [:material-code-braces: GetWorkflowRunsResponseTypeDef](./type_defs.md#getworkflowrunsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetWorkflowRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Name: str,
    IncludeGraph: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetWorkflowRunsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetWorkflowRunsResponseTypeDef](./type_defs.md#getworkflowrunsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetWorkflowRunsRequestPaginateTypeDef = {  # (1)
    "Name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetWorkflowRunsRequestPaginateTypeDef](./type_defs.md#getworkflowrunsrequestpaginatetypedef) 
## ListBlueprintsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_blueprints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/ListBlueprints.html#Glue.Paginator.ListBlueprints)

```python
# ListBlueprintsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListBlueprintsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: ListBlueprintsPaginator = client.get_paginator("list_blueprints")  # (2)
    async for item in paginator.paginate(...):
        item: ListBlueprintsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [ListBlueprintsPaginator](./paginators.md#listblueprintspaginator)
3. item: [:material-code-braces: ListBlueprintsResponseTypeDef](./type_defs.md#listblueprintsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBlueprintsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Tags: Mapping[str, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListBlueprintsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBlueprintsResponseTypeDef](./type_defs.md#listblueprintsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBlueprintsRequestPaginateTypeDef = {  # (1)
    "Tags": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBlueprintsRequestPaginateTypeDef](./type_defs.md#listblueprintsrequestpaginatetypedef) 
## ListConnectionTypesPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_connection_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/ListConnectionTypes.html#Glue.Paginator.ListConnectionTypes)

```python
# ListConnectionTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListConnectionTypesPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: ListConnectionTypesPaginator = client.get_paginator("list_connection_types")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectionTypesResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [ListConnectionTypesPaginator](./paginators.md#listconnectiontypespaginator)
3. item: [:material-code-braces: ListConnectionTypesResponseTypeDef](./type_defs.md#listconnectiontypesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConnectionTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConnectionTypesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConnectionTypesResponseTypeDef](./type_defs.md#listconnectiontypesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConnectionTypesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectionTypesRequestPaginateTypeDef](./type_defs.md#listconnectiontypesrequestpaginatetypedef) 
## ListEntitiesPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_entities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/ListEntities.html#Glue.Paginator.ListEntities)

```python
# ListEntitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListEntitiesPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: ListEntitiesPaginator = client.get_paginator("list_entities")  # (2)
    async for item in paginator.paginate(...):
        item: ListEntitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [ListEntitiesPaginator](./paginators.md#listentitiespaginator)
3. item: [:material-code-braces: ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEntitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConnectionName: str = ...,
    CatalogId: str = ...,
    ParentEntityName: str = ...,
    DataStoreApiVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEntitiesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEntitiesRequestPaginateTypeDef = {  # (1)
    "ConnectionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntitiesRequestPaginateTypeDef](./type_defs.md#listentitiesrequestpaginatetypedef) 
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/ListJobs.html#Glue.Paginator.ListJobs)

```python
# ListJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Tags: Mapping[str, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsRequestPaginateTypeDef = {  # (1)
    "Tags": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestPaginateTypeDef](./type_defs.md#listjobsrequestpaginatetypedef) 
## ListRegistriesPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_registries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/ListRegistries.html#Glue.Paginator.ListRegistries)

```python
# ListRegistriesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRegistriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRegistriesResponseTypeDef](./type_defs.md#listregistriesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRegistriesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRegistriesInputPaginateTypeDef](./type_defs.md#listregistriesinputpaginatetypedef) 
## ListSchemaVersionsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_schema_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/ListSchemaVersions.html#Glue.Paginator.ListSchemaVersions)

```python
# ListSchemaVersionsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    SchemaId: SchemaIdTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSchemaVersionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSchemaVersionsResponseTypeDef](./type_defs.md#listschemaversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSchemaVersionsInputPaginateTypeDef = {  # (1)
    "SchemaId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemaVersionsInputPaginateTypeDef](./type_defs.md#listschemaversionsinputpaginatetypedef) 
## ListSchemasPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/ListSchemas.html#Glue.Paginator.ListSchemas)

```python
# ListSchemasPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    RegistryId: RegistryIdTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSchemasResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSchemasInputPaginateTypeDef = {  # (1)
    "RegistryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemasInputPaginateTypeDef](./type_defs.md#listschemasinputpaginatetypedef) 
## ListTableOptimizerRunsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_table_optimizer_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/ListTableOptimizerRuns.html#Glue.Paginator.ListTableOptimizerRuns)

```python
# ListTableOptimizerRunsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListTableOptimizerRunsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: ListTableOptimizerRunsPaginator = client.get_paginator("list_table_optimizer_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListTableOptimizerRunsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [ListTableOptimizerRunsPaginator](./paginators.md#listtableoptimizerrunspaginator)
3. item: [:material-code-braces: ListTableOptimizerRunsResponseTypeDef](./type_defs.md#listtableoptimizerrunsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTableOptimizerRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    Type: TableOptimizerTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListTableOptimizerRunsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTableOptimizerRunsResponseTypeDef](./type_defs.md#listtableoptimizerrunsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTableOptimizerRunsRequestPaginateTypeDef = {  # (1)
    "CatalogId": ...,
    "DatabaseName": ...,
    "TableName": ...,
    "Type": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTableOptimizerRunsRequestPaginateTypeDef](./type_defs.md#listtableoptimizerrunsrequestpaginatetypedef) 
## ListTriggersPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_triggers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/ListTriggers.html#Glue.Paginator.ListTriggers)

```python
# ListTriggersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListTriggersPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: ListTriggersPaginator = client.get_paginator("list_triggers")  # (2)
    async for item in paginator.paginate(...):
        item: ListTriggersResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [ListTriggersPaginator](./paginators.md#listtriggerspaginator)
3. item: [:material-code-braces: ListTriggersResponseTypeDef](./type_defs.md#listtriggersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTriggersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DependentJobName: str = ...,
    Tags: Mapping[str, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTriggersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTriggersResponseTypeDef](./type_defs.md#listtriggersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTriggersRequestPaginateTypeDef = {  # (1)
    "DependentJobName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTriggersRequestPaginateTypeDef](./type_defs.md#listtriggersrequestpaginatetypedef) 
## ListUsageProfilesPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_usage_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/ListUsageProfiles.html#Glue.Paginator.ListUsageProfiles)

```python
# ListUsageProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListUsageProfilesPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: ListUsageProfilesPaginator = client.get_paginator("list_usage_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsageProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [ListUsageProfilesPaginator](./paginators.md#listusageprofilespaginator)
3. item: [:material-code-braces: ListUsageProfilesResponseTypeDef](./type_defs.md#listusageprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsageProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListUsageProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsageProfilesResponseTypeDef](./type_defs.md#listusageprofilesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUsageProfilesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsageProfilesRequestPaginateTypeDef](./type_defs.md#listusageprofilesrequestpaginatetypedef) 
## ListWorkflowsPaginator

Type annotations and code completion for `#!python session.create_client("glue").get_paginator("list_workflows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue/paginator/ListWorkflows.html#Glue.Paginator.ListWorkflows)

```python
# ListWorkflowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_glue.paginator import ListWorkflowsPaginator

session = get_session()
async with session.create_client("glue") as client:  # (1)
    paginator: ListWorkflowsPaginator = client.get_paginator("list_workflows")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkflowsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueClient](./client.md)
2. paginator: [ListWorkflowsPaginator](./paginators.md#listworkflowspaginator)
3. item: [:material-code-braces: ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkflowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWorkflowsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowsRequestPaginateTypeDef](./type_defs.md#listworkflowsrequestpaginatetypedef) 
