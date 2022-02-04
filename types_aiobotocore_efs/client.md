<a id="efsclient-for-aiobotocore-efs-module"></a>

# EFSClient for aiobotocore EFS module

> [Index](..) > [EFS](.) > EFSClient

Auto-generated documentation for
[EFS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
type annotations stubs module
[types-aiobotocore-efs](https://pypi.org/project/types-aiobotocore-efs/).

- [EFSClient for aiobotocore EFS module](#efsclient-for-aiobotocore-efs-module)
  - [EFSClient](#efsclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_access_point](#create_access_point)
    - [create_file_system](#create_file_system)
    - [create_mount_target](#create_mount_target)
    - [create_tags](#create_tags)
    - [delete_access_point](#delete_access_point)
    - [delete_file_system](#delete_file_system)
    - [delete_file_system_policy](#delete_file_system_policy)
    - [delete_mount_target](#delete_mount_target)
    - [delete_tags](#delete_tags)
    - [describe_access_points](#describe_access_points)
    - [describe_account_preferences](#describe_account_preferences)
    - [describe_backup_policy](#describe_backup_policy)
    - [describe_file_system_policy](#describe_file_system_policy)
    - [describe_file_systems](#describe_file_systems)
    - [describe_lifecycle_configuration](#describe_lifecycle_configuration)
    - [describe_mount_target_security_groups](#describe_mount_target_security_groups)
    - [describe_mount_targets](#describe_mount_targets)
    - [describe_tags](#describe_tags)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [modify_mount_target_security_groups](#modify_mount_target_security_groups)
    - [put_account_preferences](#put_account_preferences)
    - [put_backup_policy](#put_backup_policy)
    - [put_file_system_policy](#put_file_system_policy)
    - [put_lifecycle_configuration](#put_lifecycle_configuration)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_file_system](#update_file_system)
    - [get_paginator](#get_paginator)

<a id="efsclient"></a>

## EFSClient

Type annotations for `aiobotocore.create_client("efs")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_efs.client import EFSClient

def get_efs_client() -> EFSClient:
    return Session().client("efs")
```

Boto3 documentation:
[EFS.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_efs.client import Exceptions

def handle_error(exc: Exceptions.AccessPointAlreadyExists) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessPointAlreadyExists`
- `Exceptions.AccessPointLimitExceeded`
- `Exceptions.AccessPointNotFound`
- `Exceptions.AvailabilityZonesMismatch`
- `Exceptions.BadRequest`
- `Exceptions.ClientError`
- `Exceptions.DependencyTimeout`
- `Exceptions.FileSystemAlreadyExists`
- `Exceptions.FileSystemInUse`
- `Exceptions.FileSystemLimitExceeded`
- `Exceptions.FileSystemNotFound`
- `Exceptions.IncorrectFileSystemLifeCycleState`
- `Exceptions.IncorrectMountTargetState`
- `Exceptions.InsufficientThroughputCapacity`
- `Exceptions.InternalServerError`
- `Exceptions.InvalidPolicyException`
- `Exceptions.IpAddressInUse`
- `Exceptions.MountTargetConflict`
- `Exceptions.MountTargetNotFound`
- `Exceptions.NetworkInterfaceLimitExceeded`
- `Exceptions.NoFreeAddressesInSubnet`
- `Exceptions.PolicyNotFound`
- `Exceptions.SecurityGroupLimitExceeded`
- `Exceptions.SecurityGroupNotFound`
- `Exceptions.SubnetNotFound`
- `Exceptions.ThroughputLimitExceeded`
- `Exceptions.TooManyRequests`
- `Exceptions.UnsupportedAvailabilityZone`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

EFSClient exceptions.

Type annotations for `aiobotocore.create_client("efs").exceptions` method.

Boto3 documentation:
[EFS.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("efs").can_paginate` method.

Boto3 documentation:
[EFS.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_access_point"></a>

### create_access_point

Creates an EFS access point.

Type annotations for `aiobotocore.create_client("efs").create_access_point`
method.

Boto3 documentation:
[EFS.Client.create_access_point](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_access_point)

Asynchronous method. Use `await create_access_point(...)` for a synchronous
call.

Arguments mapping described in
[CreateAccessPointRequestRequestTypeDef](./type_defs.md#createaccesspointrequestrequesttypedef).

Keyword-only arguments:

- `ClientToken`: `str` *(required)*
- `FileSystemId`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `PosixUser`: [PosixUserTypeDef](./type_defs.md#posixusertypedef)
- `RootDirectory`: [RootDirectoryTypeDef](./type_defs.md#rootdirectorytypedef)

Returns a `Coroutine` for
[AccessPointDescriptionResponseMetadataTypeDef](./type_defs.md#accesspointdescriptionresponsemetadatatypedef).

<a id="create_file_system"></a>

### create_file_system

Creates a new, empty file system.

Type annotations for `aiobotocore.create_client("efs").create_file_system`
method.

Boto3 documentation:
[EFS.Client.create_file_system](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_file_system)

Asynchronous method. Use `await create_file_system(...)` for a synchronous
call.

Arguments mapping described in
[CreateFileSystemRequestRequestTypeDef](./type_defs.md#createfilesystemrequestrequesttypedef).

Keyword-only arguments:

- `CreationToken`: `str` *(required)*
- `PerformanceMode`: [PerformanceModeType](./literals.md#performancemodetype)
- `Encrypted`: `bool`
- `KmsKeyId`: `str`
- `ThroughputMode`: [ThroughputModeType](./literals.md#throughputmodetype)
- `ProvisionedThroughputInMibps`: `float`
- `AvailabilityZoneName`: `str`
- `Backup`: `bool`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[FileSystemDescriptionResponseMetadataTypeDef](./type_defs.md#filesystemdescriptionresponsemetadatatypedef).

<a id="create_mount_target"></a>

### create_mount_target

Creates a mount target for a file system.

Type annotations for `aiobotocore.create_client("efs").create_mount_target`
method.

Boto3 documentation:
[EFS.Client.create_mount_target](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_mount_target)

Asynchronous method. Use `await create_mount_target(...)` for a synchronous
call.

Arguments mapping described in
[CreateMountTargetRequestRequestTypeDef](./type_defs.md#createmounttargetrequestrequesttypedef).

Keyword-only arguments:

- `FileSystemId`: `str` *(required)*
- `SubnetId`: `str` *(required)*
- `IpAddress`: `str`
- `SecurityGroups`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[MountTargetDescriptionResponseMetadataTypeDef](./type_defs.md#mounttargetdescriptionresponsemetadatatypedef).

<a id="create_tags"></a>

### create_tags

.

Type annotations for `aiobotocore.create_client("efs").create_tags` method.

Boto3 documentation:
[EFS.Client.create_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_tags)

Asynchronous method. Use `await create_tags(...)` for a synchronous call.

Arguments mapping described in
[CreateTagsRequestRequestTypeDef](./type_defs.md#createtagsrequestrequesttypedef).

Keyword-only arguments:

- `FileSystemId`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

<a id="delete_access_point"></a>

### delete_access_point

Deletes the specified access point.

Type annotations for `aiobotocore.create_client("efs").delete_access_point`
method.

Boto3 documentation:
[EFS.Client.delete_access_point](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.delete_access_point)

Asynchronous method. Use `await delete_access_point(...)` for a synchronous
call.

Arguments mapping described in
[DeleteAccessPointRequestRequestTypeDef](./type_defs.md#deleteaccesspointrequestrequesttypedef).

Keyword-only arguments:

- `AccessPointId`: `str` *(required)*

<a id="delete_file_system"></a>

### delete_file_system

Deletes a file system, permanently severing access to its contents.

Type annotations for `aiobotocore.create_client("efs").delete_file_system`
method.

Boto3 documentation:
[EFS.Client.delete_file_system](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.delete_file_system)

Asynchronous method. Use `await delete_file_system(...)` for a synchronous
call.

Arguments mapping described in
[DeleteFileSystemRequestRequestTypeDef](./type_defs.md#deletefilesystemrequestrequesttypedef).

Keyword-only arguments:

- `FileSystemId`: `str` *(required)*

<a id="delete_file_system_policy"></a>

### delete_file_system_policy

Deletes the `FileSystemPolicy` for the specified file system.

Type annotations for
`aiobotocore.create_client("efs").delete_file_system_policy` method.

Boto3 documentation:
[EFS.Client.delete_file_system_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.delete_file_system_policy)

Asynchronous method. Use `await delete_file_system_policy(...)` for a
synchronous call.

Arguments mapping described in
[DeleteFileSystemPolicyRequestRequestTypeDef](./type_defs.md#deletefilesystempolicyrequestrequesttypedef).

Keyword-only arguments:

- `FileSystemId`: `str` *(required)*

<a id="delete_mount_target"></a>

### delete_mount_target

Deletes the specified mount target.

Type annotations for `aiobotocore.create_client("efs").delete_mount_target`
method.

Boto3 documentation:
[EFS.Client.delete_mount_target](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.delete_mount_target)

Asynchronous method. Use `await delete_mount_target(...)` for a synchronous
call.

Arguments mapping described in
[DeleteMountTargetRequestRequestTypeDef](./type_defs.md#deletemounttargetrequestrequesttypedef).

Keyword-only arguments:

- `MountTargetId`: `str` *(required)*

<a id="delete_tags"></a>

### delete_tags

.

Type annotations for `aiobotocore.create_client("efs").delete_tags` method.

Boto3 documentation:
[EFS.Client.delete_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.delete_tags)

Asynchronous method. Use `await delete_tags(...)` for a synchronous call.

Arguments mapping described in
[DeleteTagsRequestRequestTypeDef](./type_defs.md#deletetagsrequestrequesttypedef).

Keyword-only arguments:

- `FileSystemId`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

<a id="describe_access_points"></a>

### describe_access_points

Returns the description of a specific Amazon EFS access point if the
`AccessPointId` is provided.

Type annotations for `aiobotocore.create_client("efs").describe_access_points`
method.

Boto3 documentation:
[EFS.Client.describe_access_points](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_access_points)

Asynchronous method. Use `await describe_access_points(...)` for a synchronous
call.

Arguments mapping described in
[DescribeAccessPointsRequestRequestTypeDef](./type_defs.md#describeaccesspointsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`
- `AccessPointId`: `str`
- `FileSystemId`: `str`

Returns a `Coroutine` for
[DescribeAccessPointsResponseTypeDef](./type_defs.md#describeaccesspointsresponsetypedef).

<a id="describe_account_preferences"></a>

### describe_account_preferences

Returns the account preferences settings for the Amazon Web Services account
associated with the user making the request, in the current Amazon Web Services
Region.

Type annotations for
`aiobotocore.create_client("efs").describe_account_preferences` method.

Boto3 documentation:
[EFS.Client.describe_account_preferences](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_account_preferences)

Asynchronous method. Use `await describe_account_preferences(...)` for a
synchronous call.

Arguments mapping described in
[DescribeAccountPreferencesRequestRequestTypeDef](./type_defs.md#describeaccountpreferencesrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[DescribeAccountPreferencesResponseTypeDef](./type_defs.md#describeaccountpreferencesresponsetypedef).

<a id="describe_backup_policy"></a>

### describe_backup_policy

Returns the backup policy for the specified EFS file system.

Type annotations for `aiobotocore.create_client("efs").describe_backup_policy`
method.

Boto3 documentation:
[EFS.Client.describe_backup_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_backup_policy)

Asynchronous method. Use `await describe_backup_policy(...)` for a synchronous
call.

Arguments mapping described in
[DescribeBackupPolicyRequestRequestTypeDef](./type_defs.md#describebackuppolicyrequestrequesttypedef).

Keyword-only arguments:

- `FileSystemId`: `str` *(required)*

Returns a `Coroutine` for
[BackupPolicyDescriptionTypeDef](./type_defs.md#backuppolicydescriptiontypedef).

<a id="describe_file_system_policy"></a>

### describe_file_system_policy

Returns the `FileSystemPolicy` for the specified EFS file system.

Type annotations for
`aiobotocore.create_client("efs").describe_file_system_policy` method.

Boto3 documentation:
[EFS.Client.describe_file_system_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_file_system_policy)

Asynchronous method. Use `await describe_file_system_policy(...)` for a
synchronous call.

Arguments mapping described in
[DescribeFileSystemPolicyRequestRequestTypeDef](./type_defs.md#describefilesystempolicyrequestrequesttypedef).

Keyword-only arguments:

- `FileSystemId`: `str` *(required)*

Returns a `Coroutine` for
[FileSystemPolicyDescriptionTypeDef](./type_defs.md#filesystempolicydescriptiontypedef).

<a id="describe_file_systems"></a>

### describe_file_systems

Returns the description of a specific Amazon EFS file system if either the file
system `CreationToken` or the `FileSystemId` is provided.

Type annotations for `aiobotocore.create_client("efs").describe_file_systems`
method.

Boto3 documentation:
[EFS.Client.describe_file_systems](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_file_systems)

Asynchronous method. Use `await describe_file_systems(...)` for a synchronous
call.

Arguments mapping described in
[DescribeFileSystemsRequestRequestTypeDef](./type_defs.md#describefilesystemsrequestrequesttypedef).

Keyword-only arguments:

- `MaxItems`: `int`
- `Marker`: `str`
- `CreationToken`: `str`
- `FileSystemId`: `str`

Returns a `Coroutine` for
[DescribeFileSystemsResponseTypeDef](./type_defs.md#describefilesystemsresponsetypedef).

<a id="describe_lifecycle_configuration"></a>

### describe_lifecycle_configuration

Returns the current `LifecycleConfiguration` object for the specified Amazon
EFS file system.

Type annotations for
`aiobotocore.create_client("efs").describe_lifecycle_configuration` method.

Boto3 documentation:
[EFS.Client.describe_lifecycle_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_lifecycle_configuration)

Asynchronous method. Use `await describe_lifecycle_configuration(...)` for a
synchronous call.

Arguments mapping described in
[DescribeLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#describelifecycleconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `FileSystemId`: `str` *(required)*

Returns a `Coroutine` for
[LifecycleConfigurationDescriptionTypeDef](./type_defs.md#lifecycleconfigurationdescriptiontypedef).

<a id="describe_mount_target_security_groups"></a>

### describe_mount_target_security_groups

Returns the security groups currently in effect for a mount target.

Type annotations for
`aiobotocore.create_client("efs").describe_mount_target_security_groups`
method.

Boto3 documentation:
[EFS.Client.describe_mount_target_security_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_mount_target_security_groups)

Asynchronous method. Use `await describe_mount_target_security_groups(...)` for
a synchronous call.

Arguments mapping described in
[DescribeMountTargetSecurityGroupsRequestRequestTypeDef](./type_defs.md#describemounttargetsecuritygroupsrequestrequesttypedef).

Keyword-only arguments:

- `MountTargetId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeMountTargetSecurityGroupsResponseTypeDef](./type_defs.md#describemounttargetsecuritygroupsresponsetypedef).

<a id="describe_mount_targets"></a>

### describe_mount_targets

Returns the descriptions of all the current mount targets, or a specific mount
target, for a file system.

Type annotations for `aiobotocore.create_client("efs").describe_mount_targets`
method.

Boto3 documentation:
[EFS.Client.describe_mount_targets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_mount_targets)

Asynchronous method. Use `await describe_mount_targets(...)` for a synchronous
call.

Arguments mapping described in
[DescribeMountTargetsRequestRequestTypeDef](./type_defs.md#describemounttargetsrequestrequesttypedef).

Keyword-only arguments:

- `MaxItems`: `int`
- `Marker`: `str`
- `FileSystemId`: `str`
- `MountTargetId`: `str`
- `AccessPointId`: `str`

Returns a `Coroutine` for
[DescribeMountTargetsResponseTypeDef](./type_defs.md#describemounttargetsresponsetypedef).

<a id="describe_tags"></a>

### describe_tags

.

Type annotations for `aiobotocore.create_client("efs").describe_tags` method.

Boto3 documentation:
[EFS.Client.describe_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_tags)

Asynchronous method. Use `await describe_tags(...)` for a synchronous call.

Arguments mapping described in
[DescribeTagsRequestRequestTypeDef](./type_defs.md#describetagsrequestrequesttypedef).

Keyword-only arguments:

- `FileSystemId`: `str` *(required)*
- `MaxItems`: `int`
- `Marker`: `str`

Returns a `Coroutine` for
[DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `aiobotocore.create_client("efs").generate_presigned_url`
method.

Boto3 documentation:
[EFS.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.generate_presigned_url)

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

Lists all tags for a top-level EFS resource.

Type annotations for `aiobotocore.create_client("efs").list_tags_for_resource`
method.

Boto3 documentation:
[EFS.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="modify_mount_target_security_groups"></a>

### modify_mount_target_security_groups

Modifies the set of security groups in effect for a mount target.

Type annotations for
`aiobotocore.create_client("efs").modify_mount_target_security_groups` method.

Boto3 documentation:
[EFS.Client.modify_mount_target_security_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.modify_mount_target_security_groups)

Asynchronous method. Use `await modify_mount_target_security_groups(...)` for a
synchronous call.

Arguments mapping described in
[ModifyMountTargetSecurityGroupsRequestRequestTypeDef](./type_defs.md#modifymounttargetsecuritygroupsrequestrequesttypedef).

Keyword-only arguments:

- `MountTargetId`: `str` *(required)*
- `SecurityGroups`: `Sequence`\[`str`\]

<a id="put_account_preferences"></a>

### put_account_preferences

Use this operation to set the account preference in the current Amazon Web
Services Region to use long 17 character (63 bit) or short 8 character (32 bit)
resource IDs for new EFS file system and mount target resources.

Type annotations for `aiobotocore.create_client("efs").put_account_preferences`
method.

Boto3 documentation:
[EFS.Client.put_account_preferences](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.put_account_preferences)

Asynchronous method. Use `await put_account_preferences(...)` for a synchronous
call.

Arguments mapping described in
[PutAccountPreferencesRequestRequestTypeDef](./type_defs.md#putaccountpreferencesrequestrequesttypedef).

Keyword-only arguments:

- `ResourceIdType`: [ResourceIdTypeType](./literals.md#resourceidtypetype)
  *(required)*

Returns a `Coroutine` for
[PutAccountPreferencesResponseTypeDef](./type_defs.md#putaccountpreferencesresponsetypedef).

<a id="put_backup_policy"></a>

### put_backup_policy

Updates the file system's backup policy.

Type annotations for `aiobotocore.create_client("efs").put_backup_policy`
method.

Boto3 documentation:
[EFS.Client.put_backup_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.put_backup_policy)

Asynchronous method. Use `await put_backup_policy(...)` for a synchronous call.

Arguments mapping described in
[PutBackupPolicyRequestRequestTypeDef](./type_defs.md#putbackuppolicyrequestrequesttypedef).

Keyword-only arguments:

- `FileSystemId`: `str` *(required)*
- `BackupPolicy`: [BackupPolicyTypeDef](./type_defs.md#backuppolicytypedef)
  *(required)*

Returns a `Coroutine` for
[BackupPolicyDescriptionTypeDef](./type_defs.md#backuppolicydescriptiontypedef).

<a id="put_file_system_policy"></a>

### put_file_system_policy

Applies an Amazon EFS `FileSystemPolicy` to an Amazon EFS file system.

Type annotations for `aiobotocore.create_client("efs").put_file_system_policy`
method.

Boto3 documentation:
[EFS.Client.put_file_system_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.put_file_system_policy)

Asynchronous method. Use `await put_file_system_policy(...)` for a synchronous
call.

Arguments mapping described in
[PutFileSystemPolicyRequestRequestTypeDef](./type_defs.md#putfilesystempolicyrequestrequesttypedef).

Keyword-only arguments:

- `FileSystemId`: `str` *(required)*
- `Policy`: `str` *(required)*
- `BypassPolicyLockoutSafetyCheck`: `bool`

Returns a `Coroutine` for
[FileSystemPolicyDescriptionTypeDef](./type_defs.md#filesystempolicydescriptiontypedef).

<a id="put_lifecycle_configuration"></a>

### put_lifecycle_configuration

Enables lifecycle management by creating a new `LifecycleConfiguration` object.

Type annotations for
`aiobotocore.create_client("efs").put_lifecycle_configuration` method.

Boto3 documentation:
[EFS.Client.put_lifecycle_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.put_lifecycle_configuration)

Asynchronous method. Use `await put_lifecycle_configuration(...)` for a
synchronous call.

Arguments mapping described in
[PutLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#putlifecycleconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `FileSystemId`: `str` *(required)*
- `LifecyclePolicies`:
  `Sequence`\[[LifecyclePolicyTypeDef](./type_defs.md#lifecyclepolicytypedef)\]
  *(required)*

Returns a `Coroutine` for
[LifecycleConfigurationDescriptionTypeDef](./type_defs.md#lifecycleconfigurationdescriptiontypedef).

<a id="tag_resource"></a>

### tag_resource

Creates a tag for an EFS resource.

Type annotations for `aiobotocore.create_client("efs").tag_resource` method.

Boto3 documentation:
[EFS.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceId`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

<a id="untag_resource"></a>

### untag_resource

Removes tags from an EFS resource.

Type annotations for `aiobotocore.create_client("efs").untag_resource` method.

Boto3 documentation:
[EFS.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceId`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

<a id="update_file_system"></a>

### update_file_system

Updates the throughput mode or the amount of provisioned throughput of an
existing file system.

Type annotations for `aiobotocore.create_client("efs").update_file_system`
method.

Boto3 documentation:
[EFS.Client.update_file_system](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.update_file_system)

Asynchronous method. Use `await update_file_system(...)` for a synchronous
call.

Arguments mapping described in
[UpdateFileSystemRequestRequestTypeDef](./type_defs.md#updatefilesystemrequestrequesttypedef).

Keyword-only arguments:

- `FileSystemId`: `str` *(required)*
- `ThroughputMode`: [ThroughputModeType](./literals.md#throughputmodetype)
- `ProvisionedThroughputInMibps`: `float`

Returns a `Coroutine` for
[FileSystemDescriptionResponseMetadataTypeDef](./type_defs.md#filesystemdescriptionresponsemetadatatypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("efs").get_paginator` method
with overloads.

- `client.get_paginator("describe_file_systems")` ->
  [DescribeFileSystemsPaginator](./paginators.md#describefilesystemspaginator)
- `client.get_paginator("describe_mount_targets")` ->
  [DescribeMountTargetsPaginator](./paginators.md#describemounttargetspaginator)
- `client.get_paginator("describe_tags")` ->
  [DescribeTagsPaginator](./paginators.md#describetagspaginator)
