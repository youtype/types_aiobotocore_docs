<a id="paginators-for-aiobotocore-databasemigrationservice-module"></a>

# Paginators for aiobotocore DatabaseMigrationService module

> [Index](..) > [DatabaseMigrationService](.) > Paginators

Auto-generated documentation for
[DatabaseMigrationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
type annotations stubs module
[types-aiobotocore-dms](https://pypi.org/project/types-aiobotocore-dms/).

- [Paginators for aiobotocore DatabaseMigrationService module](#paginators-for-aiobotocore-databasemigrationservice-module)
  - [DescribeCertificatesPaginator](#describecertificatespaginator)
  - [DescribeConnectionsPaginator](#describeconnectionspaginator)
  - [DescribeEndpointTypesPaginator](#describeendpointtypespaginator)
  - [DescribeEndpointsPaginator](#describeendpointspaginator)
  - [DescribeEventSubscriptionsPaginator](#describeeventsubscriptionspaginator)
  - [DescribeEventsPaginator](#describeeventspaginator)
  - [DescribeOrderableReplicationInstancesPaginator](#describeorderablereplicationinstancespaginator)
  - [DescribeReplicationInstancesPaginator](#describereplicationinstancespaginator)
  - [DescribeReplicationSubnetGroupsPaginator](#describereplicationsubnetgroupspaginator)
  - [DescribeReplicationTaskAssessmentResultsPaginator](#describereplicationtaskassessmentresultspaginator)
  - [DescribeReplicationTasksPaginator](#describereplicationtaskspaginator)
  - [DescribeSchemasPaginator](#describeschemaspaginator)
  - [DescribeTableStatisticsPaginator](#describetablestatisticspaginator)

<a id="describecertificatespaginator"></a>

## DescribeCertificatesPaginator

Type annotations for
`session.create_client("dms").get_paginator("describe_certificates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeCertificatesPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeCertificatesPaginator = client.get_paginator("describe_certificates")
```

Boto3 documentation:
[DatabaseMigrationService.Paginator.DescribeCertificates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates)

Arguments for `DescribeCertificatesPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeCertificatesPaginator.paginate` returns
`_PageIterator`\[[DescribeCertificatesResponseTypeDef](./type_defs.md#describecertificatesresponsetypedef)\].

<a id="describeconnectionspaginator"></a>

## DescribeConnectionsPaginator

Type annotations for
`session.create_client("dms").get_paginator("describe_connections")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeConnectionsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeConnectionsPaginator = client.get_paginator("describe_connections")
```

Boto3 documentation:
[DatabaseMigrationService.Paginator.DescribeConnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections)

Arguments for `DescribeConnectionsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeConnectionsPaginator.paginate` returns
`_PageIterator`\[[DescribeConnectionsResponseTypeDef](./type_defs.md#describeconnectionsresponsetypedef)\].

<a id="describeendpointtypespaginator"></a>

## DescribeEndpointTypesPaginator

Type annotations for
`session.create_client("dms").get_paginator("describe_endpoint_types")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeEndpointTypesPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeEndpointTypesPaginator = client.get_paginator("describe_endpoint_types")
```

Boto3 documentation:
[DatabaseMigrationService.Paginator.DescribeEndpointTypes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes)

Arguments for `DescribeEndpointTypesPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeEndpointTypesPaginator.paginate` returns
`_PageIterator`\[[DescribeEndpointTypesResponseTypeDef](./type_defs.md#describeendpointtypesresponsetypedef)\].

<a id="describeendpointspaginator"></a>

## DescribeEndpointsPaginator

Type annotations for
`session.create_client("dms").get_paginator("describe_endpoints")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeEndpointsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeEndpointsPaginator = client.get_paginator("describe_endpoints")
```

Boto3 documentation:
[DatabaseMigrationService.Paginator.DescribeEndpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints)

Arguments for `DescribeEndpointsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeEndpointsPaginator.paginate` returns
`_PageIterator`\[[DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef)\].

<a id="describeeventsubscriptionspaginator"></a>

## DescribeEventSubscriptionsPaginator

Type annotations for
`session.create_client("dms").get_paginator("describe_event_subscriptions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeEventSubscriptionsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")
```

Boto3 documentation:
[DatabaseMigrationService.Paginator.DescribeEventSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions)

Arguments for `DescribeEventSubscriptionsPaginator.paginate` method:

- `SubscriptionName`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeEventSubscriptionsPaginator.paginate` returns
`_PageIterator`\[[DescribeEventSubscriptionsResponseTypeDef](./type_defs.md#describeeventsubscriptionsresponsetypedef)\].

<a id="describeeventspaginator"></a>

## DescribeEventsPaginator

Type annotations for
`session.create_client("dms").get_paginator("describe_events")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
```

Boto3 documentation:
[DatabaseMigrationService.Paginator.DescribeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents)

Arguments for `DescribeEventsPaginator.paginate` method:

- `SourceIdentifier`: `str`
- `SourceType`: `Literal['replication-instance']` (see
  [SourceTypeType](./literals.md#sourcetypetype))
- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `Duration`: `int`
- `EventCategories`: `Sequence`\[`str`\]
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeEventsPaginator.paginate` returns
`_PageIterator`\[[DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef)\].

<a id="describeorderablereplicationinstancespaginator"></a>

## DescribeOrderableReplicationInstancesPaginator

Type annotations for
`session.create_client("dms").get_paginator("describe_orderable_replication_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeOrderableReplicationInstancesPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeOrderableReplicationInstancesPaginator = client.get_paginator("describe_orderable_replication_instances")
```

Boto3 documentation:
[DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances)

Arguments for `DescribeOrderableReplicationInstancesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeOrderableReplicationInstancesPaginator.paginate` returns
`_PageIterator`\[[DescribeOrderableReplicationInstancesResponseTypeDef](./type_defs.md#describeorderablereplicationinstancesresponsetypedef)\].

<a id="describereplicationinstancespaginator"></a>

## DescribeReplicationInstancesPaginator

Type annotations for
`session.create_client("dms").get_paginator("describe_replication_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeReplicationInstancesPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeReplicationInstancesPaginator = client.get_paginator("describe_replication_instances")
```

Boto3 documentation:
[DatabaseMigrationService.Paginator.DescribeReplicationInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances)

Arguments for `DescribeReplicationInstancesPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeReplicationInstancesPaginator.paginate` returns
`_PageIterator`\[[DescribeReplicationInstancesResponseTypeDef](./type_defs.md#describereplicationinstancesresponsetypedef)\].

<a id="describereplicationsubnetgroupspaginator"></a>

## DescribeReplicationSubnetGroupsPaginator

Type annotations for
`session.create_client("dms").get_paginator("describe_replication_subnet_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeReplicationSubnetGroupsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeReplicationSubnetGroupsPaginator = client.get_paginator("describe_replication_subnet_groups")
```

Boto3 documentation:
[DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups)

Arguments for `DescribeReplicationSubnetGroupsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeReplicationSubnetGroupsPaginator.paginate` returns
`_PageIterator`\[[DescribeReplicationSubnetGroupsResponseTypeDef](./type_defs.md#describereplicationsubnetgroupsresponsetypedef)\].

<a id="describereplicationtaskassessmentresultspaginator"></a>

## DescribeReplicationTaskAssessmentResultsPaginator

Type annotations for
`session.create_client("dms").get_paginator("describe_replication_task_assessment_results")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeReplicationTaskAssessmentResultsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeReplicationTaskAssessmentResultsPaginator = client.get_paginator("describe_replication_task_assessment_results")
```

Boto3 documentation:
[DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults)

Arguments for `DescribeReplicationTaskAssessmentResultsPaginator.paginate`
method:

- `ReplicationTaskArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeReplicationTaskAssessmentResultsPaginator.paginate` returns
`_PageIterator`\[[DescribeReplicationTaskAssessmentResultsResponseTypeDef](./type_defs.md#describereplicationtaskassessmentresultsresponsetypedef)\].

<a id="describereplicationtaskspaginator"></a>

## DescribeReplicationTasksPaginator

Type annotations for
`session.create_client("dms").get_paginator("describe_replication_tasks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeReplicationTasksPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeReplicationTasksPaginator = client.get_paginator("describe_replication_tasks")
```

Boto3 documentation:
[DatabaseMigrationService.Paginator.DescribeReplicationTasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks)

Arguments for `DescribeReplicationTasksPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `WithoutSettings`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeReplicationTasksPaginator.paginate` returns
`_PageIterator`\[[DescribeReplicationTasksResponseTypeDef](./type_defs.md#describereplicationtasksresponsetypedef)\].

<a id="describeschemaspaginator"></a>

## DescribeSchemasPaginator

Type annotations for
`session.create_client("dms").get_paginator("describe_schemas")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeSchemasPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeSchemasPaginator = client.get_paginator("describe_schemas")
```

Boto3 documentation:
[DatabaseMigrationService.Paginator.DescribeSchemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas)

Arguments for `DescribeSchemasPaginator.paginate` method:

- `EndpointArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeSchemasPaginator.paginate` returns
`_PageIterator`\[[DescribeSchemasResponseTypeDef](./type_defs.md#describeschemasresponsetypedef)\].

<a id="describetablestatisticspaginator"></a>

## DescribeTableStatisticsPaginator

Type annotations for
`session.create_client("dms").get_paginator("describe_table_statistics")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.paginator import DescribeTableStatisticsPaginator

session = get_session()
async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeTableStatisticsPaginator = client.get_paginator("describe_table_statistics")
```

Boto3 documentation:
[DatabaseMigrationService.Paginator.DescribeTableStatistics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics)

Arguments for `DescribeTableStatisticsPaginator.paginate` method:

- `ReplicationTaskArn`: `str` *(required)*
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeTableStatisticsPaginator.paginate` returns
`_PageIterator`\[[DescribeTableStatisticsResponseTypeDef](./type_defs.md#describetablestatisticsresponsetypedef)\].
