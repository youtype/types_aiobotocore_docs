# EFSClient

> [Index](../README.md) > [EFS](./README.md) > EFSClient

!!! note ""

    Auto-generated documentation for [EFS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#efs)
    type annotations stubs module [types-aiobotocore-efs](https://pypi.org/project/types-aiobotocore-efs/).

## EFSClient

Type annotations and code completion for `#!python session.create_client("efs")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client)

```python
# EFSClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_efs.client import EFSClient

session = get_session()
async with session.create_client("efs") as client:
    client: EFSClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("efs").exceptions` structure.

```python
# EFSClient.exceptions usage example

async with session.create_client("efs") as client:
    try:
        do_something(client)
    except (
            client.AccessPointAlreadyExists,
        client.AccessPointLimitExceeded,
        client.AccessPointNotFound,
        client.AvailabilityZonesMismatch,
        client.BadRequest,
        client.ClientError,
        client.ConflictException,
        client.DependencyTimeout,
        client.FileSystemAlreadyExists,
        client.FileSystemInUse,
        client.FileSystemLimitExceeded,
        client.FileSystemNotFound,
        client.IncorrectFileSystemLifeCycleState,
        client.IncorrectMountTargetState,
        client.InsufficientThroughputCapacity,
        client.InternalServerError,
        client.InvalidPolicyException,
        client.IpAddressInUse,
        client.MountTargetConflict,
        client.MountTargetNotFound,
        client.NetworkInterfaceLimitExceeded,
        client.NoFreeAddressesInSubnet,
        client.PolicyNotFound,
        client.ReplicationAlreadyExists,
        client.ReplicationNotFound,
        client.SecurityGroupLimitExceeded,
        client.SecurityGroupNotFound,
        client.SubnetNotFound,
        client.ThrottlingException,
        client.ThroughputLimitExceeded,
        client.TooManyRequests,
        client.UnsupportedAvailabilityZone,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# EFSClient usage type checking example

from types_aiobotocore_efs.client import Exceptions

def handle_error(exc: Exceptions.AccessPointAlreadyExists) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("efs").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("efs").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### close



Type annotations and code completion for `#!python session.create_client("efs").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_access\_point

Creates an EFS access point.

Type annotations and code completion for `#!python session.create_client("efs").create_access_point` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/create_access_point.html)

```python
# create_access_point method definition

await def create_access_point(
    self,
    *,
    ClientToken: str,
    FileSystemId: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    PosixUser: PosixUserTypeDef = ...,  # (2)
    RootDirectory: RootDirectoryTypeDef = ...,  # (3)
) -> AccessPointDescriptionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: PosixUserTypeDef](./type_defs.md#posixusertypedef) 
3. See [:material-code-braces: RootDirectoryTypeDef](./type_defs.md#rootdirectorytypedef) 
4. See [:material-code-braces: AccessPointDescriptionResponseTypeDef](./type_defs.md#accesspointdescriptionresponsetypedef) 


```python
# create_access_point method usage example with argument unpacking

kwargs: CreateAccessPointRequestRequestTypeDef = {  # (1)
    "ClientToken": ...,
    "FileSystemId": ...,
}

parent.create_access_point(**kwargs)
```

1. See [:material-code-braces: CreateAccessPointRequestRequestTypeDef](./type_defs.md#createaccesspointrequestrequesttypedef) 

### create\_file\_system

Creates a new, empty file system.

Type annotations and code completion for `#!python session.create_client("efs").create_file_system` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/create_file_system.html)

```python
# create_file_system method definition

await def create_file_system(
    self,
    *,
    CreationToken: str,
    PerformanceMode: PerformanceModeType = ...,  # (1)
    Encrypted: bool = ...,
    KmsKeyId: str = ...,
    ThroughputMode: ThroughputModeType = ...,  # (2)
    ProvisionedThroughputInMibps: float = ...,
    AvailabilityZoneName: str = ...,
    Backup: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> FileSystemDescriptionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: PerformanceModeType](./literals.md#performancemodetype) 
2. See [:material-code-brackets: ThroughputModeType](./literals.md#throughputmodetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: FileSystemDescriptionResponseTypeDef](./type_defs.md#filesystemdescriptionresponsetypedef) 


```python
# create_file_system method usage example with argument unpacking

kwargs: CreateFileSystemRequestRequestTypeDef = {  # (1)
    "CreationToken": ...,
}

parent.create_file_system(**kwargs)
```

1. See [:material-code-braces: CreateFileSystemRequestRequestTypeDef](./type_defs.md#createfilesystemrequestrequesttypedef) 

### create\_mount\_target

Creates a mount target for a file system.

Type annotations and code completion for `#!python session.create_client("efs").create_mount_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/create_mount_target.html)

```python
# create_mount_target method definition

await def create_mount_target(
    self,
    *,
    FileSystemId: str,
    SubnetId: str,
    IpAddress: str = ...,
    SecurityGroups: Sequence[str] = ...,
) -> MountTargetDescriptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: MountTargetDescriptionResponseTypeDef](./type_defs.md#mounttargetdescriptionresponsetypedef) 


```python
# create_mount_target method usage example with argument unpacking

kwargs: CreateMountTargetRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
    "SubnetId": ...,
}

parent.create_mount_target(**kwargs)
```

1. See [:material-code-braces: CreateMountTargetRequestRequestTypeDef](./type_defs.md#createmounttargetrequestrequesttypedef) 

### create\_replication\_configuration

Creates a replication conﬁguration to either a new or existing EFS file system.

Type annotations and code completion for `#!python session.create_client("efs").create_replication_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/create_replication_configuration.html)

```python
# create_replication_configuration method definition

await def create_replication_configuration(
    self,
    *,
    SourceFileSystemId: str,
    Destinations: Sequence[DestinationToCreateTypeDef],  # (1)
) -> ReplicationConfigurationDescriptionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DestinationToCreateTypeDef](./type_defs.md#destinationtocreatetypedef) 
2. See [:material-code-braces: ReplicationConfigurationDescriptionResponseTypeDef](./type_defs.md#replicationconfigurationdescriptionresponsetypedef) 


```python
# create_replication_configuration method usage example with argument unpacking

kwargs: CreateReplicationConfigurationRequestRequestTypeDef = {  # (1)
    "SourceFileSystemId": ...,
    "Destinations": ...,
}

parent.create_replication_configuration(**kwargs)
```

1. See [:material-code-braces: CreateReplicationConfigurationRequestRequestTypeDef](./type_defs.md#createreplicationconfigurationrequestrequesttypedef) 

### create\_tags

DEPRECATED - <code>CreateTags</code> is deprecated and not maintained.

Type annotations and code completion for `#!python session.create_client("efs").create_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/create_tags.html)

```python
# create_tags method definition

await def create_tags(
    self,
    *,
    FileSystemId: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_tags method usage example with argument unpacking

kwargs: CreateTagsRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
    "Tags": ...,
}

parent.create_tags(**kwargs)
```

1. See [:material-code-braces: CreateTagsRequestRequestTypeDef](./type_defs.md#createtagsrequestrequesttypedef) 

### delete\_access\_point

Deletes the specified access point.

Type annotations and code completion for `#!python session.create_client("efs").delete_access_point` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/delete_access_point.html)

```python
# delete_access_point method definition

await def delete_access_point(
    self,
    *,
    AccessPointId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_access_point method usage example with argument unpacking

kwargs: DeleteAccessPointRequestRequestTypeDef = {  # (1)
    "AccessPointId": ...,
}

parent.delete_access_point(**kwargs)
```

1. See [:material-code-braces: DeleteAccessPointRequestRequestTypeDef](./type_defs.md#deleteaccesspointrequestrequesttypedef) 

### delete\_file\_system

Deletes a file system, permanently severing access to its contents.

Type annotations and code completion for `#!python session.create_client("efs").delete_file_system` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/delete_file_system.html)

```python
# delete_file_system method definition

await def delete_file_system(
    self,
    *,
    FileSystemId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_file_system method usage example with argument unpacking

kwargs: DeleteFileSystemRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.delete_file_system(**kwargs)
```

1. See [:material-code-braces: DeleteFileSystemRequestRequestTypeDef](./type_defs.md#deletefilesystemrequestrequesttypedef) 

### delete\_file\_system\_policy

Deletes the <code>FileSystemPolicy</code> for the specified file system.

Type annotations and code completion for `#!python session.create_client("efs").delete_file_system_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/delete_file_system_policy.html)

```python
# delete_file_system_policy method definition

await def delete_file_system_policy(
    self,
    *,
    FileSystemId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_file_system_policy method usage example with argument unpacking

kwargs: DeleteFileSystemPolicyRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.delete_file_system_policy(**kwargs)
```

1. See [:material-code-braces: DeleteFileSystemPolicyRequestRequestTypeDef](./type_defs.md#deletefilesystempolicyrequestrequesttypedef) 

### delete\_mount\_target

Deletes the specified mount target.

Type annotations and code completion for `#!python session.create_client("efs").delete_mount_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/delete_mount_target.html)

```python
# delete_mount_target method definition

await def delete_mount_target(
    self,
    *,
    MountTargetId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_mount_target method usage example with argument unpacking

kwargs: DeleteMountTargetRequestRequestTypeDef = {  # (1)
    "MountTargetId": ...,
}

parent.delete_mount_target(**kwargs)
```

1. See [:material-code-braces: DeleteMountTargetRequestRequestTypeDef](./type_defs.md#deletemounttargetrequestrequesttypedef) 

### delete\_replication\_configuration

Deletes a replication configuration.

Type annotations and code completion for `#!python session.create_client("efs").delete_replication_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/delete_replication_configuration.html)

```python
# delete_replication_configuration method definition

await def delete_replication_configuration(
    self,
    *,
    SourceFileSystemId: str,
    DeletionMode: DeletionModeType = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DeletionModeType](./literals.md#deletionmodetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_replication_configuration method usage example with argument unpacking

kwargs: DeleteReplicationConfigurationRequestRequestTypeDef = {  # (1)
    "SourceFileSystemId": ...,
}

parent.delete_replication_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteReplicationConfigurationRequestRequestTypeDef](./type_defs.md#deletereplicationconfigurationrequestrequesttypedef) 

### delete\_tags

DEPRECATED - <code>DeleteTags</code> is deprecated and not maintained.

Type annotations and code completion for `#!python session.create_client("efs").delete_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/delete_tags.html)

```python
# delete_tags method definition

await def delete_tags(
    self,
    *,
    FileSystemId: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_tags method usage example with argument unpacking

kwargs: DeleteTagsRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
    "TagKeys": ...,
}

parent.delete_tags(**kwargs)
```

1. See [:material-code-braces: DeleteTagsRequestRequestTypeDef](./type_defs.md#deletetagsrequestrequesttypedef) 

### describe\_access\_points

Returns the description of a specific Amazon EFS access point if the
<code>AccessPointId</code> is provided.

Type annotations and code completion for `#!python session.create_client("efs").describe_access_points` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/describe_access_points.html)

```python
# describe_access_points method definition

await def describe_access_points(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    AccessPointId: str = ...,
    FileSystemId: str = ...,
) -> DescribeAccessPointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccessPointsResponseTypeDef](./type_defs.md#describeaccesspointsresponsetypedef) 


```python
# describe_access_points method usage example with argument unpacking

kwargs: DescribeAccessPointsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.describe_access_points(**kwargs)
```

1. See [:material-code-braces: DescribeAccessPointsRequestRequestTypeDef](./type_defs.md#describeaccesspointsrequestrequesttypedef) 

### describe\_account\_preferences

Returns the account preferences settings for the Amazon Web Services account
associated with the user making the request, in the current Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("efs").describe_account_preferences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/describe_account_preferences.html)

```python
# describe_account_preferences method definition

await def describe_account_preferences(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeAccountPreferencesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountPreferencesResponseTypeDef](./type_defs.md#describeaccountpreferencesresponsetypedef) 


```python
# describe_account_preferences method usage example with argument unpacking

kwargs: DescribeAccountPreferencesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.describe_account_preferences(**kwargs)
```

1. See [:material-code-braces: DescribeAccountPreferencesRequestRequestTypeDef](./type_defs.md#describeaccountpreferencesrequestrequesttypedef) 

### describe\_backup\_policy

Returns the backup policy for the specified EFS file system.

Type annotations and code completion for `#!python session.create_client("efs").describe_backup_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/describe_backup_policy.html)

```python
# describe_backup_policy method definition

await def describe_backup_policy(
    self,
    *,
    FileSystemId: str,
) -> BackupPolicyDescriptionTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BackupPolicyDescriptionTypeDef](./type_defs.md#backuppolicydescriptiontypedef) 


```python
# describe_backup_policy method usage example with argument unpacking

kwargs: DescribeBackupPolicyRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.describe_backup_policy(**kwargs)
```

1. See [:material-code-braces: DescribeBackupPolicyRequestRequestTypeDef](./type_defs.md#describebackuppolicyrequestrequesttypedef) 

### describe\_file\_system\_policy

Returns the <code>FileSystemPolicy</code> for the specified EFS file system.

Type annotations and code completion for `#!python session.create_client("efs").describe_file_system_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/describe_file_system_policy.html)

```python
# describe_file_system_policy method definition

await def describe_file_system_policy(
    self,
    *,
    FileSystemId: str,
) -> FileSystemPolicyDescriptionTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: FileSystemPolicyDescriptionTypeDef](./type_defs.md#filesystempolicydescriptiontypedef) 


```python
# describe_file_system_policy method usage example with argument unpacking

kwargs: DescribeFileSystemPolicyRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.describe_file_system_policy(**kwargs)
```

1. See [:material-code-braces: DescribeFileSystemPolicyRequestRequestTypeDef](./type_defs.md#describefilesystempolicyrequestrequesttypedef) 

### describe\_file\_systems

Returns the description of a specific Amazon EFS file system if either the file
system <code>CreationToken</code> or the <code>FileSystemId</code> is provided.

Type annotations and code completion for `#!python session.create_client("efs").describe_file_systems` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/describe_file_systems.html)

```python
# describe_file_systems method definition

await def describe_file_systems(
    self,
    *,
    MaxItems: int = ...,
    Marker: str = ...,
    CreationToken: str = ...,
    FileSystemId: str = ...,
) -> DescribeFileSystemsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFileSystemsResponseTypeDef](./type_defs.md#describefilesystemsresponsetypedef) 


```python
# describe_file_systems method usage example with argument unpacking

kwargs: DescribeFileSystemsRequestRequestTypeDef = {  # (1)
    "MaxItems": ...,
}

parent.describe_file_systems(**kwargs)
```

1. See [:material-code-braces: DescribeFileSystemsRequestRequestTypeDef](./type_defs.md#describefilesystemsrequestrequesttypedef) 

### describe\_lifecycle\_configuration

Returns the current <code>LifecycleConfiguration</code> object for the
specified Amazon EFS file system.

Type annotations and code completion for `#!python session.create_client("efs").describe_lifecycle_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/describe_lifecycle_configuration.html)

```python
# describe_lifecycle_configuration method definition

await def describe_lifecycle_configuration(
    self,
    *,
    FileSystemId: str,
) -> LifecycleConfigurationDescriptionTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: LifecycleConfigurationDescriptionTypeDef](./type_defs.md#lifecycleconfigurationdescriptiontypedef) 


```python
# describe_lifecycle_configuration method usage example with argument unpacking

kwargs: DescribeLifecycleConfigurationRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.describe_lifecycle_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#describelifecycleconfigurationrequestrequesttypedef) 

### describe\_mount\_target\_security\_groups

Returns the security groups currently in effect for a mount target.

Type annotations and code completion for `#!python session.create_client("efs").describe_mount_target_security_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/describe_mount_target_security_groups.html)

```python
# describe_mount_target_security_groups method definition

await def describe_mount_target_security_groups(
    self,
    *,
    MountTargetId: str,
) -> DescribeMountTargetSecurityGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMountTargetSecurityGroupsResponseTypeDef](./type_defs.md#describemounttargetsecuritygroupsresponsetypedef) 


```python
# describe_mount_target_security_groups method usage example with argument unpacking

kwargs: DescribeMountTargetSecurityGroupsRequestRequestTypeDef = {  # (1)
    "MountTargetId": ...,
}

parent.describe_mount_target_security_groups(**kwargs)
```

1. See [:material-code-braces: DescribeMountTargetSecurityGroupsRequestRequestTypeDef](./type_defs.md#describemounttargetsecuritygroupsrequestrequesttypedef) 

### describe\_mount\_targets

Returns the descriptions of all the current mount targets, or a specific mount
target, for a file system.

Type annotations and code completion for `#!python session.create_client("efs").describe_mount_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/describe_mount_targets.html)

```python
# describe_mount_targets method definition

await def describe_mount_targets(
    self,
    *,
    MaxItems: int = ...,
    Marker: str = ...,
    FileSystemId: str = ...,
    MountTargetId: str = ...,
    AccessPointId: str = ...,
) -> DescribeMountTargetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMountTargetsResponseTypeDef](./type_defs.md#describemounttargetsresponsetypedef) 


```python
# describe_mount_targets method usage example with argument unpacking

kwargs: DescribeMountTargetsRequestRequestTypeDef = {  # (1)
    "MaxItems": ...,
}

parent.describe_mount_targets(**kwargs)
```

1. See [:material-code-braces: DescribeMountTargetsRequestRequestTypeDef](./type_defs.md#describemounttargetsrequestrequesttypedef) 

### describe\_replication\_configurations

Retrieves the replication configuration for a specific file system.

Type annotations and code completion for `#!python session.create_client("efs").describe_replication_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/describe_replication_configurations.html)

```python
# describe_replication_configurations method definition

await def describe_replication_configurations(
    self,
    *,
    FileSystemId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeReplicationConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReplicationConfigurationsResponseTypeDef](./type_defs.md#describereplicationconfigurationsresponsetypedef) 


```python
# describe_replication_configurations method usage example with argument unpacking

kwargs: DescribeReplicationConfigurationsRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.describe_replication_configurations(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationConfigurationsRequestRequestTypeDef](./type_defs.md#describereplicationconfigurationsrequestrequesttypedef) 

### describe\_tags

DEPRECATED - The <code>DescribeTags</code> action is deprecated and not
maintained.

Type annotations and code completion for `#!python session.create_client("efs").describe_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/describe_tags.html)

```python
# describe_tags method definition

await def describe_tags(
    self,
    *,
    FileSystemId: str,
    MaxItems: int = ...,
    Marker: str = ...,
) -> DescribeTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef) 


```python
# describe_tags method usage example with argument unpacking

kwargs: DescribeTagsRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.describe_tags(**kwargs)
```

1. See [:material-code-braces: DescribeTagsRequestRequestTypeDef](./type_defs.md#describetagsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists all tags for a top-level EFS resource.

Type annotations and code completion for `#!python session.create_client("efs").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### modify\_mount\_target\_security\_groups

Modifies the set of security groups in effect for a mount target.

Type annotations and code completion for `#!python session.create_client("efs").modify_mount_target_security_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/modify_mount_target_security_groups.html)

```python
# modify_mount_target_security_groups method definition

await def modify_mount_target_security_groups(
    self,
    *,
    MountTargetId: str,
    SecurityGroups: Sequence[str] = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# modify_mount_target_security_groups method usage example with argument unpacking

kwargs: ModifyMountTargetSecurityGroupsRequestRequestTypeDef = {  # (1)
    "MountTargetId": ...,
}

parent.modify_mount_target_security_groups(**kwargs)
```

1. See [:material-code-braces: ModifyMountTargetSecurityGroupsRequestRequestTypeDef](./type_defs.md#modifymounttargetsecuritygroupsrequestrequesttypedef) 

### put\_account\_preferences

Use this operation to set the account preference in the current Amazon Web
Services Region to use long 17 character (63 bit) or short 8 character (32 bit)
resource IDs for new EFS file system and mount target resources.

Type annotations and code completion for `#!python session.create_client("efs").put_account_preferences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/put_account_preferences.html)

```python
# put_account_preferences method definition

await def put_account_preferences(
    self,
    *,
    ResourceIdType: ResourceIdTypeType,  # (1)
) -> PutAccountPreferencesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceIdTypeType](./literals.md#resourceidtypetype) 
2. See [:material-code-braces: PutAccountPreferencesResponseTypeDef](./type_defs.md#putaccountpreferencesresponsetypedef) 


```python
# put_account_preferences method usage example with argument unpacking

kwargs: PutAccountPreferencesRequestRequestTypeDef = {  # (1)
    "ResourceIdType": ...,
}

parent.put_account_preferences(**kwargs)
```

1. See [:material-code-braces: PutAccountPreferencesRequestRequestTypeDef](./type_defs.md#putaccountpreferencesrequestrequesttypedef) 

### put\_backup\_policy

Updates the file system's backup policy.

Type annotations and code completion for `#!python session.create_client("efs").put_backup_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/put_backup_policy.html)

```python
# put_backup_policy method definition

await def put_backup_policy(
    self,
    *,
    FileSystemId: str,
    BackupPolicy: BackupPolicyTypeDef,  # (1)
) -> BackupPolicyDescriptionTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BackupPolicyTypeDef](./type_defs.md#backuppolicytypedef) 
2. See [:material-code-braces: BackupPolicyDescriptionTypeDef](./type_defs.md#backuppolicydescriptiontypedef) 


```python
# put_backup_policy method usage example with argument unpacking

kwargs: PutBackupPolicyRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
    "BackupPolicy": ...,
}

parent.put_backup_policy(**kwargs)
```

1. See [:material-code-braces: PutBackupPolicyRequestRequestTypeDef](./type_defs.md#putbackuppolicyrequestrequesttypedef) 

### put\_file\_system\_policy

Applies an Amazon EFS <code>FileSystemPolicy</code> to an Amazon EFS file
system.

Type annotations and code completion for `#!python session.create_client("efs").put_file_system_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/put_file_system_policy.html)

```python
# put_file_system_policy method definition

await def put_file_system_policy(
    self,
    *,
    FileSystemId: str,
    Policy: str,
    BypassPolicyLockoutSafetyCheck: bool = ...,
) -> FileSystemPolicyDescriptionTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: FileSystemPolicyDescriptionTypeDef](./type_defs.md#filesystempolicydescriptiontypedef) 


```python
# put_file_system_policy method usage example with argument unpacking

kwargs: PutFileSystemPolicyRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
    "Policy": ...,
}

parent.put_file_system_policy(**kwargs)
```

1. See [:material-code-braces: PutFileSystemPolicyRequestRequestTypeDef](./type_defs.md#putfilesystempolicyrequestrequesttypedef) 

### put\_lifecycle\_configuration

Use this action to manage storage for your file system.

Type annotations and code completion for `#!python session.create_client("efs").put_lifecycle_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/put_lifecycle_configuration.html)

```python
# put_lifecycle_configuration method definition

await def put_lifecycle_configuration(
    self,
    *,
    FileSystemId: str,
    LifecyclePolicies: Sequence[LifecyclePolicyTypeDef],  # (1)
) -> LifecycleConfigurationDescriptionTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LifecyclePolicyTypeDef](./type_defs.md#lifecyclepolicytypedef) 
2. See [:material-code-braces: LifecycleConfigurationDescriptionTypeDef](./type_defs.md#lifecycleconfigurationdescriptiontypedef) 


```python
# put_lifecycle_configuration method usage example with argument unpacking

kwargs: PutLifecycleConfigurationRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
    "LifecyclePolicies": ...,
}

parent.put_lifecycle_configuration(**kwargs)
```

1. See [:material-code-braces: PutLifecycleConfigurationRequestRequestTypeDef](./type_defs.md#putlifecycleconfigurationrequestrequesttypedef) 

### tag\_resource

Creates a tag for an EFS resource.

Type annotations and code completion for `#!python session.create_client("efs").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceId: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from an EFS resource.

Type annotations and code completion for `#!python session.create_client("efs").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceId: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_file\_system

Updates the throughput mode or the amount of provisioned throughput of an
existing file system.

Type annotations and code completion for `#!python session.create_client("efs").update_file_system` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/update_file_system.html)

```python
# update_file_system method definition

await def update_file_system(
    self,
    *,
    FileSystemId: str,
    ThroughputMode: ThroughputModeType = ...,  # (1)
    ProvisionedThroughputInMibps: float = ...,
) -> FileSystemDescriptionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ThroughputModeType](./literals.md#throughputmodetype) 
2. See [:material-code-braces: FileSystemDescriptionResponseTypeDef](./type_defs.md#filesystemdescriptionresponsetypedef) 


```python
# update_file_system method usage example with argument unpacking

kwargs: UpdateFileSystemRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.update_file_system(**kwargs)
```

1. See [:material-code-braces: UpdateFileSystemRequestRequestTypeDef](./type_defs.md#updatefilesystemrequestrequesttypedef) 

### update\_file\_system\_protection

Updates protection on the file system.

Type annotations and code completion for `#!python session.create_client("efs").update_file_system_protection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/client/update_file_system_protection.html)

```python
# update_file_system_protection method definition

await def update_file_system_protection(
    self,
    *,
    FileSystemId: str,
    ReplicationOverwriteProtection: ReplicationOverwriteProtectionType = ...,  # (1)
) -> FileSystemProtectionDescriptionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ReplicationOverwriteProtectionType](./literals.md#replicationoverwriteprotectiontype) 
2. See [:material-code-braces: FileSystemProtectionDescriptionResponseTypeDef](./type_defs.md#filesystemprotectiondescriptionresponsetypedef) 


```python
# update_file_system_protection method usage example with argument unpacking

kwargs: UpdateFileSystemProtectionRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.update_file_system_protection(**kwargs)
```

1. See [:material-code-braces: UpdateFileSystemProtectionRequestRequestTypeDef](./type_defs.md#updatefilesystemprotectionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("efs").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "EFSClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("efs").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("efs").get_paginator` method with overloads.

- `client.get_paginator("describe_access_points")` -> [DescribeAccessPointsPaginator](./paginators.md#describeaccesspointspaginator)
- `client.get_paginator("describe_file_systems")` -> [DescribeFileSystemsPaginator](./paginators.md#describefilesystemspaginator)
- `client.get_paginator("describe_mount_targets")` -> [DescribeMountTargetsPaginator](./paginators.md#describemounttargetspaginator)
- `client.get_paginator("describe_replication_configurations")` -> [DescribeReplicationConfigurationsPaginator](./paginators.md#describereplicationconfigurationspaginator)
- `client.get_paginator("describe_tags")` -> [DescribeTagsPaginator](./paginators.md#describetagspaginator)



