# Paginators

> [Index](../README.md) > [DatabaseMigrationService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DatabaseMigrationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
    type annotations stubs module [types-aiobotocore-dms](https://pypi.org/project/types-aiobotocore-dms/).

## DescribeCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeCertificatesPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeCertificatesPaginator = client.get_paginator("describe_certificates")
```


### paginate

Type annotations and code completion for `#!python DescribeCertificatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeCertificatesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeCertificatesResponseTypeDef](./type_defs.md#describecertificatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef](./type_defs.md#describecertificatesmessagedescribecertificatespaginatetypedef) 
## DescribeConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeConnectionsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeConnectionsPaginator = client.get_paginator("describe_connections")
```


### paginate

Type annotations and code completion for `#!python DescribeConnectionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeConnectionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeConnectionsResponseTypeDef](./type_defs.md#describeconnectionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef](./type_defs.md#describeconnectionsmessagedescribeconnectionspaginatetypedef) 
## DescribeEndpointTypesPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_endpoint_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeEndpointTypesPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeEndpointTypesPaginator = client.get_paginator("describe_endpoint_types")
```


### paginate

Type annotations and code completion for `#!python DescribeEndpointTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEndpointTypesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEndpointTypesResponseTypeDef](./type_defs.md#describeendpointtypesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef](./type_defs.md#describeendpointtypesmessagedescribeendpointtypespaginatetypedef) 
## DescribeEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeEndpointsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeEndpointsPaginator = client.get_paginator("describe_endpoints")
```


### paginate

Type annotations and code completion for `#!python DescribeEndpointsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEndpointsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef](./type_defs.md#describeendpointsmessagedescribeendpointspaginatetypedef) 
## DescribeEventSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_event_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeEventSubscriptionsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")
```


### paginate

Type annotations and code completion for `#!python DescribeEventSubscriptionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SubscriptionName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEventSubscriptionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEventSubscriptionsResponseTypeDef](./type_defs.md#describeeventsubscriptionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = {  # (1)
    "SubscriptionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef](./type_defs.md#describeeventsubscriptionsmessagedescribeeventsubscriptionspaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
```


### paginate

Type annotations and code completion for `#!python DescribeEventsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SourceIdentifier: str = ...,
    SourceType: SourceTypeType = ...,  # (1)
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    Duration: int = ...,
    EventCategories: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeEventsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventsMessageDescribeEventsPaginateTypeDef = {  # (1)
    "SourceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsMessageDescribeEventsPaginateTypeDef](./type_defs.md#describeeventsmessagedescribeeventspaginatetypedef) 
## DescribeOrderableReplicationInstancesPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_orderable_replication_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeOrderableReplicationInstancesPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeOrderableReplicationInstancesPaginator = client.get_paginator("describe_orderable_replication_instances")
```


### paginate

Type annotations and code completion for `#!python DescribeOrderableReplicationInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeOrderableReplicationInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeOrderableReplicationInstancesResponseTypeDef](./type_defs.md#describeorderablereplicationinstancesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef](./type_defs.md#describeorderablereplicationinstancesmessagedescribeorderablereplicationinstancespaginatetypedef) 
## DescribeReplicationInstancesPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_replication_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeReplicationInstancesPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeReplicationInstancesPaginator = client.get_paginator("describe_replication_instances")
```


### paginate

Type annotations and code completion for `#!python DescribeReplicationInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeReplicationInstancesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeReplicationInstancesResponseTypeDef](./type_defs.md#describereplicationinstancesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef](./type_defs.md#describereplicationinstancesmessagedescribereplicationinstancespaginatetypedef) 
## DescribeReplicationSubnetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_replication_subnet_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeReplicationSubnetGroupsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeReplicationSubnetGroupsPaginator = client.get_paginator("describe_replication_subnet_groups")
```


### paginate

Type annotations and code completion for `#!python DescribeReplicationSubnetGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeReplicationSubnetGroupsResponseTypeDef](./type_defs.md#describereplicationsubnetgroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef](./type_defs.md#describereplicationsubnetgroupsmessagedescribereplicationsubnetgroupspaginatetypedef) 
## DescribeReplicationTaskAssessmentResultsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_replication_task_assessment_results")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeReplicationTaskAssessmentResultsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeReplicationTaskAssessmentResultsPaginator = client.get_paginator("describe_replication_task_assessment_results")
```


### paginate

Type annotations and code completion for `#!python DescribeReplicationTaskAssessmentResultsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ReplicationTaskArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeReplicationTaskAssessmentResultsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReplicationTaskAssessmentResultsResponseTypeDef](./type_defs.md#describereplicationtaskassessmentresultsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef](./type_defs.md#describereplicationtaskassessmentresultsmessagedescribereplicationtaskassessmentresultspaginatetypedef) 
## DescribeReplicationTasksPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_replication_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeReplicationTasksPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeReplicationTasksPaginator = client.get_paginator("describe_replication_tasks")
```


### paginate

Type annotations and code completion for `#!python DescribeReplicationTasksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WithoutSettings: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeReplicationTasksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeReplicationTasksResponseTypeDef](./type_defs.md#describereplicationtasksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef](./type_defs.md#describereplicationtasksmessagedescribereplicationtaskspaginatetypedef) 
## DescribeSchemasPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeSchemasPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeSchemasPaginator = client.get_paginator("describe_schemas")
```


### paginate

Type annotations and code completion for `#!python DescribeSchemasPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    EndpointArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeSchemasResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSchemasResponseTypeDef](./type_defs.md#describeschemasresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSchemasMessageDescribeSchemasPaginateTypeDef = {  # (1)
    "EndpointArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSchemasMessageDescribeSchemasPaginateTypeDef](./type_defs.md#describeschemasmessagedescribeschemaspaginatetypedef) 
## DescribeTableStatisticsPaginator

Type annotations and code completion for `#!python session.create_client("dms").get_paginator("describe_table_statistics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeTableStatisticsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeTableStatisticsPaginator = client.get_paginator("describe_table_statistics")
```


### paginate

Type annotations and code completion for `#!python DescribeTableStatisticsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ReplicationTaskArn: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTableStatisticsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTableStatisticsResponseTypeDef](./type_defs.md#describetablestatisticsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = {  # (1)
    "ReplicationTaskArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef](./type_defs.md#describetablestatisticsmessagedescribetablestatisticspaginatetypedef) 
