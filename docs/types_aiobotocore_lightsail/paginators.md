<a id="paginators-for-aiobotocore-lightsail-module"></a>

# Paginators for aiobotocore Lightsail module

> [Index](../README.md) > [Lightsail](./README.md) > Paginators

Auto-generated documentation for
[Lightsail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
type annotations stubs module
[types-aiobotocore-lightsail](https://pypi.org/project/types-aiobotocore-lightsail/).

- [Paginators for aiobotocore Lightsail module](#paginators-for-aiobotocore-lightsail-module)
  - [GetActiveNamesPaginator](#getactivenamespaginator)
  - [GetBlueprintsPaginator](#getblueprintspaginator)
  - [GetBundlesPaginator](#getbundlespaginator)
  - [GetCloudFormationStackRecordsPaginator](#getcloudformationstackrecordspaginator)
  - [GetDiskSnapshotsPaginator](#getdisksnapshotspaginator)
  - [GetDisksPaginator](#getdiskspaginator)
  - [GetDomainsPaginator](#getdomainspaginator)
  - [GetExportSnapshotRecordsPaginator](#getexportsnapshotrecordspaginator)
  - [GetInstanceSnapshotsPaginator](#getinstancesnapshotspaginator)
  - [GetInstancesPaginator](#getinstancespaginator)
  - [GetKeyPairsPaginator](#getkeypairspaginator)
  - [GetLoadBalancersPaginator](#getloadbalancerspaginator)
  - [GetOperationsPaginator](#getoperationspaginator)
  - [GetRelationalDatabaseBlueprintsPaginator](#getrelationaldatabaseblueprintspaginator)
  - [GetRelationalDatabaseBundlesPaginator](#getrelationaldatabasebundlespaginator)
  - [GetRelationalDatabaseEventsPaginator](#getrelationaldatabaseeventspaginator)
  - [GetRelationalDatabaseParametersPaginator](#getrelationaldatabaseparameterspaginator)
  - [GetRelationalDatabaseSnapshotsPaginator](#getrelationaldatabasesnapshotspaginator)
  - [GetRelationalDatabasesPaginator](#getrelationaldatabasespaginator)
  - [GetStaticIpsPaginator](#getstaticipspaginator)

<a id="getactivenamespaginator"></a>

## GetActiveNamesPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_active_names")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetActiveNamesPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetActiveNamesPaginator = client.get_paginator("get_active_names")
```

Boto3 documentation:
[Lightsail.Paginator.GetActiveNames](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetActiveNames)

Arguments for `GetActiveNamesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetActiveNamesPaginator.paginate` returns
`AsyncIterator`\[[GetActiveNamesResultTypeDef](./type_defs.md#getactivenamesresulttypedef)\].

<a id="getblueprintspaginator"></a>

## GetBlueprintsPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_blueprints")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetBlueprintsPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetBlueprintsPaginator = client.get_paginator("get_blueprints")
```

Boto3 documentation:
[Lightsail.Paginator.GetBlueprints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBlueprints)

Arguments for `GetBlueprintsPaginator.paginate` method:

- `includeInactive`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetBlueprintsPaginator.paginate` returns
`AsyncIterator`\[[GetBlueprintsResultTypeDef](./type_defs.md#getblueprintsresulttypedef)\].

<a id="getbundlespaginator"></a>

## GetBundlesPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_bundles")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetBundlesPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetBundlesPaginator = client.get_paginator("get_bundles")
```

Boto3 documentation:
[Lightsail.Paginator.GetBundles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBundles)

Arguments for `GetBundlesPaginator.paginate` method:

- `includeInactive`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetBundlesPaginator.paginate` returns
`AsyncIterator`\[[GetBundlesResultTypeDef](./type_defs.md#getbundlesresulttypedef)\].

<a id="getcloudformationstackrecordspaginator"></a>

## GetCloudFormationStackRecordsPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_cloud_formation_stack_records")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetCloudFormationStackRecordsPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetCloudFormationStackRecordsPaginator = client.get_paginator("get_cloud_formation_stack_records")
```

Boto3 documentation:
[Lightsail.Paginator.GetCloudFormationStackRecords](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetCloudFormationStackRecords)

Arguments for `GetCloudFormationStackRecordsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetCloudFormationStackRecordsPaginator.paginate` returns
`AsyncIterator`\[[GetCloudFormationStackRecordsResultTypeDef](./type_defs.md#getcloudformationstackrecordsresulttypedef)\].

<a id="getdisksnapshotspaginator"></a>

## GetDiskSnapshotsPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_disk_snapshots")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetDiskSnapshotsPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetDiskSnapshotsPaginator = client.get_paginator("get_disk_snapshots")
```

Boto3 documentation:
[Lightsail.Paginator.GetDiskSnapshots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDiskSnapshots)

Arguments for `GetDiskSnapshotsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDiskSnapshotsPaginator.paginate` returns
`AsyncIterator`\[[GetDiskSnapshotsResultTypeDef](./type_defs.md#getdisksnapshotsresulttypedef)\].

<a id="getdiskspaginator"></a>

## GetDisksPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_disks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetDisksPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetDisksPaginator = client.get_paginator("get_disks")
```

Boto3 documentation:
[Lightsail.Paginator.GetDisks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDisks)

Arguments for `GetDisksPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDisksPaginator.paginate` returns
`AsyncIterator`\[[GetDisksResultTypeDef](./type_defs.md#getdisksresulttypedef)\].

<a id="getdomainspaginator"></a>

## GetDomainsPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_domains")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetDomainsPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetDomainsPaginator = client.get_paginator("get_domains")
```

Boto3 documentation:
[Lightsail.Paginator.GetDomains](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDomains)

Arguments for `GetDomainsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDomainsPaginator.paginate` returns
`AsyncIterator`\[[GetDomainsResultTypeDef](./type_defs.md#getdomainsresulttypedef)\].

<a id="getexportsnapshotrecordspaginator"></a>

## GetExportSnapshotRecordsPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_export_snapshot_records")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetExportSnapshotRecordsPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetExportSnapshotRecordsPaginator = client.get_paginator("get_export_snapshot_records")
```

Boto3 documentation:
[Lightsail.Paginator.GetExportSnapshotRecords](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetExportSnapshotRecords)

Arguments for `GetExportSnapshotRecordsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetExportSnapshotRecordsPaginator.paginate` returns
`AsyncIterator`\[[GetExportSnapshotRecordsResultTypeDef](./type_defs.md#getexportsnapshotrecordsresulttypedef)\].

<a id="getinstancesnapshotspaginator"></a>

## GetInstanceSnapshotsPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_instance_snapshots")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetInstanceSnapshotsPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetInstanceSnapshotsPaginator = client.get_paginator("get_instance_snapshots")
```

Boto3 documentation:
[Lightsail.Paginator.GetInstanceSnapshots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstanceSnapshots)

Arguments for `GetInstanceSnapshotsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetInstanceSnapshotsPaginator.paginate` returns
`AsyncIterator`\[[GetInstanceSnapshotsResultTypeDef](./type_defs.md#getinstancesnapshotsresulttypedef)\].

<a id="getinstancespaginator"></a>

## GetInstancesPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetInstancesPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetInstancesPaginator = client.get_paginator("get_instances")
```

Boto3 documentation:
[Lightsail.Paginator.GetInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstances)

Arguments for `GetInstancesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetInstancesPaginator.paginate` returns
`AsyncIterator`\[[GetInstancesResultTypeDef](./type_defs.md#getinstancesresulttypedef)\].

<a id="getkeypairspaginator"></a>

## GetKeyPairsPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_key_pairs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetKeyPairsPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetKeyPairsPaginator = client.get_paginator("get_key_pairs")
```

Boto3 documentation:
[Lightsail.Paginator.GetKeyPairs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetKeyPairs)

Arguments for `GetKeyPairsPaginator.paginate` method:

- `includeDefaultKeyPair`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetKeyPairsPaginator.paginate` returns
`AsyncIterator`\[[GetKeyPairsResultTypeDef](./type_defs.md#getkeypairsresulttypedef)\].

<a id="getloadbalancerspaginator"></a>

## GetLoadBalancersPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_load_balancers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetLoadBalancersPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetLoadBalancersPaginator = client.get_paginator("get_load_balancers")
```

Boto3 documentation:
[Lightsail.Paginator.GetLoadBalancers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetLoadBalancers)

Arguments for `GetLoadBalancersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetLoadBalancersPaginator.paginate` returns
`AsyncIterator`\[[GetLoadBalancersResultTypeDef](./type_defs.md#getloadbalancersresulttypedef)\].

<a id="getoperationspaginator"></a>

## GetOperationsPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_operations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetOperationsPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetOperationsPaginator = client.get_paginator("get_operations")
```

Boto3 documentation:
[Lightsail.Paginator.GetOperations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetOperations)

Arguments for `GetOperationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetOperationsPaginator.paginate` returns
`AsyncIterator`\[[GetOperationsResultTypeDef](./type_defs.md#getoperationsresulttypedef)\].

<a id="getrelationaldatabaseblueprintspaginator"></a>

## GetRelationalDatabaseBlueprintsPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_relational_database_blueprints")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetRelationalDatabaseBlueprintsPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetRelationalDatabaseBlueprintsPaginator = client.get_paginator("get_relational_database_blueprints")
```

Boto3 documentation:
[Lightsail.Paginator.GetRelationalDatabaseBlueprints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBlueprints)

Arguments for `GetRelationalDatabaseBlueprintsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetRelationalDatabaseBlueprintsPaginator.paginate` returns
`AsyncIterator`\[[GetRelationalDatabaseBlueprintsResultTypeDef](./type_defs.md#getrelationaldatabaseblueprintsresulttypedef)\].

<a id="getrelationaldatabasebundlespaginator"></a>

## GetRelationalDatabaseBundlesPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_relational_database_bundles")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetRelationalDatabaseBundlesPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetRelationalDatabaseBundlesPaginator = client.get_paginator("get_relational_database_bundles")
```

Boto3 documentation:
[Lightsail.Paginator.GetRelationalDatabaseBundles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBundles)

Arguments for `GetRelationalDatabaseBundlesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetRelationalDatabaseBundlesPaginator.paginate` returns
`AsyncIterator`\[[GetRelationalDatabaseBundlesResultTypeDef](./type_defs.md#getrelationaldatabasebundlesresulttypedef)\].

<a id="getrelationaldatabaseeventspaginator"></a>

## GetRelationalDatabaseEventsPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_relational_database_events")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetRelationalDatabaseEventsPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetRelationalDatabaseEventsPaginator = client.get_paginator("get_relational_database_events")
```

Boto3 documentation:
[Lightsail.Paginator.GetRelationalDatabaseEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseEvents)

Arguments for `GetRelationalDatabaseEventsPaginator.paginate` method:

- `relationalDatabaseName`: `str` *(required)*
- `durationInMinutes`: `int`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetRelationalDatabaseEventsPaginator.paginate` returns
`AsyncIterator`\[[GetRelationalDatabaseEventsResultTypeDef](./type_defs.md#getrelationaldatabaseeventsresulttypedef)\].

<a id="getrelationaldatabaseparameterspaginator"></a>

## GetRelationalDatabaseParametersPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_relational_database_parameters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetRelationalDatabaseParametersPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetRelationalDatabaseParametersPaginator = client.get_paginator("get_relational_database_parameters")
```

Boto3 documentation:
[Lightsail.Paginator.GetRelationalDatabaseParameters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseParameters)

Arguments for `GetRelationalDatabaseParametersPaginator.paginate` method:

- `relationalDatabaseName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetRelationalDatabaseParametersPaginator.paginate` returns
`AsyncIterator`\[[GetRelationalDatabaseParametersResultTypeDef](./type_defs.md#getrelationaldatabaseparametersresulttypedef)\].

<a id="getrelationaldatabasesnapshotspaginator"></a>

## GetRelationalDatabaseSnapshotsPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_relational_database_snapshots")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetRelationalDatabaseSnapshotsPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetRelationalDatabaseSnapshotsPaginator = client.get_paginator("get_relational_database_snapshots")
```

Boto3 documentation:
[Lightsail.Paginator.GetRelationalDatabaseSnapshots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseSnapshots)

Arguments for `GetRelationalDatabaseSnapshotsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetRelationalDatabaseSnapshotsPaginator.paginate` returns
`AsyncIterator`\[[GetRelationalDatabaseSnapshotsResultTypeDef](./type_defs.md#getrelationaldatabasesnapshotsresulttypedef)\].

<a id="getrelationaldatabasespaginator"></a>

## GetRelationalDatabasesPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_relational_databases")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetRelationalDatabasesPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetRelationalDatabasesPaginator = client.get_paginator("get_relational_databases")
```

Boto3 documentation:
[Lightsail.Paginator.GetRelationalDatabases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabases)

Arguments for `GetRelationalDatabasesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetRelationalDatabasesPaginator.paginate` returns
`AsyncIterator`\[[GetRelationalDatabasesResultTypeDef](./type_defs.md#getrelationaldatabasesresulttypedef)\].

<a id="getstaticipspaginator"></a>

## GetStaticIpsPaginator

Type annotations for
`session.create_client("lightsail").get_paginator("get_static_ips")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetStaticIpsPaginator

session = get_session()
async with session.create_client("lightsail") as client:
    client: LightsailClient
    paginator: GetStaticIpsPaginator = client.get_paginator("get_static_ips")
```

Boto3 documentation:
[Lightsail.Paginator.GetStaticIps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetStaticIps)

Arguments for `GetStaticIpsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetStaticIpsPaginator.paginate` returns
`AsyncIterator`\[[GetStaticIpsResultTypeDef](./type_defs.md#getstaticipsresulttypedef)\].