<a id="docdbclient-for-aiobotocore-docdb-module"></a>

# DocDBClient for aiobotocore DocDB module

> [Index](..) > [DocDB](.) > DocDBClient

Auto-generated documentation for
[DocDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
type annotations stubs module
[types-aiobotocore-docdb](https://pypi.org/project/types-aiobotocore-docdb/).

- [DocDBClient for aiobotocore DocDB module](#docdbclient-for-aiobotocore-docdb-module)
  - [DocDBClient](#docdbclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [add_source_identifier_to_subscription](#add_source_identifier_to_subscription)
    - [add_tags_to_resource](#add_tags_to_resource)
    - [apply_pending_maintenance_action](#apply_pending_maintenance_action)
    - [can_paginate](#can_paginate)
    - [copy_db_cluster_parameter_group](#copy_db_cluster_parameter_group)
    - [copy_db_cluster_snapshot](#copy_db_cluster_snapshot)
    - [create_db_cluster](#create_db_cluster)
    - [create_db_cluster_parameter_group](#create_db_cluster_parameter_group)
    - [create_db_cluster_snapshot](#create_db_cluster_snapshot)
    - [create_db_instance](#create_db_instance)
    - [create_db_subnet_group](#create_db_subnet_group)
    - [create_event_subscription](#create_event_subscription)
    - [create_global_cluster](#create_global_cluster)
    - [delete_db_cluster](#delete_db_cluster)
    - [delete_db_cluster_parameter_group](#delete_db_cluster_parameter_group)
    - [delete_db_cluster_snapshot](#delete_db_cluster_snapshot)
    - [delete_db_instance](#delete_db_instance)
    - [delete_db_subnet_group](#delete_db_subnet_group)
    - [delete_event_subscription](#delete_event_subscription)
    - [delete_global_cluster](#delete_global_cluster)
    - [describe_certificates](#describe_certificates)
    - [describe_db_cluster_parameter_groups](#describe_db_cluster_parameter_groups)
    - [describe_db_cluster_parameters](#describe_db_cluster_parameters)
    - [describe_db_cluster_snapshot_attributes](#describe_db_cluster_snapshot_attributes)
    - [describe_db_cluster_snapshots](#describe_db_cluster_snapshots)
    - [describe_db_clusters](#describe_db_clusters)
    - [describe_db_engine_versions](#describe_db_engine_versions)
    - [describe_db_instances](#describe_db_instances)
    - [describe_db_subnet_groups](#describe_db_subnet_groups)
    - [describe_engine_default_cluster_parameters](#describe_engine_default_cluster_parameters)
    - [describe_event_categories](#describe_event_categories)
    - [describe_event_subscriptions](#describe_event_subscriptions)
    - [describe_events](#describe_events)
    - [describe_global_clusters](#describe_global_clusters)
    - [describe_orderable_db_instance_options](#describe_orderable_db_instance_options)
    - [describe_pending_maintenance_actions](#describe_pending_maintenance_actions)
    - [failover_db_cluster](#failover_db_cluster)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [modify_db_cluster](#modify_db_cluster)
    - [modify_db_cluster_parameter_group](#modify_db_cluster_parameter_group)
    - [modify_db_cluster_snapshot_attribute](#modify_db_cluster_snapshot_attribute)
    - [modify_db_instance](#modify_db_instance)
    - [modify_db_subnet_group](#modify_db_subnet_group)
    - [modify_event_subscription](#modify_event_subscription)
    - [modify_global_cluster](#modify_global_cluster)
    - [reboot_db_instance](#reboot_db_instance)
    - [remove_from_global_cluster](#remove_from_global_cluster)
    - [remove_source_identifier_from_subscription](#remove_source_identifier_from_subscription)
    - [remove_tags_from_resource](#remove_tags_from_resource)
    - [reset_db_cluster_parameter_group](#reset_db_cluster_parameter_group)
    - [restore_db_cluster_from_snapshot](#restore_db_cluster_from_snapshot)
    - [restore_db_cluster_to_point_in_time](#restore_db_cluster_to_point_in_time)
    - [start_db_cluster](#start_db_cluster)
    - [stop_db_cluster](#stop_db_cluster)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="docdbclient"></a>

## DocDBClient

Type annotations for `session.create_client("docdb")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_docdb.client import DocDBClient

session = get_session()
async with session.create_client("docdb") as client:
    client: DocDBClient
```

Boto3 documentation:
[DocDB.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_docdb.client import Exceptions

def handle_error(exc: Exceptions.AuthorizationNotFoundFault) -> None:
    ...
```

Exceptions:

- `Exceptions.AuthorizationNotFoundFault`
- `Exceptions.CertificateNotFoundFault`
- `Exceptions.ClientError`
- `Exceptions.DBClusterAlreadyExistsFault`
- `Exceptions.DBClusterNotFoundFault`
- `Exceptions.DBClusterParameterGroupNotFoundFault`
- `Exceptions.DBClusterQuotaExceededFault`
- `Exceptions.DBClusterSnapshotAlreadyExistsFault`
- `Exceptions.DBClusterSnapshotNotFoundFault`
- `Exceptions.DBInstanceAlreadyExistsFault`
- `Exceptions.DBInstanceNotFoundFault`
- `Exceptions.DBParameterGroupAlreadyExistsFault`
- `Exceptions.DBParameterGroupNotFoundFault`
- `Exceptions.DBParameterGroupQuotaExceededFault`
- `Exceptions.DBSecurityGroupNotFoundFault`
- `Exceptions.DBSnapshotAlreadyExistsFault`
- `Exceptions.DBSnapshotNotFoundFault`
- `Exceptions.DBSubnetGroupAlreadyExistsFault`
- `Exceptions.DBSubnetGroupDoesNotCoverEnoughAZs`
- `Exceptions.DBSubnetGroupNotFoundFault`
- `Exceptions.DBSubnetGroupQuotaExceededFault`
- `Exceptions.DBSubnetQuotaExceededFault`
- `Exceptions.DBUpgradeDependencyFailureFault`
- `Exceptions.EventSubscriptionQuotaExceededFault`
- `Exceptions.GlobalClusterAlreadyExistsFault`
- `Exceptions.GlobalClusterNotFoundFault`
- `Exceptions.GlobalClusterQuotaExceededFault`
- `Exceptions.InstanceQuotaExceededFault`
- `Exceptions.InsufficientDBClusterCapacityFault`
- `Exceptions.InsufficientDBInstanceCapacityFault`
- `Exceptions.InsufficientStorageClusterCapacityFault`
- `Exceptions.InvalidDBClusterSnapshotStateFault`
- `Exceptions.InvalidDBClusterStateFault`
- `Exceptions.InvalidDBInstanceStateFault`
- `Exceptions.InvalidDBParameterGroupStateFault`
- `Exceptions.InvalidDBSecurityGroupStateFault`
- `Exceptions.InvalidDBSnapshotStateFault`
- `Exceptions.InvalidDBSubnetGroupStateFault`
- `Exceptions.InvalidDBSubnetStateFault`
- `Exceptions.InvalidEventSubscriptionStateFault`
- `Exceptions.InvalidGlobalClusterStateFault`
- `Exceptions.InvalidRestoreFault`
- `Exceptions.InvalidSubnet`
- `Exceptions.InvalidVPCNetworkStateFault`
- `Exceptions.KMSKeyNotAccessibleFault`
- `Exceptions.ResourceNotFoundFault`
- `Exceptions.SNSInvalidTopicFault`
- `Exceptions.SNSNoAuthorizationFault`
- `Exceptions.SNSTopicArnNotFoundFault`
- `Exceptions.SharedSnapshotQuotaExceededFault`
- `Exceptions.SnapshotQuotaExceededFault`
- `Exceptions.SourceNotFoundFault`
- `Exceptions.StorageQuotaExceededFault`
- `Exceptions.StorageTypeNotSupportedFault`
- `Exceptions.SubnetAlreadyInUse`
- `Exceptions.SubscriptionAlreadyExistFault`
- `Exceptions.SubscriptionCategoryNotFoundFault`
- `Exceptions.SubscriptionNotFoundFault`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

DocDBClient exceptions.

Type annotations for `session.create_client("docdb").exceptions` method.

Boto3 documentation:
[DocDB.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="add_source_identifier_to_subscription"></a>

### add_source_identifier_to_subscription

Adds a source identifier to an existing event notification subscription.

Type annotations for
`session.create_client("docdb").add_source_identifier_to_subscription` method.

Boto3 documentation:
[DocDB.Client.add_source_identifier_to_subscription](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.add_source_identifier_to_subscription)

Asynchronous method. Use `await add_source_identifier_to_subscription(...)` for
a synchronous call.

Arguments mapping described in
[AddSourceIdentifierToSubscriptionMessageRequestTypeDef](./type_defs.md#addsourceidentifiertosubscriptionmessagerequesttypedef).

Keyword-only arguments:

- `SubscriptionName`: `str` *(required)*
- `SourceIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[AddSourceIdentifierToSubscriptionResultTypeDef](./type_defs.md#addsourceidentifiertosubscriptionresulttypedef).

<a id="add_tags_to_resource"></a>

### add_tags_to_resource

Adds metadata tags to an Amazon DocumentDB resource.

Type annotations for `session.create_client("docdb").add_tags_to_resource`
method.

Boto3 documentation:
[DocDB.Client.add_tags_to_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.add_tags_to_resource)

Asynchronous method. Use `await add_tags_to_resource(...)` for a synchronous
call.

Arguments mapping described in
[AddTagsToResourceMessageRequestTypeDef](./type_defs.md#addtagstoresourcemessagerequesttypedef).

Keyword-only arguments:

- `ResourceName`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

<a id="apply_pending_maintenance_action"></a>

### apply_pending_maintenance_action

Applies a pending maintenance action to a resource (for example, to an Amazon
DocumentDB instance).

Type annotations for
`session.create_client("docdb").apply_pending_maintenance_action` method.

Boto3 documentation:
[DocDB.Client.apply_pending_maintenance_action](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.apply_pending_maintenance_action)

Asynchronous method. Use `await apply_pending_maintenance_action(...)` for a
synchronous call.

Arguments mapping described in
[ApplyPendingMaintenanceActionMessageRequestTypeDef](./type_defs.md#applypendingmaintenanceactionmessagerequesttypedef).

Keyword-only arguments:

- `ResourceIdentifier`: `str` *(required)*
- `ApplyAction`: `str` *(required)*
- `OptInType`: `str` *(required)*

Returns a `Coroutine` for
[ApplyPendingMaintenanceActionResultTypeDef](./type_defs.md#applypendingmaintenanceactionresulttypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("docdb").can_paginate` method.

Boto3 documentation:
[DocDB.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="copy_db_cluster_parameter_group"></a>

### copy_db_cluster_parameter_group

Copies the specified cluster parameter group.

Type annotations for
`session.create_client("docdb").copy_db_cluster_parameter_group` method.

Boto3 documentation:
[DocDB.Client.copy_db_cluster_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.copy_db_cluster_parameter_group)

Asynchronous method. Use `await copy_db_cluster_parameter_group(...)` for a
synchronous call.

Arguments mapping described in
[CopyDBClusterParameterGroupMessageRequestTypeDef](./type_defs.md#copydbclusterparametergroupmessagerequesttypedef).

Keyword-only arguments:

- `SourceDBClusterParameterGroupIdentifier`: `str` *(required)*
- `TargetDBClusterParameterGroupIdentifier`: `str` *(required)*
- `TargetDBClusterParameterGroupDescription`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CopyDBClusterParameterGroupResultTypeDef](./type_defs.md#copydbclusterparametergroupresulttypedef).

<a id="copy_db_cluster_snapshot"></a>

### copy_db_cluster_snapshot

Copies a snapshot of a cluster.

Type annotations for `session.create_client("docdb").copy_db_cluster_snapshot`
method.

Boto3 documentation:
[DocDB.Client.copy_db_cluster_snapshot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.copy_db_cluster_snapshot)

Asynchronous method. Use `await copy_db_cluster_snapshot(...)` for a
synchronous call.

Arguments mapping described in
[CopyDBClusterSnapshotMessageRequestTypeDef](./type_defs.md#copydbclustersnapshotmessagerequesttypedef).

Keyword-only arguments:

- `SourceDBClusterSnapshotIdentifier`: `str` *(required)*
- `TargetDBClusterSnapshotIdentifier`: `str` *(required)*
- `KmsKeyId`: `str`
- `PreSignedUrl`: `str`
- `CopyTags`: `bool`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `SourceRegion`: `str`

Returns a `Coroutine` for
[CopyDBClusterSnapshotResultTypeDef](./type_defs.md#copydbclustersnapshotresulttypedef).

<a id="create_db_cluster"></a>

### create_db_cluster

Creates a new Amazon DocumentDB cluster.

Type annotations for `session.create_client("docdb").create_db_cluster` method.

Boto3 documentation:
[DocDB.Client.create_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_cluster)

Asynchronous method. Use `await create_db_cluster(...)` for a synchronous call.

Arguments mapping described in
[CreateDBClusterMessageRequestTypeDef](./type_defs.md#createdbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*
- `Engine`: `str` *(required)*
- `AvailabilityZones`: `Sequence`\[`str`\]
- `BackupRetentionPeriod`: `int`
- `DBClusterParameterGroupName`: `str`
- `VpcSecurityGroupIds`: `Sequence`\[`str`\]
- `DBSubnetGroupName`: `str`
- `EngineVersion`: `str`
- `Port`: `int`
- `MasterUsername`: `str`
- `MasterUserPassword`: `str`
- `PreferredBackupWindow`: `str`
- `PreferredMaintenanceWindow`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `StorageEncrypted`: `bool`
- `KmsKeyId`: `str`
- `PreSignedUrl`: `str`
- `EnableCloudwatchLogsExports`: `Sequence`\[`str`\]
- `DeletionProtection`: `bool`
- `GlobalClusterIdentifier`: `str`
- `SourceRegion`: `str`

Returns a `Coroutine` for
[CreateDBClusterResultTypeDef](./type_defs.md#createdbclusterresulttypedef).

<a id="create_db_cluster_parameter_group"></a>

### create_db_cluster_parameter_group

Creates a new cluster parameter group.

Type annotations for
`session.create_client("docdb").create_db_cluster_parameter_group` method.

Boto3 documentation:
[DocDB.Client.create_db_cluster_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_cluster_parameter_group)

Asynchronous method. Use `await create_db_cluster_parameter_group(...)` for a
synchronous call.

Arguments mapping described in
[CreateDBClusterParameterGroupMessageRequestTypeDef](./type_defs.md#createdbclusterparametergroupmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterParameterGroupName`: `str` *(required)*
- `DBParameterGroupFamily`: `str` *(required)*
- `Description`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateDBClusterParameterGroupResultTypeDef](./type_defs.md#createdbclusterparametergroupresulttypedef).

<a id="create_db_cluster_snapshot"></a>

### create_db_cluster_snapshot

Creates a snapshot of a cluster.

Type annotations for
`session.create_client("docdb").create_db_cluster_snapshot` method.

Boto3 documentation:
[DocDB.Client.create_db_cluster_snapshot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_cluster_snapshot)

Asynchronous method. Use `await create_db_cluster_snapshot(...)` for a
synchronous call.

Arguments mapping described in
[CreateDBClusterSnapshotMessageRequestTypeDef](./type_defs.md#createdbclustersnapshotmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterSnapshotIdentifier`: `str` *(required)*
- `DBClusterIdentifier`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateDBClusterSnapshotResultTypeDef](./type_defs.md#createdbclustersnapshotresulttypedef).

<a id="create_db_instance"></a>

### create_db_instance

Creates a new instance.

Type annotations for `session.create_client("docdb").create_db_instance`
method.

Boto3 documentation:
[DocDB.Client.create_db_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_instance)

Asynchronous method. Use `await create_db_instance(...)` for a synchronous
call.

Arguments mapping described in
[CreateDBInstanceMessageRequestTypeDef](./type_defs.md#createdbinstancemessagerequesttypedef).

Keyword-only arguments:

- `DBInstanceIdentifier`: `str` *(required)*
- `DBInstanceClass`: `str` *(required)*
- `Engine`: `str` *(required)*
- `DBClusterIdentifier`: `str` *(required)*
- `AvailabilityZone`: `str`
- `PreferredMaintenanceWindow`: `str`
- `AutoMinorVersionUpgrade`: `bool`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `PromotionTier`: `int`

Returns a `Coroutine` for
[CreateDBInstanceResultTypeDef](./type_defs.md#createdbinstanceresulttypedef).

<a id="create_db_subnet_group"></a>

### create_db_subnet_group

Creates a new subnet group.

Type annotations for `session.create_client("docdb").create_db_subnet_group`
method.

Boto3 documentation:
[DocDB.Client.create_db_subnet_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_subnet_group)

Asynchronous method. Use `await create_db_subnet_group(...)` for a synchronous
call.

Arguments mapping described in
[CreateDBSubnetGroupMessageRequestTypeDef](./type_defs.md#createdbsubnetgroupmessagerequesttypedef).

Keyword-only arguments:

- `DBSubnetGroupName`: `str` *(required)*
- `DBSubnetGroupDescription`: `str` *(required)*
- `SubnetIds`: `Sequence`\[`str`\] *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateDBSubnetGroupResultTypeDef](./type_defs.md#createdbsubnetgroupresulttypedef).

<a id="create_event_subscription"></a>

### create_event_subscription

Creates an Amazon DocumentDB event notification subscription.

Type annotations for `session.create_client("docdb").create_event_subscription`
method.

Boto3 documentation:
[DocDB.Client.create_event_subscription](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_event_subscription)

Asynchronous method. Use `await create_event_subscription(...)` for a
synchronous call.

Arguments mapping described in
[CreateEventSubscriptionMessageRequestTypeDef](./type_defs.md#createeventsubscriptionmessagerequesttypedef).

Keyword-only arguments:

- `SubscriptionName`: `str` *(required)*
- `SnsTopicArn`: `str` *(required)*
- `SourceType`: `str`
- `EventCategories`: `Sequence`\[`str`\]
- `SourceIds`: `Sequence`\[`str`\]
- `Enabled`: `bool`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateEventSubscriptionResultTypeDef](./type_defs.md#createeventsubscriptionresulttypedef).

<a id="create_global_cluster"></a>

### create_global_cluster

Creates an Amazon DocumentDB global cluster that can span multiple multiple
Regions.

Type annotations for `session.create_client("docdb").create_global_cluster`
method.

Boto3 documentation:
[DocDB.Client.create_global_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_global_cluster)

Asynchronous method. Use `await create_global_cluster(...)` for a synchronous
call.

Arguments mapping described in
[CreateGlobalClusterMessageRequestTypeDef](./type_defs.md#createglobalclustermessagerequesttypedef).

Keyword-only arguments:

- `GlobalClusterIdentifier`: `str` *(required)*
- `SourceDBClusterIdentifier`: `str`
- `Engine`: `str`
- `EngineVersion`: `str`
- `DeletionProtection`: `bool`
- `DatabaseName`: `str`
- `StorageEncrypted`: `bool`

Returns a `Coroutine` for
[CreateGlobalClusterResultTypeDef](./type_defs.md#createglobalclusterresulttypedef).

<a id="delete_db_cluster"></a>

### delete_db_cluster

Deletes a previously provisioned cluster.

Type annotations for `session.create_client("docdb").delete_db_cluster` method.

Boto3 documentation:
[DocDB.Client.delete_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.delete_db_cluster)

Asynchronous method. Use `await delete_db_cluster(...)` for a synchronous call.

Arguments mapping described in
[DeleteDBClusterMessageRequestTypeDef](./type_defs.md#deletedbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*
- `SkipFinalSnapshot`: `bool`
- `FinalDBSnapshotIdentifier`: `str`

Returns a `Coroutine` for
[DeleteDBClusterResultTypeDef](./type_defs.md#deletedbclusterresulttypedef).

<a id="delete_db_cluster_parameter_group"></a>

### delete_db_cluster_parameter_group

Deletes a specified cluster parameter group.

Type annotations for
`session.create_client("docdb").delete_db_cluster_parameter_group` method.

Boto3 documentation:
[DocDB.Client.delete_db_cluster_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.delete_db_cluster_parameter_group)

Asynchronous method. Use `await delete_db_cluster_parameter_group(...)` for a
synchronous call.

Arguments mapping described in
[DeleteDBClusterParameterGroupMessageRequestTypeDef](./type_defs.md#deletedbclusterparametergroupmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterParameterGroupName`: `str` *(required)*

<a id="delete_db_cluster_snapshot"></a>

### delete_db_cluster_snapshot

Deletes a cluster snapshot.

Type annotations for
`session.create_client("docdb").delete_db_cluster_snapshot` method.

Boto3 documentation:
[DocDB.Client.delete_db_cluster_snapshot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.delete_db_cluster_snapshot)

Asynchronous method. Use `await delete_db_cluster_snapshot(...)` for a
synchronous call.

Arguments mapping described in
[DeleteDBClusterSnapshotMessageRequestTypeDef](./type_defs.md#deletedbclustersnapshotmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterSnapshotIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[DeleteDBClusterSnapshotResultTypeDef](./type_defs.md#deletedbclustersnapshotresulttypedef).

<a id="delete_db_instance"></a>

### delete_db_instance

Deletes a previously provisioned instance.

Type annotations for `session.create_client("docdb").delete_db_instance`
method.

Boto3 documentation:
[DocDB.Client.delete_db_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.delete_db_instance)

Asynchronous method. Use `await delete_db_instance(...)` for a synchronous
call.

Arguments mapping described in
[DeleteDBInstanceMessageRequestTypeDef](./type_defs.md#deletedbinstancemessagerequesttypedef).

Keyword-only arguments:

- `DBInstanceIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[DeleteDBInstanceResultTypeDef](./type_defs.md#deletedbinstanceresulttypedef).

<a id="delete_db_subnet_group"></a>

### delete_db_subnet_group

Deletes a subnet group.

Type annotations for `session.create_client("docdb").delete_db_subnet_group`
method.

Boto3 documentation:
[DocDB.Client.delete_db_subnet_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.delete_db_subnet_group)

Asynchronous method. Use `await delete_db_subnet_group(...)` for a synchronous
call.

Arguments mapping described in
[DeleteDBSubnetGroupMessageRequestTypeDef](./type_defs.md#deletedbsubnetgroupmessagerequesttypedef).

Keyword-only arguments:

- `DBSubnetGroupName`: `str` *(required)*

<a id="delete_event_subscription"></a>

### delete_event_subscription

Deletes an Amazon DocumentDB event notification subscription.

Type annotations for `session.create_client("docdb").delete_event_subscription`
method.

Boto3 documentation:
[DocDB.Client.delete_event_subscription](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.delete_event_subscription)

Asynchronous method. Use `await delete_event_subscription(...)` for a
synchronous call.

Arguments mapping described in
[DeleteEventSubscriptionMessageRequestTypeDef](./type_defs.md#deleteeventsubscriptionmessagerequesttypedef).

Keyword-only arguments:

- `SubscriptionName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteEventSubscriptionResultTypeDef](./type_defs.md#deleteeventsubscriptionresulttypedef).

<a id="delete_global_cluster"></a>

### delete_global_cluster

Deletes a global cluster.

Type annotations for `session.create_client("docdb").delete_global_cluster`
method.

Boto3 documentation:
[DocDB.Client.delete_global_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.delete_global_cluster)

Asynchronous method. Use `await delete_global_cluster(...)` for a synchronous
call.

Arguments mapping described in
[DeleteGlobalClusterMessageRequestTypeDef](./type_defs.md#deleteglobalclustermessagerequesttypedef).

Keyword-only arguments:

- `GlobalClusterIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[DeleteGlobalClusterResultTypeDef](./type_defs.md#deleteglobalclusterresulttypedef).

<a id="describe_certificates"></a>

### describe_certificates

Returns a list of certificate authority (CA) certificates provided by Amazon
DocumentDB for this account.

Type annotations for `session.create_client("docdb").describe_certificates`
method.

Boto3 documentation:
[DocDB.Client.describe_certificates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_certificates)

Asynchronous method. Use `await describe_certificates(...)` for a synchronous
call.

Arguments mapping described in
[DescribeCertificatesMessageRequestTypeDef](./type_defs.md#describecertificatesmessagerequesttypedef).

Keyword-only arguments:

- `CertificateIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[CertificateMessageTypeDef](./type_defs.md#certificatemessagetypedef).

<a id="describe_db_cluster_parameter_groups"></a>

### describe_db_cluster_parameter_groups

Returns a list of `DBClusterParameterGroup` descriptions.

Type annotations for
`session.create_client("docdb").describe_db_cluster_parameter_groups` method.

Boto3 documentation:
[DocDB.Client.describe_db_cluster_parameter_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_cluster_parameter_groups)

Asynchronous method. Use `await describe_db_cluster_parameter_groups(...)` for
a synchronous call.

Arguments mapping described in
[DescribeDBClusterParameterGroupsMessageRequestTypeDef](./type_defs.md#describedbclusterparametergroupsmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterParameterGroupName`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[DBClusterParameterGroupsMessageTypeDef](./type_defs.md#dbclusterparametergroupsmessagetypedef).

<a id="describe_db_cluster_parameters"></a>

### describe_db_cluster_parameters

Returns the detailed parameter list for a particular cluster parameter group.

Type annotations for
`session.create_client("docdb").describe_db_cluster_parameters` method.

Boto3 documentation:
[DocDB.Client.describe_db_cluster_parameters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_cluster_parameters)

Asynchronous method. Use `await describe_db_cluster_parameters(...)` for a
synchronous call.

Arguments mapping described in
[DescribeDBClusterParametersMessageRequestTypeDef](./type_defs.md#describedbclusterparametersmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterParameterGroupName`: `str` *(required)*
- `Source`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[DBClusterParameterGroupDetailsTypeDef](./type_defs.md#dbclusterparametergroupdetailstypedef).

<a id="describe_db_cluster_snapshot_attributes"></a>

### describe_db_cluster_snapshot_attributes

Returns a list of cluster snapshot attribute names and values for a manual DB
cluster snapshot.

Type annotations for
`session.create_client("docdb").describe_db_cluster_snapshot_attributes`
method.

Boto3 documentation:
[DocDB.Client.describe_db_cluster_snapshot_attributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_cluster_snapshot_attributes)

Asynchronous method. Use `await describe_db_cluster_snapshot_attributes(...)`
for a synchronous call.

Arguments mapping described in
[DescribeDBClusterSnapshotAttributesMessageRequestTypeDef](./type_defs.md#describedbclustersnapshotattributesmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterSnapshotIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDBClusterSnapshotAttributesResultTypeDef](./type_defs.md#describedbclustersnapshotattributesresulttypedef).

<a id="describe_db_cluster_snapshots"></a>

### describe_db_cluster_snapshots

Returns information about cluster snapshots.

Type annotations for
`session.create_client("docdb").describe_db_cluster_snapshots` method.

Boto3 documentation:
[DocDB.Client.describe_db_cluster_snapshots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_cluster_snapshots)

Asynchronous method. Use `await describe_db_cluster_snapshots(...)` for a
synchronous call.

Arguments mapping described in
[DescribeDBClusterSnapshotsMessageRequestTypeDef](./type_defs.md#describedbclustersnapshotsmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str`
- `DBClusterSnapshotIdentifier`: `str`
- `SnapshotType`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`
- `IncludeShared`: `bool`
- `IncludePublic`: `bool`

Returns a `Coroutine` for
[DBClusterSnapshotMessageTypeDef](./type_defs.md#dbclustersnapshotmessagetypedef).

<a id="describe_db_clusters"></a>

### describe_db_clusters

Returns information about provisioned Amazon DocumentDB clusters.

Type annotations for `session.create_client("docdb").describe_db_clusters`
method.

Boto3 documentation:
[DocDB.Client.describe_db_clusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_clusters)

Asynchronous method. Use `await describe_db_clusters(...)` for a synchronous
call.

Arguments mapping described in
[DescribeDBClustersMessageRequestTypeDef](./type_defs.md#describedbclustersmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[DBClusterMessageTypeDef](./type_defs.md#dbclustermessagetypedef).

<a id="describe_db_engine_versions"></a>

### describe_db_engine_versions

Returns a list of the available engines.

Type annotations for
`session.create_client("docdb").describe_db_engine_versions` method.

Boto3 documentation:
[DocDB.Client.describe_db_engine_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_engine_versions)

Asynchronous method. Use `await describe_db_engine_versions(...)` for a
synchronous call.

Arguments mapping described in
[DescribeDBEngineVersionsMessageRequestTypeDef](./type_defs.md#describedbengineversionsmessagerequesttypedef).

Keyword-only arguments:

- `Engine`: `str`
- `EngineVersion`: `str`
- `DBParameterGroupFamily`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`
- `DefaultOnly`: `bool`
- `ListSupportedCharacterSets`: `bool`
- `ListSupportedTimezones`: `bool`

Returns a `Coroutine` for
[DBEngineVersionMessageTypeDef](./type_defs.md#dbengineversionmessagetypedef).

<a id="describe_db_instances"></a>

### describe_db_instances

Returns information about provisioned Amazon DocumentDB instances.

Type annotations for `session.create_client("docdb").describe_db_instances`
method.

Boto3 documentation:
[DocDB.Client.describe_db_instances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_instances)

Asynchronous method. Use `await describe_db_instances(...)` for a synchronous
call.

Arguments mapping described in
[DescribeDBInstancesMessageRequestTypeDef](./type_defs.md#describedbinstancesmessagerequesttypedef).

Keyword-only arguments:

- `DBInstanceIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[DBInstanceMessageTypeDef](./type_defs.md#dbinstancemessagetypedef).

<a id="describe_db_subnet_groups"></a>

### describe_db_subnet_groups

Returns a list of `DBSubnetGroup` descriptions.

Type annotations for `session.create_client("docdb").describe_db_subnet_groups`
method.

Boto3 documentation:
[DocDB.Client.describe_db_subnet_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_subnet_groups)

Asynchronous method. Use `await describe_db_subnet_groups(...)` for a
synchronous call.

Arguments mapping described in
[DescribeDBSubnetGroupsMessageRequestTypeDef](./type_defs.md#describedbsubnetgroupsmessagerequesttypedef).

Keyword-only arguments:

- `DBSubnetGroupName`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[DBSubnetGroupMessageTypeDef](./type_defs.md#dbsubnetgroupmessagetypedef).

<a id="describe_engine_default_cluster_parameters"></a>

### describe_engine_default_cluster_parameters

Returns the default engine and system parameter information for the cluster
database engine.

Type annotations for
`session.create_client("docdb").describe_engine_default_cluster_parameters`
method.

Boto3 documentation:
[DocDB.Client.describe_engine_default_cluster_parameters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_engine_default_cluster_parameters)

Asynchronous method. Use
`await describe_engine_default_cluster_parameters(...)` for a synchronous call.

Arguments mapping described in
[DescribeEngineDefaultClusterParametersMessageRequestTypeDef](./type_defs.md#describeenginedefaultclusterparametersmessagerequesttypedef).

Keyword-only arguments:

- `DBParameterGroupFamily`: `str` *(required)*
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[DescribeEngineDefaultClusterParametersResultTypeDef](./type_defs.md#describeenginedefaultclusterparametersresulttypedef).

<a id="describe_event_categories"></a>

### describe_event_categories

Displays a list of categories for all event source types, or, if specified, for
a specified source type.

Type annotations for `session.create_client("docdb").describe_event_categories`
method.

Boto3 documentation:
[DocDB.Client.describe_event_categories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_event_categories)

Asynchronous method. Use `await describe_event_categories(...)` for a
synchronous call.

Arguments mapping described in
[DescribeEventCategoriesMessageRequestTypeDef](./type_defs.md#describeeventcategoriesmessagerequesttypedef).

Keyword-only arguments:

- `SourceType`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[EventCategoriesMessageTypeDef](./type_defs.md#eventcategoriesmessagetypedef).

<a id="describe_event_subscriptions"></a>

### describe_event_subscriptions

Lists all the subscription descriptions for a customer account.

Type annotations for
`session.create_client("docdb").describe_event_subscriptions` method.

Boto3 documentation:
[DocDB.Client.describe_event_subscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_event_subscriptions)

Asynchronous method. Use `await describe_event_subscriptions(...)` for a
synchronous call.

Arguments mapping described in
[DescribeEventSubscriptionsMessageRequestTypeDef](./type_defs.md#describeeventsubscriptionsmessagerequesttypedef).

Keyword-only arguments:

- `SubscriptionName`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[EventSubscriptionsMessageTypeDef](./type_defs.md#eventsubscriptionsmessagetypedef).

<a id="describe_events"></a>

### describe_events

Returns events related to instances, security groups, snapshots, and DB
parameter groups for the past 14 days.

Type annotations for `session.create_client("docdb").describe_events` method.

Boto3 documentation:
[DocDB.Client.describe_events](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_events)

Asynchronous method. Use `await describe_events(...)` for a synchronous call.

Arguments mapping described in
[DescribeEventsMessageRequestTypeDef](./type_defs.md#describeeventsmessagerequesttypedef).

Keyword-only arguments:

- `SourceIdentifier`: `str`
- `SourceType`: [SourceTypeType](./literals.md#sourcetypetype)
- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `Duration`: `int`
- `EventCategories`: `Sequence`\[`str`\]
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[EventsMessageTypeDef](./type_defs.md#eventsmessagetypedef).

<a id="describe_global_clusters"></a>

### describe_global_clusters

Returns information about Amazon DocumentDB global clusters.

Type annotations for `session.create_client("docdb").describe_global_clusters`
method.

Boto3 documentation:
[DocDB.Client.describe_global_clusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_global_clusters)

Asynchronous method. Use `await describe_global_clusters(...)` for a
synchronous call.

Arguments mapping described in
[DescribeGlobalClustersMessageRequestTypeDef](./type_defs.md#describeglobalclustersmessagerequesttypedef).

Keyword-only arguments:

- `GlobalClusterIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[GlobalClustersMessageTypeDef](./type_defs.md#globalclustersmessagetypedef).

<a id="describe_orderable_db_instance_options"></a>

### describe_orderable_db_instance_options

Returns a list of orderable instance options for the specified engine.

Type annotations for
`session.create_client("docdb").describe_orderable_db_instance_options` method.

Boto3 documentation:
[DocDB.Client.describe_orderable_db_instance_options](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_orderable_db_instance_options)

Asynchronous method. Use `await describe_orderable_db_instance_options(...)`
for a synchronous call.

Arguments mapping described in
[DescribeOrderableDBInstanceOptionsMessageRequestTypeDef](./type_defs.md#describeorderabledbinstanceoptionsmessagerequesttypedef).

Keyword-only arguments:

- `Engine`: `str` *(required)*
- `EngineVersion`: `str`
- `DBInstanceClass`: `str`
- `LicenseModel`: `str`
- `Vpc`: `bool`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[OrderableDBInstanceOptionsMessageTypeDef](./type_defs.md#orderabledbinstanceoptionsmessagetypedef).

<a id="describe_pending_maintenance_actions"></a>

### describe_pending_maintenance_actions

Returns a list of resources (for example, instances) that have at least one
pending maintenance action.

Type annotations for
`session.create_client("docdb").describe_pending_maintenance_actions` method.

Boto3 documentation:
[DocDB.Client.describe_pending_maintenance_actions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_pending_maintenance_actions)

Asynchronous method. Use `await describe_pending_maintenance_actions(...)` for
a synchronous call.

Arguments mapping described in
[DescribePendingMaintenanceActionsMessageRequestTypeDef](./type_defs.md#describependingmaintenanceactionsmessagerequesttypedef).

Keyword-only arguments:

- `ResourceIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `Marker`: `str`
- `MaxRecords`: `int`

Returns a `Coroutine` for
[PendingMaintenanceActionsMessageTypeDef](./type_defs.md#pendingmaintenanceactionsmessagetypedef).

<a id="failover_db_cluster"></a>

### failover_db_cluster

Forces a failover for a cluster.

Type annotations for `session.create_client("docdb").failover_db_cluster`
method.

Boto3 documentation:
[DocDB.Client.failover_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.failover_db_cluster)

Asynchronous method. Use `await failover_db_cluster(...)` for a synchronous
call.

Arguments mapping described in
[FailoverDBClusterMessageRequestTypeDef](./type_defs.md#failoverdbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str`
- `TargetDBInstanceIdentifier`: `str`

Returns a `Coroutine` for
[FailoverDBClusterResultTypeDef](./type_defs.md#failoverdbclusterresulttypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("docdb").generate_presigned_url`
method.

Boto3 documentation:
[DocDB.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Lists all tags on an Amazon DocumentDB resource.

Type annotations for `session.create_client("docdb").list_tags_for_resource`
method.

Boto3 documentation:
[DocDB.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceMessageRequestTypeDef](./type_defs.md#listtagsforresourcemessagerequesttypedef).

Keyword-only arguments:

- `ResourceName`: `str` *(required)*
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[TagListMessageTypeDef](./type_defs.md#taglistmessagetypedef).

<a id="modify_db_cluster"></a>

### modify_db_cluster

Modifies a setting for an Amazon DocumentDB cluster.

Type annotations for `session.create_client("docdb").modify_db_cluster` method.

Boto3 documentation:
[DocDB.Client.modify_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_cluster)

Asynchronous method. Use `await modify_db_cluster(...)` for a synchronous call.

Arguments mapping described in
[ModifyDBClusterMessageRequestTypeDef](./type_defs.md#modifydbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*
- `NewDBClusterIdentifier`: `str`
- `ApplyImmediately`: `bool`
- `BackupRetentionPeriod`: `int`
- `DBClusterParameterGroupName`: `str`
- `VpcSecurityGroupIds`: `Sequence`\[`str`\]
- `Port`: `int`
- `MasterUserPassword`: `str`
- `PreferredBackupWindow`: `str`
- `PreferredMaintenanceWindow`: `str`
- `CloudwatchLogsExportConfiguration`:
  [CloudwatchLogsExportConfigurationTypeDef](./type_defs.md#cloudwatchlogsexportconfigurationtypedef)
- `EngineVersion`: `str`
- `DeletionProtection`: `bool`

Returns a `Coroutine` for
[ModifyDBClusterResultTypeDef](./type_defs.md#modifydbclusterresulttypedef).

<a id="modify_db_cluster_parameter_group"></a>

### modify_db_cluster_parameter_group

Modifies the parameters of a cluster parameter group.

Type annotations for
`session.create_client("docdb").modify_db_cluster_parameter_group` method.

Boto3 documentation:
[DocDB.Client.modify_db_cluster_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_cluster_parameter_group)

Asynchronous method. Use `await modify_db_cluster_parameter_group(...)` for a
synchronous call.

Arguments mapping described in
[ModifyDBClusterParameterGroupMessageRequestTypeDef](./type_defs.md#modifydbclusterparametergroupmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterParameterGroupName`: `str` *(required)*
- `Parameters`:
  `Sequence`\[[ParameterTypeDef](./type_defs.md#parametertypedef)\]
  *(required)*

Returns a `Coroutine` for
[DBClusterParameterGroupNameMessageTypeDef](./type_defs.md#dbclusterparametergroupnamemessagetypedef).

<a id="modify_db_cluster_snapshot_attribute"></a>

### modify_db_cluster_snapshot_attribute

Adds an attribute and values to, or removes an attribute and values from, a
manual cluster snapshot.

Type annotations for
`session.create_client("docdb").modify_db_cluster_snapshot_attribute` method.

Boto3 documentation:
[DocDB.Client.modify_db_cluster_snapshot_attribute](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_cluster_snapshot_attribute)

Asynchronous method. Use `await modify_db_cluster_snapshot_attribute(...)` for
a synchronous call.

Arguments mapping described in
[ModifyDBClusterSnapshotAttributeMessageRequestTypeDef](./type_defs.md#modifydbclustersnapshotattributemessagerequesttypedef).

Keyword-only arguments:

- `DBClusterSnapshotIdentifier`: `str` *(required)*
- `AttributeName`: `str` *(required)*
- `ValuesToAdd`: `Sequence`\[`str`\]
- `ValuesToRemove`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[ModifyDBClusterSnapshotAttributeResultTypeDef](./type_defs.md#modifydbclustersnapshotattributeresulttypedef).

<a id="modify_db_instance"></a>

### modify_db_instance

Modifies settings for an instance.

Type annotations for `session.create_client("docdb").modify_db_instance`
method.

Boto3 documentation:
[DocDB.Client.modify_db_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_instance)

Asynchronous method. Use `await modify_db_instance(...)` for a synchronous
call.

Arguments mapping described in
[ModifyDBInstanceMessageRequestTypeDef](./type_defs.md#modifydbinstancemessagerequesttypedef).

Keyword-only arguments:

- `DBInstanceIdentifier`: `str` *(required)*
- `DBInstanceClass`: `str`
- `ApplyImmediately`: `bool`
- `PreferredMaintenanceWindow`: `str`
- `AutoMinorVersionUpgrade`: `bool`
- `NewDBInstanceIdentifier`: `str`
- `CACertificateIdentifier`: `str`
- `PromotionTier`: `int`

Returns a `Coroutine` for
[ModifyDBInstanceResultTypeDef](./type_defs.md#modifydbinstanceresulttypedef).

<a id="modify_db_subnet_group"></a>

### modify_db_subnet_group

Modifies an existing subnet group.

Type annotations for `session.create_client("docdb").modify_db_subnet_group`
method.

Boto3 documentation:
[DocDB.Client.modify_db_subnet_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_subnet_group)

Asynchronous method. Use `await modify_db_subnet_group(...)` for a synchronous
call.

Arguments mapping described in
[ModifyDBSubnetGroupMessageRequestTypeDef](./type_defs.md#modifydbsubnetgroupmessagerequesttypedef).

Keyword-only arguments:

- `DBSubnetGroupName`: `str` *(required)*
- `SubnetIds`: `Sequence`\[`str`\] *(required)*
- `DBSubnetGroupDescription`: `str`

Returns a `Coroutine` for
[ModifyDBSubnetGroupResultTypeDef](./type_defs.md#modifydbsubnetgroupresulttypedef).

<a id="modify_event_subscription"></a>

### modify_event_subscription

Modifies an existing Amazon DocumentDB event notification subscription.

Type annotations for `session.create_client("docdb").modify_event_subscription`
method.

Boto3 documentation:
[DocDB.Client.modify_event_subscription](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_event_subscription)

Asynchronous method. Use `await modify_event_subscription(...)` for a
synchronous call.

Arguments mapping described in
[ModifyEventSubscriptionMessageRequestTypeDef](./type_defs.md#modifyeventsubscriptionmessagerequesttypedef).

Keyword-only arguments:

- `SubscriptionName`: `str` *(required)*
- `SnsTopicArn`: `str`
- `SourceType`: `str`
- `EventCategories`: `Sequence`\[`str`\]
- `Enabled`: `bool`

Returns a `Coroutine` for
[ModifyEventSubscriptionResultTypeDef](./type_defs.md#modifyeventsubscriptionresulttypedef).

<a id="modify_global_cluster"></a>

### modify_global_cluster

Modify a setting for an Amazon DocumentDB global cluster.

Type annotations for `session.create_client("docdb").modify_global_cluster`
method.

Boto3 documentation:
[DocDB.Client.modify_global_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_global_cluster)

Asynchronous method. Use `await modify_global_cluster(...)` for a synchronous
call.

Arguments mapping described in
[ModifyGlobalClusterMessageRequestTypeDef](./type_defs.md#modifyglobalclustermessagerequesttypedef).

Keyword-only arguments:

- `GlobalClusterIdentifier`: `str` *(required)*
- `NewGlobalClusterIdentifier`: `str`
- `DeletionProtection`: `bool`

Returns a `Coroutine` for
[ModifyGlobalClusterResultTypeDef](./type_defs.md#modifyglobalclusterresulttypedef).

<a id="reboot_db_instance"></a>

### reboot_db_instance

You might need to reboot your instance, usually for maintenance reasons.

Type annotations for `session.create_client("docdb").reboot_db_instance`
method.

Boto3 documentation:
[DocDB.Client.reboot_db_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.reboot_db_instance)

Asynchronous method. Use `await reboot_db_instance(...)` for a synchronous
call.

Arguments mapping described in
[RebootDBInstanceMessageRequestTypeDef](./type_defs.md#rebootdbinstancemessagerequesttypedef).

Keyword-only arguments:

- `DBInstanceIdentifier`: `str` *(required)*
- `ForceFailover`: `bool`

Returns a `Coroutine` for
[RebootDBInstanceResultTypeDef](./type_defs.md#rebootdbinstanceresulttypedef).

<a id="remove_from_global_cluster"></a>

### remove_from_global_cluster

Detaches an Amazon DocumentDB secondary cluster from a global cluster.

Type annotations for
`session.create_client("docdb").remove_from_global_cluster` method.

Boto3 documentation:
[DocDB.Client.remove_from_global_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.remove_from_global_cluster)

Asynchronous method. Use `await remove_from_global_cluster(...)` for a
synchronous call.

Arguments mapping described in
[RemoveFromGlobalClusterMessageRequestTypeDef](./type_defs.md#removefromglobalclustermessagerequesttypedef).

Keyword-only arguments:

- `GlobalClusterIdentifier`: `str` *(required)*
- `DbClusterIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[RemoveFromGlobalClusterResultTypeDef](./type_defs.md#removefromglobalclusterresulttypedef).

<a id="remove_source_identifier_from_subscription"></a>

### remove_source_identifier_from_subscription

Removes a source identifier from an existing Amazon DocumentDB event
notification subscription.

Type annotations for
`session.create_client("docdb").remove_source_identifier_from_subscription`
method.

Boto3 documentation:
[DocDB.Client.remove_source_identifier_from_subscription](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.remove_source_identifier_from_subscription)

Asynchronous method. Use
`await remove_source_identifier_from_subscription(...)` for a synchronous call.

Arguments mapping described in
[RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef](./type_defs.md#removesourceidentifierfromsubscriptionmessagerequesttypedef).

Keyword-only arguments:

- `SubscriptionName`: `str` *(required)*
- `SourceIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[RemoveSourceIdentifierFromSubscriptionResultTypeDef](./type_defs.md#removesourceidentifierfromsubscriptionresulttypedef).

<a id="remove_tags_from_resource"></a>

### remove_tags_from_resource

Removes metadata tags from an Amazon DocumentDB resource.

Type annotations for `session.create_client("docdb").remove_tags_from_resource`
method.

Boto3 documentation:
[DocDB.Client.remove_tags_from_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.remove_tags_from_resource)

Asynchronous method. Use `await remove_tags_from_resource(...)` for a
synchronous call.

Arguments mapping described in
[RemoveTagsFromResourceMessageRequestTypeDef](./type_defs.md#removetagsfromresourcemessagerequesttypedef).

Keyword-only arguments:

- `ResourceName`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

<a id="reset_db_cluster_parameter_group"></a>

### reset_db_cluster_parameter_group

Modifies the parameters of a cluster parameter group to the default value.

Type annotations for
`session.create_client("docdb").reset_db_cluster_parameter_group` method.

Boto3 documentation:
[DocDB.Client.reset_db_cluster_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.reset_db_cluster_parameter_group)

Asynchronous method. Use `await reset_db_cluster_parameter_group(...)` for a
synchronous call.

Arguments mapping described in
[ResetDBClusterParameterGroupMessageRequestTypeDef](./type_defs.md#resetdbclusterparametergroupmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterParameterGroupName`: `str` *(required)*
- `ResetAllParameters`: `bool`
- `Parameters`:
  `Sequence`\[[ParameterTypeDef](./type_defs.md#parametertypedef)\]

Returns a `Coroutine` for
[DBClusterParameterGroupNameMessageTypeDef](./type_defs.md#dbclusterparametergroupnamemessagetypedef).

<a id="restore_db_cluster_from_snapshot"></a>

### restore_db_cluster_from_snapshot

Creates a new cluster from a snapshot or cluster snapshot.

Type annotations for
`session.create_client("docdb").restore_db_cluster_from_snapshot` method.

Boto3 documentation:
[DocDB.Client.restore_db_cluster_from_snapshot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.restore_db_cluster_from_snapshot)

Asynchronous method. Use `await restore_db_cluster_from_snapshot(...)` for a
synchronous call.

Arguments mapping described in
[RestoreDBClusterFromSnapshotMessageRequestTypeDef](./type_defs.md#restoredbclusterfromsnapshotmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*
- `SnapshotIdentifier`: `str` *(required)*
- `Engine`: `str` *(required)*
- `AvailabilityZones`: `Sequence`\[`str`\]
- `EngineVersion`: `str`
- `Port`: `int`
- `DBSubnetGroupName`: `str`
- `VpcSecurityGroupIds`: `Sequence`\[`str`\]
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `KmsKeyId`: `str`
- `EnableCloudwatchLogsExports`: `Sequence`\[`str`\]
- `DeletionProtection`: `bool`

Returns a `Coroutine` for
[RestoreDBClusterFromSnapshotResultTypeDef](./type_defs.md#restoredbclusterfromsnapshotresulttypedef).

<a id="restore_db_cluster_to_point_in_time"></a>

### restore_db_cluster_to_point_in_time

Restores a cluster to an arbitrary point in time.

Type annotations for
`session.create_client("docdb").restore_db_cluster_to_point_in_time` method.

Boto3 documentation:
[DocDB.Client.restore_db_cluster_to_point_in_time](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.restore_db_cluster_to_point_in_time)

Asynchronous method. Use `await restore_db_cluster_to_point_in_time(...)` for a
synchronous call.

Arguments mapping described in
[RestoreDBClusterToPointInTimeMessageRequestTypeDef](./type_defs.md#restoredbclustertopointintimemessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*
- `SourceDBClusterIdentifier`: `str` *(required)*
- `RestoreToTime`: `Union`\[`datetime`, `str`\]
- `UseLatestRestorableTime`: `bool`
- `Port`: `int`
- `DBSubnetGroupName`: `str`
- `VpcSecurityGroupIds`: `Sequence`\[`str`\]
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `KmsKeyId`: `str`
- `EnableCloudwatchLogsExports`: `Sequence`\[`str`\]
- `DeletionProtection`: `bool`

Returns a `Coroutine` for
[RestoreDBClusterToPointInTimeResultTypeDef](./type_defs.md#restoredbclustertopointintimeresulttypedef).

<a id="start_db_cluster"></a>

### start_db_cluster

Restarts the stopped cluster that is specified by `DBClusterIdentifier`.

Type annotations for `session.create_client("docdb").start_db_cluster` method.

Boto3 documentation:
[DocDB.Client.start_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.start_db_cluster)

Asynchronous method. Use `await start_db_cluster(...)` for a synchronous call.

Arguments mapping described in
[StartDBClusterMessageRequestTypeDef](./type_defs.md#startdbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[StartDBClusterResultTypeDef](./type_defs.md#startdbclusterresulttypedef).

<a id="stop_db_cluster"></a>

### stop_db_cluster

Stops the running cluster that is specified by `DBClusterIdentifier`.

Type annotations for `session.create_client("docdb").stop_db_cluster` method.

Boto3 documentation:
[DocDB.Client.stop_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.stop_db_cluster)

Asynchronous method. Use `await stop_db_cluster(...)` for a synchronous call.

Arguments mapping described in
[StopDBClusterMessageRequestTypeDef](./type_defs.md#stopdbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[StopDBClusterResultTypeDef](./type_defs.md#stopdbclusterresulttypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("docdb").__aenter__` method.

Boto3 documentation:
[DocDB.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [DocDBClient](#docdbclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("docdb").__aexit__` method.

Boto3 documentation:
[DocDB.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("docdb").get_paginator` method with
overloads.

- `client.get_paginator("describe_certificates")` ->
  [DescribeCertificatesPaginator](./paginators.md#describecertificatespaginator)
- `client.get_paginator("describe_db_cluster_parameter_groups")` ->
  [DescribeDBClusterParameterGroupsPaginator](./paginators.md#describedbclusterparametergroupspaginator)
- `client.get_paginator("describe_db_cluster_parameters")` ->
  [DescribeDBClusterParametersPaginator](./paginators.md#describedbclusterparameterspaginator)
- `client.get_paginator("describe_db_cluster_snapshots")` ->
  [DescribeDBClusterSnapshotsPaginator](./paginators.md#describedbclustersnapshotspaginator)
- `client.get_paginator("describe_db_clusters")` ->
  [DescribeDBClustersPaginator](./paginators.md#describedbclusterspaginator)
- `client.get_paginator("describe_db_engine_versions")` ->
  [DescribeDBEngineVersionsPaginator](./paginators.md#describedbengineversionspaginator)
- `client.get_paginator("describe_db_instances")` ->
  [DescribeDBInstancesPaginator](./paginators.md#describedbinstancespaginator)
- `client.get_paginator("describe_db_subnet_groups")` ->
  [DescribeDBSubnetGroupsPaginator](./paginators.md#describedbsubnetgroupspaginator)
- `client.get_paginator("describe_event_subscriptions")` ->
  [DescribeEventSubscriptionsPaginator](./paginators.md#describeeventsubscriptionspaginator)
- `client.get_paginator("describe_events")` ->
  [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
- `client.get_paginator("describe_global_clusters")` ->
  [DescribeGlobalClustersPaginator](./paginators.md#describeglobalclusterspaginator)
- `client.get_paginator("describe_orderable_db_instance_options")` ->
  [DescribeOrderableDBInstanceOptionsPaginator](./paginators.md#describeorderabledbinstanceoptionspaginator)
- `client.get_paginator("describe_pending_maintenance_actions")` ->
  [DescribePendingMaintenanceActionsPaginator](./paginators.md#describependingmaintenanceactionspaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("docdb").get_waiter` method with
overloads.

- `client.get_waiter("db_instance_available")` ->
  [DBInstanceAvailableWaiter](./waiters.md#dbinstanceavailablewaiter)
- `client.get_waiter("db_instance_deleted")` ->
  [DBInstanceDeletedWaiter](./waiters.md#dbinstancedeletedwaiter)
