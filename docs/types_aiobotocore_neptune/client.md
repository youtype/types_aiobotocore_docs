<a id="neptuneclient-for-aiobotocore-neptune-module"></a>

# NeptuneClient for aiobotocore Neptune module

> [Index](../README.md) > [Neptune](./README.md) > NeptuneClient

Auto-generated documentation for
[Neptune](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
type annotations stubs module
[types-aiobotocore-neptune](https://pypi.org/project/types-aiobotocore-neptune/).

- [NeptuneClient for aiobotocore Neptune module](#neptuneclient-for-aiobotocore-neptune-module)
  - [NeptuneClient](#neptuneclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [add_role_to_db_cluster](#add_role_to_db_cluster)
    - [add_source_identifier_to_subscription](#add_source_identifier_to_subscription)
    - [add_tags_to_resource](#add_tags_to_resource)
    - [apply_pending_maintenance_action](#apply_pending_maintenance_action)
    - [can_paginate](#can_paginate)
    - [copy_db_cluster_parameter_group](#copy_db_cluster_parameter_group)
    - [copy_db_cluster_snapshot](#copy_db_cluster_snapshot)
    - [copy_db_parameter_group](#copy_db_parameter_group)
    - [create_db_cluster](#create_db_cluster)
    - [create_db_cluster_endpoint](#create_db_cluster_endpoint)
    - [create_db_cluster_parameter_group](#create_db_cluster_parameter_group)
    - [create_db_cluster_snapshot](#create_db_cluster_snapshot)
    - [create_db_instance](#create_db_instance)
    - [create_db_parameter_group](#create_db_parameter_group)
    - [create_db_subnet_group](#create_db_subnet_group)
    - [create_event_subscription](#create_event_subscription)
    - [delete_db_cluster](#delete_db_cluster)
    - [delete_db_cluster_endpoint](#delete_db_cluster_endpoint)
    - [delete_db_cluster_parameter_group](#delete_db_cluster_parameter_group)
    - [delete_db_cluster_snapshot](#delete_db_cluster_snapshot)
    - [delete_db_instance](#delete_db_instance)
    - [delete_db_parameter_group](#delete_db_parameter_group)
    - [delete_db_subnet_group](#delete_db_subnet_group)
    - [delete_event_subscription](#delete_event_subscription)
    - [describe_db_cluster_endpoints](#describe_db_cluster_endpoints)
    - [describe_db_cluster_parameter_groups](#describe_db_cluster_parameter_groups)
    - [describe_db_cluster_parameters](#describe_db_cluster_parameters)
    - [describe_db_cluster_snapshot_attributes](#describe_db_cluster_snapshot_attributes)
    - [describe_db_cluster_snapshots](#describe_db_cluster_snapshots)
    - [describe_db_clusters](#describe_db_clusters)
    - [describe_db_engine_versions](#describe_db_engine_versions)
    - [describe_db_instances](#describe_db_instances)
    - [describe_db_parameter_groups](#describe_db_parameter_groups)
    - [describe_db_parameters](#describe_db_parameters)
    - [describe_db_subnet_groups](#describe_db_subnet_groups)
    - [describe_engine_default_cluster_parameters](#describe_engine_default_cluster_parameters)
    - [describe_engine_default_parameters](#describe_engine_default_parameters)
    - [describe_event_categories](#describe_event_categories)
    - [describe_event_subscriptions](#describe_event_subscriptions)
    - [describe_events](#describe_events)
    - [describe_orderable_db_instance_options](#describe_orderable_db_instance_options)
    - [describe_pending_maintenance_actions](#describe_pending_maintenance_actions)
    - [describe_valid_db_instance_modifications](#describe_valid_db_instance_modifications)
    - [failover_db_cluster](#failover_db_cluster)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [modify_db_cluster](#modify_db_cluster)
    - [modify_db_cluster_endpoint](#modify_db_cluster_endpoint)
    - [modify_db_cluster_parameter_group](#modify_db_cluster_parameter_group)
    - [modify_db_cluster_snapshot_attribute](#modify_db_cluster_snapshot_attribute)
    - [modify_db_instance](#modify_db_instance)
    - [modify_db_parameter_group](#modify_db_parameter_group)
    - [modify_db_subnet_group](#modify_db_subnet_group)
    - [modify_event_subscription](#modify_event_subscription)
    - [promote_read_replica_db_cluster](#promote_read_replica_db_cluster)
    - [reboot_db_instance](#reboot_db_instance)
    - [remove_role_from_db_cluster](#remove_role_from_db_cluster)
    - [remove_source_identifier_from_subscription](#remove_source_identifier_from_subscription)
    - [remove_tags_from_resource](#remove_tags_from_resource)
    - [reset_db_cluster_parameter_group](#reset_db_cluster_parameter_group)
    - [reset_db_parameter_group](#reset_db_parameter_group)
    - [restore_db_cluster_from_snapshot](#restore_db_cluster_from_snapshot)
    - [restore_db_cluster_to_point_in_time](#restore_db_cluster_to_point_in_time)
    - [start_db_cluster](#start_db_cluster)
    - [stop_db_cluster](#stop_db_cluster)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="neptuneclient"></a>

## NeptuneClient

Type annotations for `session.create_client("neptune")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_neptune.client import NeptuneClient

session = get_session()
async with session.create_client("neptune") as client:
    client: NeptuneClient
```

Boto3 documentation:
[Neptune.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_neptune.client import Exceptions

def handle_error(exc: Exceptions.AuthorizationNotFoundFault) -> None:
    ...
```

Exceptions:

- `Exceptions.AuthorizationNotFoundFault`
- `Exceptions.CertificateNotFoundFault`
- `Exceptions.ClientError`
- `Exceptions.DBClusterAlreadyExistsFault`
- `Exceptions.DBClusterEndpointAlreadyExistsFault`
- `Exceptions.DBClusterEndpointNotFoundFault`
- `Exceptions.DBClusterEndpointQuotaExceededFault`
- `Exceptions.DBClusterNotFoundFault`
- `Exceptions.DBClusterParameterGroupNotFoundFault`
- `Exceptions.DBClusterQuotaExceededFault`
- `Exceptions.DBClusterRoleAlreadyExistsFault`
- `Exceptions.DBClusterRoleNotFoundFault`
- `Exceptions.DBClusterRoleQuotaExceededFault`
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
- `Exceptions.DomainNotFoundFault`
- `Exceptions.EventSubscriptionQuotaExceededFault`
- `Exceptions.InstanceQuotaExceededFault`
- `Exceptions.InsufficientDBClusterCapacityFault`
- `Exceptions.InsufficientDBInstanceCapacityFault`
- `Exceptions.InsufficientStorageClusterCapacityFault`
- `Exceptions.InvalidDBClusterEndpointStateFault`
- `Exceptions.InvalidDBClusterSnapshotStateFault`
- `Exceptions.InvalidDBClusterStateFault`
- `Exceptions.InvalidDBInstanceStateFault`
- `Exceptions.InvalidDBParameterGroupStateFault`
- `Exceptions.InvalidDBSecurityGroupStateFault`
- `Exceptions.InvalidDBSnapshotStateFault`
- `Exceptions.InvalidDBSubnetGroupStateFault`
- `Exceptions.InvalidDBSubnetStateFault`
- `Exceptions.InvalidEventSubscriptionStateFault`
- `Exceptions.InvalidRestoreFault`
- `Exceptions.InvalidSubnet`
- `Exceptions.InvalidVPCNetworkStateFault`
- `Exceptions.KMSKeyNotAccessibleFault`
- `Exceptions.OptionGroupNotFoundFault`
- `Exceptions.ProvisionedIopsNotAvailableInAZFault`
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

NeptuneClient exceptions.

Type annotations for `session.create_client("neptune").exceptions` method.

Boto3 documentation:
[Neptune.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="add\_role\_to\_db\_cluster"></a>

### add_role_to_db_cluster

Associates an Identity and Access Management (IAM) role with an Neptune DB
cluster.

Type annotations for `session.create_client("neptune").add_role_to_db_cluster`
method.

Boto3 documentation:
[Neptune.Client.add_role_to_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.add_role_to_db_cluster)

Asynchronous method. Use `await add_role_to_db_cluster(...)` for a synchronous
call.

Arguments mapping described in
[AddRoleToDBClusterMessageRequestTypeDef](./type_defs.md#addroletodbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*
- `RoleArn`: `str` *(required)*
- `FeatureName`: `str`

<a id="add\_source\_identifier\_to\_subscription"></a>

### add_source_identifier_to_subscription

Adds a source identifier to an existing event notification subscription.

Type annotations for
`session.create_client("neptune").add_source_identifier_to_subscription`
method.

Boto3 documentation:
[Neptune.Client.add_source_identifier_to_subscription](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.add_source_identifier_to_subscription)

Asynchronous method. Use `await add_source_identifier_to_subscription(...)` for
a synchronous call.

Arguments mapping described in
[AddSourceIdentifierToSubscriptionMessageRequestTypeDef](./type_defs.md#addsourceidentifiertosubscriptionmessagerequesttypedef).

Keyword-only arguments:

- `SubscriptionName`: `str` *(required)*
- `SourceIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[AddSourceIdentifierToSubscriptionResultTypeDef](./type_defs.md#addsourceidentifiertosubscriptionresulttypedef).

<a id="add\_tags\_to\_resource"></a>

### add_tags_to_resource

Adds metadata tags to an Amazon Neptune resource.

Type annotations for `session.create_client("neptune").add_tags_to_resource`
method.

Boto3 documentation:
[Neptune.Client.add_tags_to_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.add_tags_to_resource)

Asynchronous method. Use `await add_tags_to_resource(...)` for a synchronous
call.

Arguments mapping described in
[AddTagsToResourceMessageRequestTypeDef](./type_defs.md#addtagstoresourcemessagerequesttypedef).

Keyword-only arguments:

- `ResourceName`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

<a id="apply\_pending\_maintenance\_action"></a>

### apply_pending_maintenance_action

Applies a pending maintenance action to a resource (for example, to a DB
instance).

Type annotations for
`session.create_client("neptune").apply_pending_maintenance_action` method.

Boto3 documentation:
[Neptune.Client.apply_pending_maintenance_action](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.apply_pending_maintenance_action)

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

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("neptune").can_paginate` method.

Boto3 documentation:
[Neptune.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="copy\_db\_cluster\_parameter\_group"></a>

### copy_db_cluster_parameter_group

Copies the specified DB cluster parameter group.

Type annotations for
`session.create_client("neptune").copy_db_cluster_parameter_group` method.

Boto3 documentation:
[Neptune.Client.copy_db_cluster_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.copy_db_cluster_parameter_group)

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

<a id="copy\_db\_cluster\_snapshot"></a>

### copy_db_cluster_snapshot

Copies a snapshot of a DB cluster.

Type annotations for
`session.create_client("neptune").copy_db_cluster_snapshot` method.

Boto3 documentation:
[Neptune.Client.copy_db_cluster_snapshot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.copy_db_cluster_snapshot)

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

<a id="copy\_db\_parameter\_group"></a>

### copy_db_parameter_group

Copies the specified DB parameter group.

Type annotations for `session.create_client("neptune").copy_db_parameter_group`
method.

Boto3 documentation:
[Neptune.Client.copy_db_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.copy_db_parameter_group)

Asynchronous method. Use `await copy_db_parameter_group(...)` for a synchronous
call.

Arguments mapping described in
[CopyDBParameterGroupMessageRequestTypeDef](./type_defs.md#copydbparametergroupmessagerequesttypedef).

Keyword-only arguments:

- `SourceDBParameterGroupIdentifier`: `str` *(required)*
- `TargetDBParameterGroupIdentifier`: `str` *(required)*
- `TargetDBParameterGroupDescription`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CopyDBParameterGroupResultTypeDef](./type_defs.md#copydbparametergroupresulttypedef).

<a id="create\_db\_cluster"></a>

### create_db_cluster

Creates a new Amazon Neptune DB cluster.

Type annotations for `session.create_client("neptune").create_db_cluster`
method.

Boto3 documentation:
[Neptune.Client.create_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_cluster)

Asynchronous method. Use `await create_db_cluster(...)` for a synchronous call.

Arguments mapping described in
[CreateDBClusterMessageRequestTypeDef](./type_defs.md#createdbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*
- `Engine`: `str` *(required)*
- `AvailabilityZones`: `Sequence`\[`str`\]
- `BackupRetentionPeriod`: `int`
- `CharacterSetName`: `str`
- `CopyTagsToSnapshot`: `bool`
- `DatabaseName`: `str`
- `DBClusterParameterGroupName`: `str`
- `VpcSecurityGroupIds`: `Sequence`\[`str`\]
- `DBSubnetGroupName`: `str`
- `EngineVersion`: `str`
- `Port`: `int`
- `MasterUsername`: `str`
- `MasterUserPassword`: `str`
- `OptionGroupName`: `str`
- `PreferredBackupWindow`: `str`
- `PreferredMaintenanceWindow`: `str`
- `ReplicationSourceIdentifier`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `StorageEncrypted`: `bool`
- `KmsKeyId`: `str`
- `PreSignedUrl`: `str`
- `EnableIAMDatabaseAuthentication`: `bool`
- `EnableCloudwatchLogsExports`: `Sequence`\[`str`\]
- `DeletionProtection`: `bool`
- `SourceRegion`: `str`

Returns a `Coroutine` for
[CreateDBClusterResultTypeDef](./type_defs.md#createdbclusterresulttypedef).

<a id="create\_db\_cluster\_endpoint"></a>

### create_db_cluster_endpoint

Creates a new custom endpoint and associates it with an Amazon Neptune DB
cluster.

Type annotations for
`session.create_client("neptune").create_db_cluster_endpoint` method.

Boto3 documentation:
[Neptune.Client.create_db_cluster_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_cluster_endpoint)

Asynchronous method. Use `await create_db_cluster_endpoint(...)` for a
synchronous call.

Arguments mapping described in
[CreateDBClusterEndpointMessageRequestTypeDef](./type_defs.md#createdbclusterendpointmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*
- `DBClusterEndpointIdentifier`: `str` *(required)*
- `EndpointType`: `str` *(required)*
- `StaticMembers`: `Sequence`\[`str`\]
- `ExcludedMembers`: `Sequence`\[`str`\]
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateDBClusterEndpointOutputTypeDef](./type_defs.md#createdbclusterendpointoutputtypedef).

<a id="create\_db\_cluster\_parameter\_group"></a>

### create_db_cluster_parameter_group

Creates a new DB cluster parameter group.

Type annotations for
`session.create_client("neptune").create_db_cluster_parameter_group` method.

Boto3 documentation:
[Neptune.Client.create_db_cluster_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_cluster_parameter_group)

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

<a id="create\_db\_cluster\_snapshot"></a>

### create_db_cluster_snapshot

Creates a snapshot of a DB cluster.

Type annotations for
`session.create_client("neptune").create_db_cluster_snapshot` method.

Boto3 documentation:
[Neptune.Client.create_db_cluster_snapshot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_cluster_snapshot)

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

<a id="create\_db\_instance"></a>

### create_db_instance

Creates a new DB instance.

Type annotations for `session.create_client("neptune").create_db_instance`
method.

Boto3 documentation:
[Neptune.Client.create_db_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_instance)

Asynchronous method. Use `await create_db_instance(...)` for a synchronous
call.

Arguments mapping described in
[CreateDBInstanceMessageRequestTypeDef](./type_defs.md#createdbinstancemessagerequesttypedef).

Keyword-only arguments:

- `DBInstanceIdentifier`: `str` *(required)*
- `DBInstanceClass`: `str` *(required)*
- `Engine`: `str` *(required)*
- `DBName`: `str`
- `AllocatedStorage`: `int`
- `MasterUsername`: `str`
- `MasterUserPassword`: `str`
- `DBSecurityGroups`: `Sequence`\[`str`\]
- `VpcSecurityGroupIds`: `Sequence`\[`str`\]
- `AvailabilityZone`: `str`
- `DBSubnetGroupName`: `str`
- `PreferredMaintenanceWindow`: `str`
- `DBParameterGroupName`: `str`
- `BackupRetentionPeriod`: `int`
- `PreferredBackupWindow`: `str`
- `Port`: `int`
- `MultiAZ`: `bool`
- `EngineVersion`: `str`
- `AutoMinorVersionUpgrade`: `bool`
- `LicenseModel`: `str`
- `Iops`: `int`
- `OptionGroupName`: `str`
- `CharacterSetName`: `str`
- `PubliclyAccessible`: `bool`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `DBClusterIdentifier`: `str`
- `StorageType`: `str`
- `TdeCredentialArn`: `str`
- `TdeCredentialPassword`: `str`
- `StorageEncrypted`: `bool`
- `KmsKeyId`: `str`
- `Domain`: `str`
- `CopyTagsToSnapshot`: `bool`
- `MonitoringInterval`: `int`
- `MonitoringRoleArn`: `str`
- `DomainIAMRoleName`: `str`
- `PromotionTier`: `int`
- `Timezone`: `str`
- `EnableIAMDatabaseAuthentication`: `bool`
- `EnablePerformanceInsights`: `bool`
- `PerformanceInsightsKMSKeyId`: `str`
- `EnableCloudwatchLogsExports`: `Sequence`\[`str`\]
- `DeletionProtection`: `bool`

Returns a `Coroutine` for
[CreateDBInstanceResultTypeDef](./type_defs.md#createdbinstanceresulttypedef).

<a id="create\_db\_parameter\_group"></a>

### create_db_parameter_group

Creates a new DB parameter group.

Type annotations for
`session.create_client("neptune").create_db_parameter_group` method.

Boto3 documentation:
[Neptune.Client.create_db_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_parameter_group)

Asynchronous method. Use `await create_db_parameter_group(...)` for a
synchronous call.

Arguments mapping described in
[CreateDBParameterGroupMessageRequestTypeDef](./type_defs.md#createdbparametergroupmessagerequesttypedef).

Keyword-only arguments:

- `DBParameterGroupName`: `str` *(required)*
- `DBParameterGroupFamily`: `str` *(required)*
- `Description`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateDBParameterGroupResultTypeDef](./type_defs.md#createdbparametergroupresulttypedef).

<a id="create\_db\_subnet\_group"></a>

### create_db_subnet_group

Creates a new DB subnet group.

Type annotations for `session.create_client("neptune").create_db_subnet_group`
method.

Boto3 documentation:
[Neptune.Client.create_db_subnet_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_db_subnet_group)

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

<a id="create\_event\_subscription"></a>

### create_event_subscription

Creates an event notification subscription.

Type annotations for
`session.create_client("neptune").create_event_subscription` method.

Boto3 documentation:
[Neptune.Client.create_event_subscription](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.create_event_subscription)

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

<a id="delete\_db\_cluster"></a>

### delete_db_cluster

The DeleteDBCluster action deletes a previously provisioned DB cluster.

Type annotations for `session.create_client("neptune").delete_db_cluster`
method.

Boto3 documentation:
[Neptune.Client.delete_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.delete_db_cluster)

Asynchronous method. Use `await delete_db_cluster(...)` for a synchronous call.

Arguments mapping described in
[DeleteDBClusterMessageRequestTypeDef](./type_defs.md#deletedbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*
- `SkipFinalSnapshot`: `bool`
- `FinalDBSnapshotIdentifier`: `str`

Returns a `Coroutine` for
[DeleteDBClusterResultTypeDef](./type_defs.md#deletedbclusterresulttypedef).

<a id="delete\_db\_cluster\_endpoint"></a>

### delete_db_cluster_endpoint

Deletes a custom endpoint and removes it from an Amazon Neptune DB cluster.

Type annotations for
`session.create_client("neptune").delete_db_cluster_endpoint` method.

Boto3 documentation:
[Neptune.Client.delete_db_cluster_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.delete_db_cluster_endpoint)

Asynchronous method. Use `await delete_db_cluster_endpoint(...)` for a
synchronous call.

Arguments mapping described in
[DeleteDBClusterEndpointMessageRequestTypeDef](./type_defs.md#deletedbclusterendpointmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterEndpointIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[DeleteDBClusterEndpointOutputTypeDef](./type_defs.md#deletedbclusterendpointoutputtypedef).

<a id="delete\_db\_cluster\_parameter\_group"></a>

### delete_db_cluster_parameter_group

Deletes a specified DB cluster parameter group.

Type annotations for
`session.create_client("neptune").delete_db_cluster_parameter_group` method.

Boto3 documentation:
[Neptune.Client.delete_db_cluster_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.delete_db_cluster_parameter_group)

Asynchronous method. Use `await delete_db_cluster_parameter_group(...)` for a
synchronous call.

Arguments mapping described in
[DeleteDBClusterParameterGroupMessageRequestTypeDef](./type_defs.md#deletedbclusterparametergroupmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterParameterGroupName`: `str` *(required)*

<a id="delete\_db\_cluster\_snapshot"></a>

### delete_db_cluster_snapshot

Deletes a DB cluster snapshot.

Type annotations for
`session.create_client("neptune").delete_db_cluster_snapshot` method.

Boto3 documentation:
[Neptune.Client.delete_db_cluster_snapshot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.delete_db_cluster_snapshot)

Asynchronous method. Use `await delete_db_cluster_snapshot(...)` for a
synchronous call.

Arguments mapping described in
[DeleteDBClusterSnapshotMessageRequestTypeDef](./type_defs.md#deletedbclustersnapshotmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterSnapshotIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[DeleteDBClusterSnapshotResultTypeDef](./type_defs.md#deletedbclustersnapshotresulttypedef).

<a id="delete\_db\_instance"></a>

### delete_db_instance

The DeleteDBInstance action deletes a previously provisioned DB instance.

Type annotations for `session.create_client("neptune").delete_db_instance`
method.

Boto3 documentation:
[Neptune.Client.delete_db_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.delete_db_instance)

Asynchronous method. Use `await delete_db_instance(...)` for a synchronous
call.

Arguments mapping described in
[DeleteDBInstanceMessageRequestTypeDef](./type_defs.md#deletedbinstancemessagerequesttypedef).

Keyword-only arguments:

- `DBInstanceIdentifier`: `str` *(required)*
- `SkipFinalSnapshot`: `bool`
- `FinalDBSnapshotIdentifier`: `str`

Returns a `Coroutine` for
[DeleteDBInstanceResultTypeDef](./type_defs.md#deletedbinstanceresulttypedef).

<a id="delete\_db\_parameter\_group"></a>

### delete_db_parameter_group

Deletes a specified DBParameterGroup.

Type annotations for
`session.create_client("neptune").delete_db_parameter_group` method.

Boto3 documentation:
[Neptune.Client.delete_db_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.delete_db_parameter_group)

Asynchronous method. Use `await delete_db_parameter_group(...)` for a
synchronous call.

Arguments mapping described in
[DeleteDBParameterGroupMessageRequestTypeDef](./type_defs.md#deletedbparametergroupmessagerequesttypedef).

Keyword-only arguments:

- `DBParameterGroupName`: `str` *(required)*

<a id="delete\_db\_subnet\_group"></a>

### delete_db_subnet_group

Deletes a DB subnet group.

Type annotations for `session.create_client("neptune").delete_db_subnet_group`
method.

Boto3 documentation:
[Neptune.Client.delete_db_subnet_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.delete_db_subnet_group)

Asynchronous method. Use `await delete_db_subnet_group(...)` for a synchronous
call.

Arguments mapping described in
[DeleteDBSubnetGroupMessageRequestTypeDef](./type_defs.md#deletedbsubnetgroupmessagerequesttypedef).

Keyword-only arguments:

- `DBSubnetGroupName`: `str` *(required)*

<a id="delete\_event\_subscription"></a>

### delete_event_subscription

Deletes an event notification subscription.

Type annotations for
`session.create_client("neptune").delete_event_subscription` method.

Boto3 documentation:
[Neptune.Client.delete_event_subscription](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.delete_event_subscription)

Asynchronous method. Use `await delete_event_subscription(...)` for a
synchronous call.

Arguments mapping described in
[DeleteEventSubscriptionMessageRequestTypeDef](./type_defs.md#deleteeventsubscriptionmessagerequesttypedef).

Keyword-only arguments:

- `SubscriptionName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteEventSubscriptionResultTypeDef](./type_defs.md#deleteeventsubscriptionresulttypedef).

<a id="describe\_db\_cluster\_endpoints"></a>

### describe_db_cluster_endpoints

Returns information about endpoints for an Amazon Neptune DB cluster.

Type annotations for
`session.create_client("neptune").describe_db_cluster_endpoints` method.

Boto3 documentation:
[Neptune.Client.describe_db_cluster_endpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_cluster_endpoints)

Asynchronous method. Use `await describe_db_cluster_endpoints(...)` for a
synchronous call.

Arguments mapping described in
[DescribeDBClusterEndpointsMessageRequestTypeDef](./type_defs.md#describedbclusterendpointsmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str`
- `DBClusterEndpointIdentifier`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[DBClusterEndpointMessageTypeDef](./type_defs.md#dbclusterendpointmessagetypedef).

<a id="describe\_db\_cluster\_parameter\_groups"></a>

### describe_db_cluster_parameter_groups

Returns a list of `DBClusterParameterGroup` descriptions.

Type annotations for
`session.create_client("neptune").describe_db_cluster_parameter_groups` method.

Boto3 documentation:
[Neptune.Client.describe_db_cluster_parameter_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_cluster_parameter_groups)

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

<a id="describe\_db\_cluster\_parameters"></a>

### describe_db_cluster_parameters

Returns the detailed parameter list for a particular DB cluster parameter
group.

Type annotations for
`session.create_client("neptune").describe_db_cluster_parameters` method.

Boto3 documentation:
[Neptune.Client.describe_db_cluster_parameters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_cluster_parameters)

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

<a id="describe\_db\_cluster\_snapshot\_attributes"></a>

### describe_db_cluster_snapshot_attributes

Returns a list of DB cluster snapshot attribute names and values for a manual
DB cluster snapshot.

Type annotations for
`session.create_client("neptune").describe_db_cluster_snapshot_attributes`
method.

Boto3 documentation:
[Neptune.Client.describe_db_cluster_snapshot_attributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_cluster_snapshot_attributes)

Asynchronous method. Use `await describe_db_cluster_snapshot_attributes(...)`
for a synchronous call.

Arguments mapping described in
[DescribeDBClusterSnapshotAttributesMessageRequestTypeDef](./type_defs.md#describedbclustersnapshotattributesmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterSnapshotIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDBClusterSnapshotAttributesResultTypeDef](./type_defs.md#describedbclustersnapshotattributesresulttypedef).

<a id="describe\_db\_cluster\_snapshots"></a>

### describe_db_cluster_snapshots

Returns information about DB cluster snapshots.

Type annotations for
`session.create_client("neptune").describe_db_cluster_snapshots` method.

Boto3 documentation:
[Neptune.Client.describe_db_cluster_snapshots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_cluster_snapshots)

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

<a id="describe\_db\_clusters"></a>

### describe_db_clusters

Returns information about provisioned DB clusters, and supports pagination.

Type annotations for `session.create_client("neptune").describe_db_clusters`
method.

Boto3 documentation:
[Neptune.Client.describe_db_clusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_clusters)

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

<a id="describe\_db\_engine\_versions"></a>

### describe_db_engine_versions

Returns a list of the available DB engines.

Type annotations for
`session.create_client("neptune").describe_db_engine_versions` method.

Boto3 documentation:
[Neptune.Client.describe_db_engine_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_engine_versions)

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

<a id="describe\_db\_instances"></a>

### describe_db_instances

Returns information about provisioned instances, and supports pagination.

Type annotations for `session.create_client("neptune").describe_db_instances`
method.

Boto3 documentation:
[Neptune.Client.describe_db_instances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_instances)

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

<a id="describe\_db\_parameter\_groups"></a>

### describe_db_parameter_groups

Returns a list of `DBParameterGroup` descriptions.

Type annotations for
`session.create_client("neptune").describe_db_parameter_groups` method.

Boto3 documentation:
[Neptune.Client.describe_db_parameter_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_parameter_groups)

Asynchronous method. Use `await describe_db_parameter_groups(...)` for a
synchronous call.

Arguments mapping described in
[DescribeDBParameterGroupsMessageRequestTypeDef](./type_defs.md#describedbparametergroupsmessagerequesttypedef).

Keyword-only arguments:

- `DBParameterGroupName`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[DBParameterGroupsMessageTypeDef](./type_defs.md#dbparametergroupsmessagetypedef).

<a id="describe\_db\_parameters"></a>

### describe_db_parameters

Returns the detailed parameter list for a particular DB parameter group.

Type annotations for `session.create_client("neptune").describe_db_parameters`
method.

Boto3 documentation:
[Neptune.Client.describe_db_parameters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_parameters)

Asynchronous method. Use `await describe_db_parameters(...)` for a synchronous
call.

Arguments mapping described in
[DescribeDBParametersMessageRequestTypeDef](./type_defs.md#describedbparametersmessagerequesttypedef).

Keyword-only arguments:

- `DBParameterGroupName`: `str` *(required)*
- `Source`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[DBParameterGroupDetailsTypeDef](./type_defs.md#dbparametergroupdetailstypedef).

<a id="describe\_db\_subnet\_groups"></a>

### describe_db_subnet_groups

Returns a list of DBSubnetGroup descriptions.

Type annotations for
`session.create_client("neptune").describe_db_subnet_groups` method.

Boto3 documentation:
[Neptune.Client.describe_db_subnet_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_db_subnet_groups)

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

<a id="describe\_engine\_default\_cluster\_parameters"></a>

### describe_engine_default_cluster_parameters

Returns the default engine and system parameter information for the cluster
database engine.

Type annotations for
`session.create_client("neptune").describe_engine_default_cluster_parameters`
method.

Boto3 documentation:
[Neptune.Client.describe_engine_default_cluster_parameters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_engine_default_cluster_parameters)

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

<a id="describe\_engine\_default\_parameters"></a>

### describe_engine_default_parameters

Returns the default engine and system parameter information for the specified
database engine.

Type annotations for
`session.create_client("neptune").describe_engine_default_parameters` method.

Boto3 documentation:
[Neptune.Client.describe_engine_default_parameters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_engine_default_parameters)

Asynchronous method. Use `await describe_engine_default_parameters(...)` for a
synchronous call.

Arguments mapping described in
[DescribeEngineDefaultParametersMessageRequestTypeDef](./type_defs.md#describeenginedefaultparametersmessagerequesttypedef).

Keyword-only arguments:

- `DBParameterGroupFamily`: `str` *(required)*
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `MaxRecords`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[DescribeEngineDefaultParametersResultTypeDef](./type_defs.md#describeenginedefaultparametersresulttypedef).

<a id="describe\_event\_categories"></a>

### describe_event_categories

Displays a list of categories for all event source types, or, if specified, for
a specified source type.

Type annotations for
`session.create_client("neptune").describe_event_categories` method.

Boto3 documentation:
[Neptune.Client.describe_event_categories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_event_categories)

Asynchronous method. Use `await describe_event_categories(...)` for a
synchronous call.

Arguments mapping described in
[DescribeEventCategoriesMessageRequestTypeDef](./type_defs.md#describeeventcategoriesmessagerequesttypedef).

Keyword-only arguments:

- `SourceType`: `str`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[EventCategoriesMessageTypeDef](./type_defs.md#eventcategoriesmessagetypedef).

<a id="describe\_event\_subscriptions"></a>

### describe_event_subscriptions

Lists all the subscription descriptions for a customer account.

Type annotations for
`session.create_client("neptune").describe_event_subscriptions` method.

Boto3 documentation:
[Neptune.Client.describe_event_subscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_event_subscriptions)

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

<a id="describe\_events"></a>

### describe_events

Returns events related to DB instances, DB security groups, DB snapshots, and
DB parameter groups for the past 14 days.

Type annotations for `session.create_client("neptune").describe_events` method.

Boto3 documentation:
[Neptune.Client.describe_events](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_events)

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

<a id="describe\_orderable\_db\_instance\_options"></a>

### describe_orderable_db_instance_options

Returns a list of orderable DB instance options for the specified engine.

Type annotations for
`session.create_client("neptune").describe_orderable_db_instance_options`
method.

Boto3 documentation:
[Neptune.Client.describe_orderable_db_instance_options](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_orderable_db_instance_options)

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

<a id="describe\_pending\_maintenance\_actions"></a>

### describe_pending_maintenance_actions

Returns a list of resources (for example, DB instances) that have at least one
pending maintenance action.

Type annotations for
`session.create_client("neptune").describe_pending_maintenance_actions` method.

Boto3 documentation:
[Neptune.Client.describe_pending_maintenance_actions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_pending_maintenance_actions)

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

<a id="describe\_valid\_db\_instance\_modifications"></a>

### describe_valid_db_instance_modifications

You can call DescribeValidDBInstanceModifications to learn what modifications
you can make to your DB instance.

Type annotations for
`session.create_client("neptune").describe_valid_db_instance_modifications`
method.

Boto3 documentation:
[Neptune.Client.describe_valid_db_instance_modifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.describe_valid_db_instance_modifications)

Asynchronous method. Use `await describe_valid_db_instance_modifications(...)`
for a synchronous call.

Arguments mapping described in
[DescribeValidDBInstanceModificationsMessageRequestTypeDef](./type_defs.md#describevaliddbinstancemodificationsmessagerequesttypedef).

Keyword-only arguments:

- `DBInstanceIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[DescribeValidDBInstanceModificationsResultTypeDef](./type_defs.md#describevaliddbinstancemodificationsresulttypedef).

<a id="failover\_db\_cluster"></a>

### failover_db_cluster

Forces a failover for a DB cluster.

Type annotations for `session.create_client("neptune").failover_db_cluster`
method.

Boto3 documentation:
[Neptune.Client.failover_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.failover_db_cluster)

Asynchronous method. Use `await failover_db_cluster(...)` for a synchronous
call.

Arguments mapping described in
[FailoverDBClusterMessageRequestTypeDef](./type_defs.md#failoverdbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str`
- `TargetDBInstanceIdentifier`: `str`

Returns a `Coroutine` for
[FailoverDBClusterResultTypeDef](./type_defs.md#failoverdbclusterresulttypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("neptune").generate_presigned_url`
method.

Boto3 documentation:
[Neptune.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Lists all tags on an Amazon Neptune resource.

Type annotations for `session.create_client("neptune").list_tags_for_resource`
method.

Boto3 documentation:
[Neptune.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceMessageRequestTypeDef](./type_defs.md#listtagsforresourcemessagerequesttypedef).

Keyword-only arguments:

- `ResourceName`: `str` *(required)*
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[TagListMessageTypeDef](./type_defs.md#taglistmessagetypedef).

<a id="modify\_db\_cluster"></a>

### modify_db_cluster

Modify a setting for a DB cluster.

Type annotations for `session.create_client("neptune").modify_db_cluster`
method.

Boto3 documentation:
[Neptune.Client.modify_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_cluster)

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
- `OptionGroupName`: `str`
- `PreferredBackupWindow`: `str`
- `PreferredMaintenanceWindow`: `str`
- `EnableIAMDatabaseAuthentication`: `bool`
- `CloudwatchLogsExportConfiguration`:
  [CloudwatchLogsExportConfigurationTypeDef](./type_defs.md#cloudwatchlogsexportconfigurationtypedef)
- `EngineVersion`: `str`
- `AllowMajorVersionUpgrade`: `bool`
- `DBInstanceParameterGroupName`: `str`
- `DeletionProtection`: `bool`
- `CopyTagsToSnapshot`: `bool`

Returns a `Coroutine` for
[ModifyDBClusterResultTypeDef](./type_defs.md#modifydbclusterresulttypedef).

<a id="modify\_db\_cluster\_endpoint"></a>

### modify_db_cluster_endpoint

Modifies the properties of an endpoint in an Amazon Neptune DB cluster.

Type annotations for
`session.create_client("neptune").modify_db_cluster_endpoint` method.

Boto3 documentation:
[Neptune.Client.modify_db_cluster_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_cluster_endpoint)

Asynchronous method. Use `await modify_db_cluster_endpoint(...)` for a
synchronous call.

Arguments mapping described in
[ModifyDBClusterEndpointMessageRequestTypeDef](./type_defs.md#modifydbclusterendpointmessagerequesttypedef).

Keyword-only arguments:

- `DBClusterEndpointIdentifier`: `str` *(required)*
- `EndpointType`: `str`
- `StaticMembers`: `Sequence`\[`str`\]
- `ExcludedMembers`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[ModifyDBClusterEndpointOutputTypeDef](./type_defs.md#modifydbclusterendpointoutputtypedef).

<a id="modify\_db\_cluster\_parameter\_group"></a>

### modify_db_cluster_parameter_group

Modifies the parameters of a DB cluster parameter group.

Type annotations for
`session.create_client("neptune").modify_db_cluster_parameter_group` method.

Boto3 documentation:
[Neptune.Client.modify_db_cluster_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_cluster_parameter_group)

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

<a id="modify\_db\_cluster\_snapshot\_attribute"></a>

### modify_db_cluster_snapshot_attribute

Adds an attribute and values to, or removes an attribute and values from, a
manual DB cluster snapshot.

Type annotations for
`session.create_client("neptune").modify_db_cluster_snapshot_attribute` method.

Boto3 documentation:
[Neptune.Client.modify_db_cluster_snapshot_attribute](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_cluster_snapshot_attribute)

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

<a id="modify\_db\_instance"></a>

### modify_db_instance

Modifies settings for a DB instance.

Type annotations for `session.create_client("neptune").modify_db_instance`
method.

Boto3 documentation:
[Neptune.Client.modify_db_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_instance)

Asynchronous method. Use `await modify_db_instance(...)` for a synchronous
call.

Arguments mapping described in
[ModifyDBInstanceMessageRequestTypeDef](./type_defs.md#modifydbinstancemessagerequesttypedef).

Keyword-only arguments:

- `DBInstanceIdentifier`: `str` *(required)*
- `AllocatedStorage`: `int`
- `DBInstanceClass`: `str`
- `DBSubnetGroupName`: `str`
- `DBSecurityGroups`: `Sequence`\[`str`\]
- `VpcSecurityGroupIds`: `Sequence`\[`str`\]
- `ApplyImmediately`: `bool`
- `MasterUserPassword`: `str`
- `DBParameterGroupName`: `str`
- `BackupRetentionPeriod`: `int`
- `PreferredBackupWindow`: `str`
- `PreferredMaintenanceWindow`: `str`
- `MultiAZ`: `bool`
- `EngineVersion`: `str`
- `AllowMajorVersionUpgrade`: `bool`
- `AutoMinorVersionUpgrade`: `bool`
- `LicenseModel`: `str`
- `Iops`: `int`
- `OptionGroupName`: `str`
- `NewDBInstanceIdentifier`: `str`
- `StorageType`: `str`
- `TdeCredentialArn`: `str`
- `TdeCredentialPassword`: `str`
- `CACertificateIdentifier`: `str`
- `Domain`: `str`
- `CopyTagsToSnapshot`: `bool`
- `MonitoringInterval`: `int`
- `DBPortNumber`: `int`
- `PubliclyAccessible`: `bool`
- `MonitoringRoleArn`: `str`
- `DomainIAMRoleName`: `str`
- `PromotionTier`: `int`
- `EnableIAMDatabaseAuthentication`: `bool`
- `EnablePerformanceInsights`: `bool`
- `PerformanceInsightsKMSKeyId`: `str`
- `CloudwatchLogsExportConfiguration`:
  [CloudwatchLogsExportConfigurationTypeDef](./type_defs.md#cloudwatchlogsexportconfigurationtypedef)
- `DeletionProtection`: `bool`

Returns a `Coroutine` for
[ModifyDBInstanceResultTypeDef](./type_defs.md#modifydbinstanceresulttypedef).

<a id="modify\_db\_parameter\_group"></a>

### modify_db_parameter_group

Modifies the parameters of a DB parameter group.

Type annotations for
`session.create_client("neptune").modify_db_parameter_group` method.

Boto3 documentation:
[Neptune.Client.modify_db_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_parameter_group)

Asynchronous method. Use `await modify_db_parameter_group(...)` for a
synchronous call.

Arguments mapping described in
[ModifyDBParameterGroupMessageRequestTypeDef](./type_defs.md#modifydbparametergroupmessagerequesttypedef).

Keyword-only arguments:

- `DBParameterGroupName`: `str` *(required)*
- `Parameters`:
  `Sequence`\[[ParameterTypeDef](./type_defs.md#parametertypedef)\]
  *(required)*

Returns a `Coroutine` for
[DBParameterGroupNameMessageTypeDef](./type_defs.md#dbparametergroupnamemessagetypedef).

<a id="modify\_db\_subnet\_group"></a>

### modify_db_subnet_group

Modifies an existing DB subnet group.

Type annotations for `session.create_client("neptune").modify_db_subnet_group`
method.

Boto3 documentation:
[Neptune.Client.modify_db_subnet_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_db_subnet_group)

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

<a id="modify\_event\_subscription"></a>

### modify_event_subscription

Modifies an existing event notification subscription.

Type annotations for
`session.create_client("neptune").modify_event_subscription` method.

Boto3 documentation:
[Neptune.Client.modify_event_subscription](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.modify_event_subscription)

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

<a id="promote\_read\_replica\_db\_cluster"></a>

### promote_read_replica_db_cluster

Not supported.

Type annotations for
`session.create_client("neptune").promote_read_replica_db_cluster` method.

Boto3 documentation:
[Neptune.Client.promote_read_replica_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.promote_read_replica_db_cluster)

Asynchronous method. Use `await promote_read_replica_db_cluster(...)` for a
synchronous call.

Arguments mapping described in
[PromoteReadReplicaDBClusterMessageRequestTypeDef](./type_defs.md#promotereadreplicadbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[PromoteReadReplicaDBClusterResultTypeDef](./type_defs.md#promotereadreplicadbclusterresulttypedef).

<a id="reboot\_db\_instance"></a>

### reboot_db_instance

You might need to reboot your DB instance, usually for maintenance reasons.

Type annotations for `session.create_client("neptune").reboot_db_instance`
method.

Boto3 documentation:
[Neptune.Client.reboot_db_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.reboot_db_instance)

Asynchronous method. Use `await reboot_db_instance(...)` for a synchronous
call.

Arguments mapping described in
[RebootDBInstanceMessageRequestTypeDef](./type_defs.md#rebootdbinstancemessagerequesttypedef).

Keyword-only arguments:

- `DBInstanceIdentifier`: `str` *(required)*
- `ForceFailover`: `bool`

Returns a `Coroutine` for
[RebootDBInstanceResultTypeDef](./type_defs.md#rebootdbinstanceresulttypedef).

<a id="remove\_role\_from\_db\_cluster"></a>

### remove_role_from_db_cluster

Disassociates an Identity and Access Management (IAM) role from a DB cluster.

Type annotations for
`session.create_client("neptune").remove_role_from_db_cluster` method.

Boto3 documentation:
[Neptune.Client.remove_role_from_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.remove_role_from_db_cluster)

Asynchronous method. Use `await remove_role_from_db_cluster(...)` for a
synchronous call.

Arguments mapping described in
[RemoveRoleFromDBClusterMessageRequestTypeDef](./type_defs.md#removerolefromdbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*
- `RoleArn`: `str` *(required)*
- `FeatureName`: `str`

<a id="remove\_source\_identifier\_from\_subscription"></a>

### remove_source_identifier_from_subscription

Removes a source identifier from an existing event notification subscription.

Type annotations for
`session.create_client("neptune").remove_source_identifier_from_subscription`
method.

Boto3 documentation:
[Neptune.Client.remove_source_identifier_from_subscription](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.remove_source_identifier_from_subscription)

Asynchronous method. Use
`await remove_source_identifier_from_subscription(...)` for a synchronous call.

Arguments mapping described in
[RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef](./type_defs.md#removesourceidentifierfromsubscriptionmessagerequesttypedef).

Keyword-only arguments:

- `SubscriptionName`: `str` *(required)*
- `SourceIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[RemoveSourceIdentifierFromSubscriptionResultTypeDef](./type_defs.md#removesourceidentifierfromsubscriptionresulttypedef).

<a id="remove\_tags\_from\_resource"></a>

### remove_tags_from_resource

Removes metadata tags from an Amazon Neptune resource.

Type annotations for
`session.create_client("neptune").remove_tags_from_resource` method.

Boto3 documentation:
[Neptune.Client.remove_tags_from_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.remove_tags_from_resource)

Asynchronous method. Use `await remove_tags_from_resource(...)` for a
synchronous call.

Arguments mapping described in
[RemoveTagsFromResourceMessageRequestTypeDef](./type_defs.md#removetagsfromresourcemessagerequesttypedef).

Keyword-only arguments:

- `ResourceName`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

<a id="reset\_db\_cluster\_parameter\_group"></a>

### reset_db_cluster_parameter_group

Modifies the parameters of a DB cluster parameter group to the default value.

Type annotations for
`session.create_client("neptune").reset_db_cluster_parameter_group` method.

Boto3 documentation:
[Neptune.Client.reset_db_cluster_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.reset_db_cluster_parameter_group)

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

<a id="reset\_db\_parameter\_group"></a>

### reset_db_parameter_group

Modifies the parameters of a DB parameter group to the engine/system default
value.

Type annotations for
`session.create_client("neptune").reset_db_parameter_group` method.

Boto3 documentation:
[Neptune.Client.reset_db_parameter_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.reset_db_parameter_group)

Asynchronous method. Use `await reset_db_parameter_group(...)` for a
synchronous call.

Arguments mapping described in
[ResetDBParameterGroupMessageRequestTypeDef](./type_defs.md#resetdbparametergroupmessagerequesttypedef).

Keyword-only arguments:

- `DBParameterGroupName`: `str` *(required)*
- `ResetAllParameters`: `bool`
- `Parameters`:
  `Sequence`\[[ParameterTypeDef](./type_defs.md#parametertypedef)\]

Returns a `Coroutine` for
[DBParameterGroupNameMessageTypeDef](./type_defs.md#dbparametergroupnamemessagetypedef).

<a id="restore\_db\_cluster\_from\_snapshot"></a>

### restore_db_cluster_from_snapshot

Creates a new DB cluster from a DB snapshot or DB cluster snapshot.

Type annotations for
`session.create_client("neptune").restore_db_cluster_from_snapshot` method.

Boto3 documentation:
[Neptune.Client.restore_db_cluster_from_snapshot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.restore_db_cluster_from_snapshot)

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
- `DatabaseName`: `str`
- `OptionGroupName`: `str`
- `VpcSecurityGroupIds`: `Sequence`\[`str`\]
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `KmsKeyId`: `str`
- `EnableIAMDatabaseAuthentication`: `bool`
- `EnableCloudwatchLogsExports`: `Sequence`\[`str`\]
- `DBClusterParameterGroupName`: `str`
- `DeletionProtection`: `bool`
- `CopyTagsToSnapshot`: `bool`

Returns a `Coroutine` for
[RestoreDBClusterFromSnapshotResultTypeDef](./type_defs.md#restoredbclusterfromsnapshotresulttypedef).

<a id="restore\_db\_cluster\_to\_point\_in\_time"></a>

### restore_db_cluster_to_point_in_time

Restores a DB cluster to an arbitrary point in time.

Type annotations for
`session.create_client("neptune").restore_db_cluster_to_point_in_time` method.

Boto3 documentation:
[Neptune.Client.restore_db_cluster_to_point_in_time](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.restore_db_cluster_to_point_in_time)

Asynchronous method. Use `await restore_db_cluster_to_point_in_time(...)` for a
synchronous call.

Arguments mapping described in
[RestoreDBClusterToPointInTimeMessageRequestTypeDef](./type_defs.md#restoredbclustertopointintimemessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*
- `SourceDBClusterIdentifier`: `str` *(required)*
- `RestoreType`: `str`
- `RestoreToTime`: `Union`\[`datetime`, `str`\]
- `UseLatestRestorableTime`: `bool`
- `Port`: `int`
- `DBSubnetGroupName`: `str`
- `OptionGroupName`: `str`
- `VpcSecurityGroupIds`: `Sequence`\[`str`\]
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `KmsKeyId`: `str`
- `EnableIAMDatabaseAuthentication`: `bool`
- `EnableCloudwatchLogsExports`: `Sequence`\[`str`\]
- `DBClusterParameterGroupName`: `str`
- `DeletionProtection`: `bool`

Returns a `Coroutine` for
[RestoreDBClusterToPointInTimeResultTypeDef](./type_defs.md#restoredbclustertopointintimeresulttypedef).

<a id="start\_db\_cluster"></a>

### start_db_cluster

Starts an Amazon Neptune DB cluster that was stopped using the Amazon console,
the Amazon CLI stop-db-cluster command, or the StopDBCluster API.

Type annotations for `session.create_client("neptune").start_db_cluster`
method.

Boto3 documentation:
[Neptune.Client.start_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.start_db_cluster)

Asynchronous method. Use `await start_db_cluster(...)` for a synchronous call.

Arguments mapping described in
[StartDBClusterMessageRequestTypeDef](./type_defs.md#startdbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[StartDBClusterResultTypeDef](./type_defs.md#startdbclusterresulttypedef).

<a id="stop\_db\_cluster"></a>

### stop_db_cluster

Stops an Amazon Neptune DB cluster.

Type annotations for `session.create_client("neptune").stop_db_cluster` method.

Boto3 documentation:
[Neptune.Client.stop_db_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.stop_db_cluster)

Asynchronous method. Use `await stop_db_cluster(...)` for a synchronous call.

Arguments mapping described in
[StopDBClusterMessageRequestTypeDef](./type_defs.md#stopdbclustermessagerequesttypedef).

Keyword-only arguments:

- `DBClusterIdentifier`: `str` *(required)*

Returns a `Coroutine` for
[StopDBClusterResultTypeDef](./type_defs.md#stopdbclusterresulttypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("neptune").__aenter__` method.

Boto3 documentation:
[Neptune.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [NeptuneClient](#neptuneclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("neptune").__aexit__` method.

Boto3 documentation:
[Neptune.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("neptune").get_paginator` method
with overloads.

- `client.get_paginator("describe_db_cluster_endpoints")` ->
  [DescribeDBClusterEndpointsPaginator](./paginators.md#describedbclusterendpointspaginator)
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
- `client.get_paginator("describe_db_parameter_groups")` ->
  [DescribeDBParameterGroupsPaginator](./paginators.md#describedbparametergroupspaginator)
- `client.get_paginator("describe_db_parameters")` ->
  [DescribeDBParametersPaginator](./paginators.md#describedbparameterspaginator)
- `client.get_paginator("describe_db_subnet_groups")` ->
  [DescribeDBSubnetGroupsPaginator](./paginators.md#describedbsubnetgroupspaginator)
- `client.get_paginator("describe_engine_default_parameters")` ->
  [DescribeEngineDefaultParametersPaginator](./paginators.md#describeenginedefaultparameterspaginator)
- `client.get_paginator("describe_event_subscriptions")` ->
  [DescribeEventSubscriptionsPaginator](./paginators.md#describeeventsubscriptionspaginator)
- `client.get_paginator("describe_events")` ->
  [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
- `client.get_paginator("describe_orderable_db_instance_options")` ->
  [DescribeOrderableDBInstanceOptionsPaginator](./paginators.md#describeorderabledbinstanceoptionspaginator)
- `client.get_paginator("describe_pending_maintenance_actions")` ->
  [DescribePendingMaintenanceActionsPaginator](./paginators.md#describependingmaintenanceactionspaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("neptune").get_waiter` method with
overloads.

- `client.get_waiter("db_instance_available")` ->
  [DBInstanceAvailableWaiter](./waiters.md#dbinstanceavailablewaiter)
- `client.get_waiter("db_instance_deleted")` ->
  [DBInstanceDeletedWaiter](./waiters.md#dbinstancedeletedwaiter)
