# Paginators

> [Index](../README.md) > [DatabaseMigrationService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DatabaseMigrationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#databasemigrationservice)
    type annotations stubs module [types-aiobotocore-dms](https://pypi.org/project/types-aiobotocore-dms/).

## DescribeCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeCertificates.html#DatabaseMigrationService.Paginator.DescribeCertificates)

```python
# DescribeCertificatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeCertificatesPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeCertificatesPaginator = client.get_paginator("describe_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCertificatesResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeCertificatesPaginator](./paginators.md#describecertificatespaginator)
3. item: [:material-code-braces: DescribeCertificatesResponseTypeDef](./type_defs.md#describecertificatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCertificatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeCertificatesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeCertificatesResponseTypeDef](./type_defs.md#describecertificatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCertificatesMessagePaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCertificatesMessagePaginateTypeDef](./type_defs.md#describecertificatesmessagepaginatetypedef) 
## DescribeConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeConnections.html#DatabaseMigrationService.Paginator.DescribeConnections)

```python
# DescribeConnectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeConnectionsPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeConnectionsPaginator = client.get_paginator("describe_connections")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConnectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeConnectionsPaginator](./paginators.md#describeconnectionspaginator)
3. item: [:material-code-braces: DescribeConnectionsResponseTypeDef](./type_defs.md#describeconnectionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConnectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeConnectionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeConnectionsResponseTypeDef](./type_defs.md#describeconnectionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeConnectionsMessagePaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConnectionsMessagePaginateTypeDef](./type_defs.md#describeconnectionsmessagepaginatetypedef) 
## DescribeDataMigrationsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_data_migrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeDataMigrations.html#DatabaseMigrationService.Paginator.DescribeDataMigrations)

```python
# DescribeDataMigrationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeDataMigrationsPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeDataMigrationsPaginator = client.get_paginator("describe_data_migrations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDataMigrationsResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeDataMigrationsPaginator](./paginators.md#describedatamigrationspaginator)
3. item: [:material-code-braces: DescribeDataMigrationsResponseTypeDef](./type_defs.md#describedatamigrationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDataMigrationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WithoutSettings: bool = ...,
    WithoutStatistics: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeDataMigrationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDataMigrationsResponseTypeDef](./type_defs.md#describedatamigrationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDataMigrationsMessagePaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDataMigrationsMessagePaginateTypeDef](./type_defs.md#describedatamigrationsmessagepaginatetypedef) 
## DescribeEndpointTypesPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_endpoint_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeEndpointTypes.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes)

```python
# DescribeEndpointTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeEndpointTypesPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeEndpointTypesPaginator = client.get_paginator("describe_endpoint_types")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEndpointTypesResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeEndpointTypesPaginator](./paginators.md#describeendpointtypespaginator)
3. item: [:material-code-braces: DescribeEndpointTypesResponseTypeDef](./type_defs.md#describeendpointtypesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEndpointTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeEndpointTypesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEndpointTypesResponseTypeDef](./type_defs.md#describeendpointtypesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEndpointTypesMessagePaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointTypesMessagePaginateTypeDef](./type_defs.md#describeendpointtypesmessagepaginatetypedef) 
## DescribeEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeEndpoints.html#DatabaseMigrationService.Paginator.DescribeEndpoints)

```python
# DescribeEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeEndpointsPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeEndpointsPaginator = client.get_paginator("describe_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeEndpointsPaginator](./paginators.md#describeendpointspaginator)
3. item: [:material-code-braces: DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeEndpointsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEndpointsMessagePaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointsMessagePaginateTypeDef](./type_defs.md#describeendpointsmessagepaginatetypedef) 
## DescribeEventSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_event_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeEventSubscriptions.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions)

```python
# DescribeEventSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeEventSubscriptionsPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEventSubscriptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeEventSubscriptionsPaginator](./paginators.md#describeeventsubscriptionspaginator)
3. item: [:material-code-braces: DescribeEventSubscriptionsResponseTypeDef](./type_defs.md#describeeventsubscriptionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SubscriptionName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeEventSubscriptionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEventSubscriptionsResponseTypeDef](./type_defs.md#describeeventsubscriptionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEventSubscriptionsMessagePaginateTypeDef = {  # (1)
    "SubscriptionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventSubscriptionsMessagePaginateTypeDef](./type_defs.md#describeeventsubscriptionsmessagepaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeEvents.html#DatabaseMigrationService.Paginator.DescribeEvents)

```python
# DescribeEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
3. item: [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SourceIdentifier: str = ...,
    SourceType: SourceTypeType = ...,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    Duration: int = ...,
    EventCategories: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[DescribeEventsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEventsMessagePaginateTypeDef = {  # (1)
    "SourceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsMessagePaginateTypeDef](./type_defs.md#describeeventsmessagepaginatetypedef) 
## DescribeOrderableReplicationInstancesPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_orderable_replication_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeOrderableReplicationInstances.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances)

```python
# DescribeOrderableReplicationInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeOrderableReplicationInstancesPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeOrderableReplicationInstancesPaginator = client.get_paginator("describe_orderable_replication_instances")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeOrderableReplicationInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeOrderableReplicationInstancesPaginator](./paginators.md#describeorderablereplicationinstancespaginator)
3. item: [:material-code-braces: DescribeOrderableReplicationInstancesResponseTypeDef](./type_defs.md#describeorderablereplicationinstancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrderableReplicationInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeOrderableReplicationInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeOrderableReplicationInstancesResponseTypeDef](./type_defs.md#describeorderablereplicationinstancesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeOrderableReplicationInstancesMessagePaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrderableReplicationInstancesMessagePaginateTypeDef](./type_defs.md#describeorderablereplicationinstancesmessagepaginatetypedef) 
## DescribeReplicationInstancesPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_replication_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeReplicationInstances.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances)

```python
# DescribeReplicationInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeReplicationInstancesPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeReplicationInstancesPaginator = client.get_paginator("describe_replication_instances")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReplicationInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeReplicationInstancesPaginator](./paginators.md#describereplicationinstancespaginator)
3. item: [:material-code-braces: DescribeReplicationInstancesResponseTypeDef](./type_defs.md#describereplicationinstancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReplicationInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeReplicationInstancesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeReplicationInstancesResponseTypeDef](./type_defs.md#describereplicationinstancesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReplicationInstancesMessagePaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationInstancesMessagePaginateTypeDef](./type_defs.md#describereplicationinstancesmessagepaginatetypedef) 
## DescribeReplicationSubnetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_replication_subnet_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeReplicationSubnetGroups.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups)

```python
# DescribeReplicationSubnetGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeReplicationSubnetGroupsPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeReplicationSubnetGroupsPaginator = client.get_paginator("describe_replication_subnet_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReplicationSubnetGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeReplicationSubnetGroupsPaginator](./paginators.md#describereplicationsubnetgroupspaginator)
3. item: [:material-code-braces: DescribeReplicationSubnetGroupsResponseTypeDef](./type_defs.md#describereplicationsubnetgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReplicationSubnetGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeReplicationSubnetGroupsResponseTypeDef](./type_defs.md#describereplicationsubnetgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReplicationSubnetGroupsMessagePaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationSubnetGroupsMessagePaginateTypeDef](./type_defs.md#describereplicationsubnetgroupsmessagepaginatetypedef) 
## DescribeReplicationTaskAssessmentResultsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_replication_task_assessment_results")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeReplicationTaskAssessmentResults.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults)

```python
# DescribeReplicationTaskAssessmentResultsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeReplicationTaskAssessmentResultsPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeReplicationTaskAssessmentResultsPaginator = client.get_paginator("describe_replication_task_assessment_results")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReplicationTaskAssessmentResultsResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeReplicationTaskAssessmentResultsPaginator](./paginators.md#describereplicationtaskassessmentresultspaginator)
3. item: [:material-code-braces: DescribeReplicationTaskAssessmentResultsResponseTypeDef](./type_defs.md#describereplicationtaskassessmentresultsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReplicationTaskAssessmentResultsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReplicationTaskArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeReplicationTaskAssessmentResultsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReplicationTaskAssessmentResultsResponseTypeDef](./type_defs.md#describereplicationtaskassessmentresultsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReplicationTaskAssessmentResultsMessagePaginateTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationTaskAssessmentResultsMessagePaginateTypeDef](./type_defs.md#describereplicationtaskassessmentresultsmessagepaginatetypedef) 
## DescribeReplicationTasksPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_replication_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeReplicationTasks.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks)

```python
# DescribeReplicationTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeReplicationTasksPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeReplicationTasksPaginator = client.get_paginator("describe_replication_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReplicationTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeReplicationTasksPaginator](./paginators.md#describereplicationtaskspaginator)
3. item: [:material-code-braces: DescribeReplicationTasksResponseTypeDef](./type_defs.md#describereplicationtasksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReplicationTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WithoutSettings: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeReplicationTasksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeReplicationTasksResponseTypeDef](./type_defs.md#describereplicationtasksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReplicationTasksMessagePaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationTasksMessagePaginateTypeDef](./type_defs.md#describereplicationtasksmessagepaginatetypedef) 
## DescribeSchemasPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeSchemas.html#DatabaseMigrationService.Paginator.DescribeSchemas)

```python
# DescribeSchemasPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeSchemasPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeSchemasPaginator = client.get_paginator("describe_schemas")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSchemasResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeSchemasPaginator](./paginators.md#describeschemaspaginator)
3. item: [:material-code-braces: DescribeSchemasResponseTypeDef](./type_defs.md#describeschemasresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSchemasPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    EndpointArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeSchemasResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSchemasResponseTypeDef](./type_defs.md#describeschemasresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSchemasMessagePaginateTypeDef = {  # (1)
    "EndpointArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSchemasMessagePaginateTypeDef](./type_defs.md#describeschemasmessagepaginatetypedef) 
## DescribeTableStatisticsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_table_statistics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms/paginator/DescribeTableStatistics.html#DatabaseMigrationService.Paginator.DescribeTableStatistics)

```python
# DescribeTableStatisticsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeTableStatisticsPaginator

session = get_session()
async with session.create_client("dms") as client:  # (1)
    paginator: DescribeTableStatisticsPaginator = client.get_paginator("describe_table_statistics")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTableStatisticsResponseTypeDef
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeTableStatisticsPaginator](./paginators.md#describetablestatisticspaginator)
3. item: [:material-code-braces: DescribeTableStatisticsResponseTypeDef](./type_defs.md#describetablestatisticsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTableStatisticsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReplicationTaskArn: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeTableStatisticsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTableStatisticsResponseTypeDef](./type_defs.md#describetablestatisticsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTableStatisticsMessagePaginateTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTableStatisticsMessagePaginateTypeDef](./type_defs.md#describetablestatisticsmessagepaginatetypedef) 
