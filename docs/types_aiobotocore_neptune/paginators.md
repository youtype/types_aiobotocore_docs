<a id="paginators-for-aiobotocore-neptune-module"></a>

# Paginators for aiobotocore Neptune module

> [Index](../README.md) > [Neptune](./README.md) > Paginators

Auto-generated documentation for
[Neptune](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
type annotations stubs module
[types-aiobotocore-neptune](https://pypi.org/project/types-aiobotocore-neptune/).

- [Paginators for aiobotocore Neptune module](#paginators-for-aiobotocore-neptune-module)
  - [DescribeDBClusterEndpointsPaginator](#describedbclusterendpointspaginator)
  - [DescribeDBClusterParameterGroupsPaginator](#describedbclusterparametergroupspaginator)
  - [DescribeDBClusterParametersPaginator](#describedbclusterparameterspaginator)
  - [DescribeDBClusterSnapshotsPaginator](#describedbclustersnapshotspaginator)
  - [DescribeDBClustersPaginator](#describedbclusterspaginator)
  - [DescribeDBEngineVersionsPaginator](#describedbengineversionspaginator)
  - [DescribeDBInstancesPaginator](#describedbinstancespaginator)
  - [DescribeDBParameterGroupsPaginator](#describedbparametergroupspaginator)
  - [DescribeDBParametersPaginator](#describedbparameterspaginator)
  - [DescribeDBSubnetGroupsPaginator](#describedbsubnetgroupspaginator)
  - [DescribeEngineDefaultParametersPaginator](#describeenginedefaultparameterspaginator)
  - [DescribeEventSubscriptionsPaginator](#describeeventsubscriptionspaginator)
  - [DescribeEventsPaginator](#describeeventspaginator)
  - [DescribeOrderableDBInstanceOptionsPaginator](#describeorderabledbinstanceoptionspaginator)
  - [DescribePendingMaintenanceActionsPaginator](#describependingmaintenanceactionspaginator)

<a id="describedbclusterendpointspaginator"></a>

## DescribeDBClusterEndpointsPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_db_cluster_endpoints")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeDBClusterEndpointsPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeDBClusterEndpointsPaginator = client.get_paginator("describe_db_cluster_endpoints")
```

Boto3 documentation:
[Neptune.Paginator.DescribeDBClusterEndpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterEndpoints)

Arguments for `DescribeDBClusterEndpointsPaginator.paginate` method:

- `DBClusterIdentifier`: `str`
- `DBClusterEndpointIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDBClusterEndpointsPaginator.paginate` returns
`AsyncIterator`\[[DBClusterEndpointMessageTypeDef](./type_defs.md#dbclusterendpointmessagetypedef)\].

<a id="describedbclusterparametergroupspaginator"></a>

## DescribeDBClusterParameterGroupsPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_db_cluster_parameter_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeDBClusterParameterGroupsPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeDBClusterParameterGroupsPaginator = client.get_paginator("describe_db_cluster_parameter_groups")
```

Boto3 documentation:
[Neptune.Paginator.DescribeDBClusterParameterGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameterGroups)

Arguments for `DescribeDBClusterParameterGroupsPaginator.paginate` method:

- `DBClusterParameterGroupName`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDBClusterParameterGroupsPaginator.paginate` returns
`AsyncIterator`\[[DBClusterParameterGroupsMessageTypeDef](./type_defs.md#dbclusterparametergroupsmessagetypedef)\].

<a id="describedbclusterparameterspaginator"></a>

## DescribeDBClusterParametersPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_db_cluster_parameters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeDBClusterParametersPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeDBClusterParametersPaginator = client.get_paginator("describe_db_cluster_parameters")
```

Boto3 documentation:
[Neptune.Paginator.DescribeDBClusterParameters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameters)

Arguments for `DescribeDBClusterParametersPaginator.paginate` method:

- `DBClusterParameterGroupName`: `str` *(required)*
- `Source`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDBClusterParametersPaginator.paginate` returns
`AsyncIterator`\[[DBClusterParameterGroupDetailsTypeDef](./type_defs.md#dbclusterparametergroupdetailstypedef)\].

<a id="describedbclustersnapshotspaginator"></a>

## DescribeDBClusterSnapshotsPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_db_cluster_snapshots")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeDBClusterSnapshotsPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeDBClusterSnapshotsPaginator = client.get_paginator("describe_db_cluster_snapshots")
```

Boto3 documentation:
[Neptune.Paginator.DescribeDBClusterSnapshots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterSnapshots)

Arguments for `DescribeDBClusterSnapshotsPaginator.paginate` method:

- `DBClusterIdentifier`: `str`
- `DBClusterSnapshotIdentifier`: `str`
- `SnapshotType`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `IncludeShared`: `bool`
- `IncludePublic`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDBClusterSnapshotsPaginator.paginate` returns
`AsyncIterator`\[[DBClusterSnapshotMessageTypeDef](./type_defs.md#dbclustersnapshotmessagetypedef)\].

<a id="describedbclusterspaginator"></a>

## DescribeDBClustersPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_db_clusters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeDBClustersPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeDBClustersPaginator = client.get_paginator("describe_db_clusters")
```

Boto3 documentation:
[Neptune.Paginator.DescribeDBClusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusters)

Arguments for `DescribeDBClustersPaginator.paginate` method:

- `DBClusterIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDBClustersPaginator.paginate` returns
`AsyncIterator`\[[DBClusterMessageTypeDef](./type_defs.md#dbclustermessagetypedef)\].

<a id="describedbengineversionspaginator"></a>

## DescribeDBEngineVersionsPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_db_engine_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeDBEngineVersionsPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeDBEngineVersionsPaginator = client.get_paginator("describe_db_engine_versions")
```

Boto3 documentation:
[Neptune.Paginator.DescribeDBEngineVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBEngineVersions)

Arguments for `DescribeDBEngineVersionsPaginator.paginate` method:

- `Engine`: `str`
- `EngineVersion`: `str`
- `DBParameterGroupFamily`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `DefaultOnly`: `bool`
- `ListSupportedCharacterSets`: `bool`
- `ListSupportedTimezones`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDBEngineVersionsPaginator.paginate` returns
`AsyncIterator`\[[DBEngineVersionMessageTypeDef](./type_defs.md#dbengineversionmessagetypedef)\].

<a id="describedbinstancespaginator"></a>

## DescribeDBInstancesPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_db_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeDBInstancesPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeDBInstancesPaginator = client.get_paginator("describe_db_instances")
```

Boto3 documentation:
[Neptune.Paginator.DescribeDBInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBInstances)

Arguments for `DescribeDBInstancesPaginator.paginate` method:

- `DBInstanceIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDBInstancesPaginator.paginate` returns
`AsyncIterator`\[[DBInstanceMessageTypeDef](./type_defs.md#dbinstancemessagetypedef)\].

<a id="describedbparametergroupspaginator"></a>

## DescribeDBParameterGroupsPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_db_parameter_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeDBParameterGroupsPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeDBParameterGroupsPaginator = client.get_paginator("describe_db_parameter_groups")
```

Boto3 documentation:
[Neptune.Paginator.DescribeDBParameterGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameterGroups)

Arguments for `DescribeDBParameterGroupsPaginator.paginate` method:

- `DBParameterGroupName`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDBParameterGroupsPaginator.paginate` returns
`AsyncIterator`\[[DBParameterGroupsMessageTypeDef](./type_defs.md#dbparametergroupsmessagetypedef)\].

<a id="describedbparameterspaginator"></a>

## DescribeDBParametersPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_db_parameters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeDBParametersPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeDBParametersPaginator = client.get_paginator("describe_db_parameters")
```

Boto3 documentation:
[Neptune.Paginator.DescribeDBParameters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameters)

Arguments for `DescribeDBParametersPaginator.paginate` method:

- `DBParameterGroupName`: `str` *(required)*
- `Source`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDBParametersPaginator.paginate` returns
`AsyncIterator`\[[DBParameterGroupDetailsTypeDef](./type_defs.md#dbparametergroupdetailstypedef)\].

<a id="describedbsubnetgroupspaginator"></a>

## DescribeDBSubnetGroupsPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_db_subnet_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeDBSubnetGroupsPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeDBSubnetGroupsPaginator = client.get_paginator("describe_db_subnet_groups")
```

Boto3 documentation:
[Neptune.Paginator.DescribeDBSubnetGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBSubnetGroups)

Arguments for `DescribeDBSubnetGroupsPaginator.paginate` method:

- `DBSubnetGroupName`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDBSubnetGroupsPaginator.paginate` returns
`AsyncIterator`\[[DBSubnetGroupMessageTypeDef](./type_defs.md#dbsubnetgroupmessagetypedef)\].

<a id="describeenginedefaultparameterspaginator"></a>

## DescribeEngineDefaultParametersPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_engine_default_parameters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeEngineDefaultParametersPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeEngineDefaultParametersPaginator = client.get_paginator("describe_engine_default_parameters")
```

Boto3 documentation:
[Neptune.Paginator.DescribeEngineDefaultParameters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEngineDefaultParameters)

Arguments for `DescribeEngineDefaultParametersPaginator.paginate` method:

- `DBParameterGroupFamily`: `str` *(required)*
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeEngineDefaultParametersPaginator.paginate` returns
`AsyncIterator`\[[DescribeEngineDefaultParametersResultTypeDef](./type_defs.md#describeenginedefaultparametersresulttypedef)\].

<a id="describeeventsubscriptionspaginator"></a>

## DescribeEventSubscriptionsPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_event_subscriptions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeEventSubscriptionsPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")
```

Boto3 documentation:
[Neptune.Paginator.DescribeEventSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEventSubscriptions)

Arguments for `DescribeEventSubscriptionsPaginator.paginate` method:

- `SubscriptionName`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeEventSubscriptionsPaginator.paginate` returns
`AsyncIterator`\[[EventSubscriptionsMessageTypeDef](./type_defs.md#eventsubscriptionsmessagetypedef)\].

<a id="describeeventspaginator"></a>

## DescribeEventsPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_events")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
```

Boto3 documentation:
[Neptune.Paginator.DescribeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEvents)

Arguments for `DescribeEventsPaginator.paginate` method:

- `SourceIdentifier`: `str`
- `SourceType`: [SourceTypeType](./literals.md#sourcetypetype)
- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `Duration`: `int`
- `EventCategories`: `Sequence`\[`str`\]
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeEventsPaginator.paginate` returns
`AsyncIterator`\[[EventsMessageTypeDef](./type_defs.md#eventsmessagetypedef)\].

<a id="describeorderabledbinstanceoptionspaginator"></a>

## DescribeOrderableDBInstanceOptionsPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_orderable_db_instance_options")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribeOrderableDBInstanceOptionsPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeOrderableDBInstanceOptionsPaginator = client.get_paginator("describe_orderable_db_instance_options")
```

Boto3 documentation:
[Neptune.Paginator.DescribeOrderableDBInstanceOptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeOrderableDBInstanceOptions)

Arguments for `DescribeOrderableDBInstanceOptionsPaginator.paginate` method:

- `Engine`: `str` *(required)*
- `EngineVersion`: `str`
- `DBInstanceClass`: `str`
- `LicenseModel`: `str`
- `Vpc`: `bool`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeOrderableDBInstanceOptionsPaginator.paginate` returns
`AsyncIterator`\[[OrderableDBInstanceOptionsMessageTypeDef](./type_defs.md#orderabledbinstanceoptionsmessagetypedef)\].

<a id="describependingmaintenanceactionspaginator"></a>

## DescribePendingMaintenanceActionsPaginator

Type annotations for
`session.create_client("neptune").get_paginator("describe_pending_maintenance_actions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.paginator import DescribePendingMaintenanceActionsPaginator

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribePendingMaintenanceActionsPaginator = client.get_paginator("describe_pending_maintenance_actions")
```

Boto3 documentation:
[Neptune.Paginator.DescribePendingMaintenanceActions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribePendingMaintenanceActions)

Arguments for `DescribePendingMaintenanceActionsPaginator.paginate` method:

- `ResourceIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribePendingMaintenanceActionsPaginator.paginate` returns
`AsyncIterator`\[[PendingMaintenanceActionsMessageTypeDef](./type_defs.md#pendingmaintenanceactionsmessagetypedef)\].
