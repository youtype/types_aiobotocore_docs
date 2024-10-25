# Waiters

> [Index](../README.md) > [RDS](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [RDS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
    type annotations stubs module [types-aiobotocore-rds](https://pypi.org/project/types-aiobotocore-rds/).

## DBClusterAvailableWaiter

Type annotations and code completion for `#!python session.create_client("rds").get_waiter("db_cluster_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterAvailable)

```python
# DBClusterAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rds.waiter import DBClusterAvailableWaiter

session = get_session()
async with session.create_client("rds") as client:  # (1)
    waiter: DBClusterAvailableWaiter = client.get_waiter("db_cluster_available")  # (2)
    await waiter.wait()
```

1. client: [RDSClient](./client.md)
2. waiter: [DBClusterAvailableWaiter](./waiters.md#dbclusteravailablewaiter)


### wait

Type annotations and code completion for `#!python DBClusterAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DBClusterIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    IncludeShared: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeDBClustersMessageDBClusterAvailableWaitTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeDBClustersMessageDBClusterAvailableWaitTypeDef](./type_defs.md#describedbclustersmessagedbclusteravailablewaittypedef) 
## DBClusterDeletedWaiter

Type annotations and code completion for `#!python session.create_client("rds").get_waiter("db_cluster_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterDeleted)

```python
# DBClusterDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rds.waiter import DBClusterDeletedWaiter

session = get_session()
async with session.create_client("rds") as client:  # (1)
    waiter: DBClusterDeletedWaiter = client.get_waiter("db_cluster_deleted")  # (2)
    await waiter.wait()
```

1. client: [RDSClient](./client.md)
2. waiter: [DBClusterDeletedWaiter](./waiters.md#dbclusterdeletedwaiter)


### wait

Type annotations and code completion for `#!python DBClusterDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DBClusterIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    IncludeShared: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeDBClustersMessageDBClusterDeletedWaitTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeDBClustersMessageDBClusterDeletedWaitTypeDef](./type_defs.md#describedbclustersmessagedbclusterdeletedwaittypedef) 
## DBClusterSnapshotAvailableWaiter

Type annotations and code completion for `#!python session.create_client("rds").get_waiter("db_cluster_snapshot_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotAvailable)

```python
# DBClusterSnapshotAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rds.waiter import DBClusterSnapshotAvailableWaiter

session = get_session()
async with session.create_client("rds") as client:  # (1)
    waiter: DBClusterSnapshotAvailableWaiter = client.get_waiter("db_cluster_snapshot_available")  # (2)
    await waiter.wait()
```

1. client: [RDSClient](./client.md)
2. waiter: [DBClusterSnapshotAvailableWaiter](./waiters.md#dbclustersnapshotavailablewaiter)


### wait

Type annotations and code completion for `#!python DBClusterSnapshotAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DBClusterIdentifier: str = ...,
    DBClusterSnapshotIdentifier: str = ...,
    SnapshotType: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    IncludeShared: bool = ...,
    IncludePublic: bool = ...,
    DbClusterResourceId: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeDBClusterSnapshotsMessageDBClusterSnapshotAvailableWaitTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterSnapshotsMessageDBClusterSnapshotAvailableWaitTypeDef](./type_defs.md#describedbclustersnapshotsmessagedbclustersnapshotavailablewaittypedef) 
## DBClusterSnapshotDeletedWaiter

Type annotations and code completion for `#!python session.create_client("rds").get_waiter("db_cluster_snapshot_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotDeleted)

```python
# DBClusterSnapshotDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rds.waiter import DBClusterSnapshotDeletedWaiter

session = get_session()
async with session.create_client("rds") as client:  # (1)
    waiter: DBClusterSnapshotDeletedWaiter = client.get_waiter("db_cluster_snapshot_deleted")  # (2)
    await waiter.wait()
```

1. client: [RDSClient](./client.md)
2. waiter: [DBClusterSnapshotDeletedWaiter](./waiters.md#dbclustersnapshotdeletedwaiter)


### wait

Type annotations and code completion for `#!python DBClusterSnapshotDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DBClusterIdentifier: str = ...,
    DBClusterSnapshotIdentifier: str = ...,
    SnapshotType: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    IncludeShared: bool = ...,
    IncludePublic: bool = ...,
    DbClusterResourceId: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeDBClusterSnapshotsMessageDBClusterSnapshotDeletedWaitTypeDef = {  # (1)
    "DBClusterIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeDBClusterSnapshotsMessageDBClusterSnapshotDeletedWaitTypeDef](./type_defs.md#describedbclustersnapshotsmessagedbclustersnapshotdeletedwaittypedef) 
## DBInstanceAvailableWaiter

Type annotations and code completion for `#!python session.create_client("rds").get_waiter("db_instance_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBInstanceAvailable)

```python
# DBInstanceAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rds.waiter import DBInstanceAvailableWaiter

session = get_session()
async with session.create_client("rds") as client:  # (1)
    waiter: DBInstanceAvailableWaiter = client.get_waiter("db_instance_available")  # (2)
    await waiter.wait()
```

1. client: [RDSClient](./client.md)
2. waiter: [DBInstanceAvailableWaiter](./waiters.md#dbinstanceavailablewaiter)


### wait

Type annotations and code completion for `#!python DBInstanceAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef](./type_defs.md#describedbinstancesmessagedbinstanceavailablewaittypedef) 
## DBInstanceDeletedWaiter

Type annotations and code completion for `#!python session.create_client("rds").get_waiter("db_instance_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBInstanceDeleted)

```python
# DBInstanceDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rds.waiter import DBInstanceDeletedWaiter

session = get_session()
async with session.create_client("rds") as client:  # (1)
    waiter: DBInstanceDeletedWaiter = client.get_waiter("db_instance_deleted")  # (2)
    await waiter.wait()
```

1. client: [RDSClient](./client.md)
2. waiter: [DBInstanceDeletedWaiter](./waiters.md#dbinstancedeletedwaiter)


### wait

Type annotations and code completion for `#!python DBInstanceDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef](./type_defs.md#describedbinstancesmessagedbinstancedeletedwaittypedef) 
## DBSnapshotAvailableWaiter

Type annotations and code completion for `#!python session.create_client("rds").get_waiter("db_snapshot_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotAvailable)

```python
# DBSnapshotAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rds.waiter import DBSnapshotAvailableWaiter

session = get_session()
async with session.create_client("rds") as client:  # (1)
    waiter: DBSnapshotAvailableWaiter = client.get_waiter("db_snapshot_available")  # (2)
    await waiter.wait()
```

1. client: [RDSClient](./client.md)
2. waiter: [DBSnapshotAvailableWaiter](./waiters.md#dbsnapshotavailablewaiter)


### wait

Type annotations and code completion for `#!python DBSnapshotAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    DBSnapshotIdentifier: str = ...,
    SnapshotType: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    IncludeShared: bool = ...,
    IncludePublic: bool = ...,
    DbiResourceId: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeDBSnapshotsMessageDBSnapshotAvailableWaitTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeDBSnapshotsMessageDBSnapshotAvailableWaitTypeDef](./type_defs.md#describedbsnapshotsmessagedbsnapshotavailablewaittypedef) 
## DBSnapshotCompletedWaiter

Type annotations and code completion for `#!python session.create_client("rds").get_waiter("db_snapshot_completed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotCompleted)

```python
# DBSnapshotCompletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rds.waiter import DBSnapshotCompletedWaiter

session = get_session()
async with session.create_client("rds") as client:  # (1)
    waiter: DBSnapshotCompletedWaiter = client.get_waiter("db_snapshot_completed")  # (2)
    await waiter.wait()
```

1. client: [RDSClient](./client.md)
2. waiter: [DBSnapshotCompletedWaiter](./waiters.md#dbsnapshotcompletedwaiter)


### wait

Type annotations and code completion for `#!python DBSnapshotCompletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    DBSnapshotIdentifier: str = ...,
    SnapshotType: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    IncludeShared: bool = ...,
    IncludePublic: bool = ...,
    DbiResourceId: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeDBSnapshotsMessageDBSnapshotCompletedWaitTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeDBSnapshotsMessageDBSnapshotCompletedWaitTypeDef](./type_defs.md#describedbsnapshotsmessagedbsnapshotcompletedwaittypedef) 
## DBSnapshotDeletedWaiter

Type annotations and code completion for `#!python session.create_client("rds").get_waiter("db_snapshot_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotDeleted)

```python
# DBSnapshotDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rds.waiter import DBSnapshotDeletedWaiter

session = get_session()
async with session.create_client("rds") as client:  # (1)
    waiter: DBSnapshotDeletedWaiter = client.get_waiter("db_snapshot_deleted")  # (2)
    await waiter.wait()
```

1. client: [RDSClient](./client.md)
2. waiter: [DBSnapshotDeletedWaiter](./waiters.md#dbsnapshotdeletedwaiter)


### wait

Type annotations and code completion for `#!python DBSnapshotDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    DBSnapshotIdentifier: str = ...,
    SnapshotType: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxRecords: int = ...,
    Marker: str = ...,
    IncludeShared: bool = ...,
    IncludePublic: bool = ...,
    DbiResourceId: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeDBSnapshotsMessageDBSnapshotDeletedWaitTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeDBSnapshotsMessageDBSnapshotDeletedWaitTypeDef](./type_defs.md#describedbsnapshotsmessagedbsnapshotdeletedwaittypedef) 
## TenantDatabaseAvailableWaiter

Type annotations and code completion for `#!python session.create_client("rds").get_waiter("tenant_database_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.TenantDatabaseAvailable)

```python
# TenantDatabaseAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rds.waiter import TenantDatabaseAvailableWaiter

session = get_session()
async with session.create_client("rds") as client:  # (1)
    waiter: TenantDatabaseAvailableWaiter = client.get_waiter("tenant_database_available")  # (2)
    await waiter.wait()
```

1. client: [RDSClient](./client.md)
2. waiter: [TenantDatabaseAvailableWaiter](./waiters.md#tenantdatabaseavailablewaiter)


### wait

Type annotations and code completion for `#!python TenantDatabaseAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    TenantDBName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    Marker: str = ...,
    MaxRecords: int = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeTenantDatabasesMessageTenantDatabaseAvailableWaitTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeTenantDatabasesMessageTenantDatabaseAvailableWaitTypeDef](./type_defs.md#describetenantdatabasesmessagetenantdatabaseavailablewaittypedef) 
## TenantDatabaseDeletedWaiter

Type annotations and code completion for `#!python session.create_client("rds").get_waiter("tenant_database_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.TenantDatabaseDeleted)

```python
# TenantDatabaseDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_rds.waiter import TenantDatabaseDeletedWaiter

session = get_session()
async with session.create_client("rds") as client:  # (1)
    waiter: TenantDatabaseDeletedWaiter = client.get_waiter("tenant_database_deleted")  # (2)
    await waiter.wait()
```

1. client: [RDSClient](./client.md)
2. waiter: [TenantDatabaseDeletedWaiter](./waiters.md#tenantdatabasedeletedwaiter)


### wait

Type annotations and code completion for `#!python TenantDatabaseDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DBInstanceIdentifier: str = ...,
    TenantDBName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    Marker: str = ...,
    MaxRecords: int = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeTenantDatabasesMessageTenantDatabaseDeletedWaitTypeDef = {  # (1)
    "DBInstanceIdentifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeTenantDatabasesMessageTenantDatabaseDeletedWaitTypeDef](./type_defs.md#describetenantdatabasesmessagetenantdatabasedeletedwaittypedef) 
