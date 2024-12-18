# DataSyncClient

> [Index](../README.md) > [DataSync](./README.md) > DataSyncClient

!!! note ""

    Auto-generated documentation for [DataSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#datasync)
    type annotations stubs module [types-aiobotocore-datasync](https://pypi.org/project/types-aiobotocore-datasync/).

## DataSyncClient

Type annotations and code completion for `#!python session.create_client("datasync")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client)

```python
# DataSyncClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_datasync.client import DataSyncClient

session = get_session()
async with session.create_client("datasync") as client:
    client: DataSyncClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("datasync").exceptions` structure.

```python
# DataSyncClient.exceptions usage example

async with session.create_client("datasync") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalException,
        client.InvalidRequestException,
    ) as e:
        print(e)
```

```python
# DataSyncClient usage type checking example

from types_aiobotocore_datasync.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("datasync").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("datasync").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/generate_presigned_url.html)

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



Type annotations and code completion for `#!python session.create_client("datasync").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### add\_storage\_system

Creates an Amazon Web Services resource for an on-premises storage system that
you want DataSync Discovery to collect information about.

Type annotations and code completion for `#!python session.create_client("datasync").add_storage_system` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/add_storage_system.html)

```python
# add_storage_system method definition

await def add_storage_system(
    self,
    *,
    ServerConfiguration: DiscoveryServerConfigurationTypeDef,  # (1)
    SystemType: DiscoverySystemTypeType,  # (2)
    AgentArns: Sequence[str],
    ClientToken: str,
    Credentials: CredentialsTypeDef,  # (3)
    CloudWatchLogGroupArn: str = ...,
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (4)
    Name: str = ...,
) -> AddStorageSystemResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DiscoveryServerConfigurationTypeDef](./type_defs.md#discoveryserverconfigurationtypedef) 
2. See [:material-code-brackets: DiscoverySystemTypeType](./literals.md#discoverysystemtypetype) 
3. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
4. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
5. See [:material-code-braces: AddStorageSystemResponseTypeDef](./type_defs.md#addstoragesystemresponsetypedef) 


```python
# add_storage_system method usage example with argument unpacking

kwargs: AddStorageSystemRequestRequestTypeDef = {  # (1)
    "ServerConfiguration": ...,
    "SystemType": ...,
    "AgentArns": ...,
    "ClientToken": ...,
    "Credentials": ...,
}

parent.add_storage_system(**kwargs)
```

1. See [:material-code-braces: AddStorageSystemRequestRequestTypeDef](./type_defs.md#addstoragesystemrequestrequesttypedef) 

### cancel\_task\_execution

Stops an DataSync task execution that's in progress.

Type annotations and code completion for `#!python session.create_client("datasync").cancel_task_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/cancel_task_execution.html)

```python
# cancel_task_execution method definition

await def cancel_task_execution(
    self,
    *,
    TaskExecutionArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_task_execution method usage example with argument unpacking

kwargs: CancelTaskExecutionRequestRequestTypeDef = {  # (1)
    "TaskExecutionArn": ...,
}

parent.cancel_task_execution(**kwargs)
```

1. See [:material-code-braces: CancelTaskExecutionRequestRequestTypeDef](./type_defs.md#canceltaskexecutionrequestrequesttypedef) 

### create\_agent

Activates an DataSync agent that you deploy in your storage environment.

Type annotations and code completion for `#!python session.create_client("datasync").create_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/create_agent.html)

```python
# create_agent method definition

await def create_agent(
    self,
    *,
    ActivationKey: str,
    AgentName: str = ...,
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (1)
    VpcEndpointId: str = ...,
    SubnetArns: Sequence[str] = ...,
    SecurityGroupArns: Sequence[str] = ...,
) -> CreateAgentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
2. See [:material-code-braces: CreateAgentResponseTypeDef](./type_defs.md#createagentresponsetypedef) 


```python
# create_agent method usage example with argument unpacking

kwargs: CreateAgentRequestRequestTypeDef = {  # (1)
    "ActivationKey": ...,
}

parent.create_agent(**kwargs)
```

1. See [:material-code-braces: CreateAgentRequestRequestTypeDef](./type_defs.md#createagentrequestrequesttypedef) 

### create\_location\_azure\_blob

Creates a transfer <i>location</i> for a Microsoft Azure Blob Storage container.

Type annotations and code completion for `#!python session.create_client("datasync").create_location_azure_blob` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/create_location_azure_blob.html)

```python
# create_location_azure_blob method definition

await def create_location_azure_blob(
    self,
    *,
    ContainerUrl: str,
    AuthenticationType: AzureBlobAuthenticationTypeType,  # (1)
    AgentArns: Sequence[str],
    SasConfiguration: AzureBlobSasConfigurationTypeDef = ...,  # (2)
    BlobType: AzureBlobTypeType = ...,  # (3)
    AccessTier: AzureAccessTierType = ...,  # (4)
    Subdirectory: str = ...,
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (5)
) -> CreateLocationAzureBlobResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: AzureBlobAuthenticationTypeType](./literals.md#azureblobauthenticationtypetype) 
2. See [:material-code-braces: AzureBlobSasConfigurationTypeDef](./type_defs.md#azureblobsasconfigurationtypedef) 
3. See [:material-code-brackets: AzureBlobTypeType](./literals.md#azureblobtypetype) 
4. See [:material-code-brackets: AzureAccessTierType](./literals.md#azureaccesstiertype) 
5. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
6. See [:material-code-braces: CreateLocationAzureBlobResponseTypeDef](./type_defs.md#createlocationazureblobresponsetypedef) 


```python
# create_location_azure_blob method usage example with argument unpacking

kwargs: CreateLocationAzureBlobRequestRequestTypeDef = {  # (1)
    "ContainerUrl": ...,
    "AuthenticationType": ...,
    "AgentArns": ...,
}

parent.create_location_azure_blob(**kwargs)
```

1. See [:material-code-braces: CreateLocationAzureBlobRequestRequestTypeDef](./type_defs.md#createlocationazureblobrequestrequesttypedef) 

### create\_location\_efs

Creates a transfer <i>location</i> for an Amazon EFS file system.

Type annotations and code completion for `#!python session.create_client("datasync").create_location_efs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/create_location_efs.html)

```python
# create_location_efs method definition

await def create_location_efs(
    self,
    *,
    EfsFilesystemArn: str,
    Ec2Config: Ec2ConfigTypeDef,  # (1)
    Subdirectory: str = ...,
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (2)
    AccessPointArn: str = ...,
    FileSystemAccessRoleArn: str = ...,
    InTransitEncryption: EfsInTransitEncryptionType = ...,  # (3)
) -> CreateLocationEfsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: Ec2ConfigTypeDef](./type_defs.md#ec2configtypedef) 
2. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
3. See [:material-code-brackets: EfsInTransitEncryptionType](./literals.md#efsintransitencryptiontype) 
4. See [:material-code-braces: CreateLocationEfsResponseTypeDef](./type_defs.md#createlocationefsresponsetypedef) 


```python
# create_location_efs method usage example with argument unpacking

kwargs: CreateLocationEfsRequestRequestTypeDef = {  # (1)
    "EfsFilesystemArn": ...,
    "Ec2Config": ...,
}

parent.create_location_efs(**kwargs)
```

1. See [:material-code-braces: CreateLocationEfsRequestRequestTypeDef](./type_defs.md#createlocationefsrequestrequesttypedef) 

### create\_location\_fsx\_lustre

Creates a transfer <i>location</i> for an Amazon FSx for Lustre file system.

Type annotations and code completion for `#!python session.create_client("datasync").create_location_fsx_lustre` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/create_location_fsx_lustre.html)

```python
# create_location_fsx_lustre method definition

await def create_location_fsx_lustre(
    self,
    *,
    FsxFilesystemArn: str,
    SecurityGroupArns: Sequence[str],
    Subdirectory: str = ...,
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (1)
) -> CreateLocationFsxLustreResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
2. See [:material-code-braces: CreateLocationFsxLustreResponseTypeDef](./type_defs.md#createlocationfsxlustreresponsetypedef) 


```python
# create_location_fsx_lustre method usage example with argument unpacking

kwargs: CreateLocationFsxLustreRequestRequestTypeDef = {  # (1)
    "FsxFilesystemArn": ...,
    "SecurityGroupArns": ...,
}

parent.create_location_fsx_lustre(**kwargs)
```

1. See [:material-code-braces: CreateLocationFsxLustreRequestRequestTypeDef](./type_defs.md#createlocationfsxlustrerequestrequesttypedef) 

### create\_location\_fsx\_ontap

Creates a transfer <i>location</i> for an Amazon FSx for NetApp ONTAP file
system.

Type annotations and code completion for `#!python session.create_client("datasync").create_location_fsx_ontap` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/create_location_fsx_ontap.html)

```python
# create_location_fsx_ontap method definition

await def create_location_fsx_ontap(
    self,
    *,
    Protocol: FsxProtocolTypeDef,  # (1)
    SecurityGroupArns: Sequence[str],
    StorageVirtualMachineArn: str,
    Subdirectory: str = ...,
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (2)
) -> CreateLocationFsxOntapResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FsxProtocolTypeDef](./type_defs.md#fsxprotocoltypedef) 
2. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
3. See [:material-code-braces: CreateLocationFsxOntapResponseTypeDef](./type_defs.md#createlocationfsxontapresponsetypedef) 


```python
# create_location_fsx_ontap method usage example with argument unpacking

kwargs: CreateLocationFsxOntapRequestRequestTypeDef = {  # (1)
    "Protocol": ...,
    "SecurityGroupArns": ...,
    "StorageVirtualMachineArn": ...,
}

parent.create_location_fsx_ontap(**kwargs)
```

1. See [:material-code-braces: CreateLocationFsxOntapRequestRequestTypeDef](./type_defs.md#createlocationfsxontaprequestrequesttypedef) 

### create\_location\_fsx\_open\_zfs

Creates a transfer <i>location</i> for an Amazon FSx for OpenZFS file system.

Type annotations and code completion for `#!python session.create_client("datasync").create_location_fsx_open_zfs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/create_location_fsx_open_zfs.html)

```python
# create_location_fsx_open_zfs method definition

await def create_location_fsx_open_zfs(
    self,
    *,
    FsxFilesystemArn: str,
    Protocol: FsxProtocolTypeDef,  # (1)
    SecurityGroupArns: Sequence[str],
    Subdirectory: str = ...,
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (2)
) -> CreateLocationFsxOpenZfsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FsxProtocolTypeDef](./type_defs.md#fsxprotocoltypedef) 
2. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
3. See [:material-code-braces: CreateLocationFsxOpenZfsResponseTypeDef](./type_defs.md#createlocationfsxopenzfsresponsetypedef) 


```python
# create_location_fsx_open_zfs method usage example with argument unpacking

kwargs: CreateLocationFsxOpenZfsRequestRequestTypeDef = {  # (1)
    "FsxFilesystemArn": ...,
    "Protocol": ...,
    "SecurityGroupArns": ...,
}

parent.create_location_fsx_open_zfs(**kwargs)
```

1. See [:material-code-braces: CreateLocationFsxOpenZfsRequestRequestTypeDef](./type_defs.md#createlocationfsxopenzfsrequestrequesttypedef) 

### create\_location\_fsx\_windows

Creates a transfer <i>location</i> for an Amazon FSx for Windows File Server
file system.

Type annotations and code completion for `#!python session.create_client("datasync").create_location_fsx_windows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/create_location_fsx_windows.html)

```python
# create_location_fsx_windows method definition

await def create_location_fsx_windows(
    self,
    *,
    FsxFilesystemArn: str,
    SecurityGroupArns: Sequence[str],
    User: str,
    Password: str,
    Subdirectory: str = ...,
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (1)
    Domain: str = ...,
) -> CreateLocationFsxWindowsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
2. See [:material-code-braces: CreateLocationFsxWindowsResponseTypeDef](./type_defs.md#createlocationfsxwindowsresponsetypedef) 


```python
# create_location_fsx_windows method usage example with argument unpacking

kwargs: CreateLocationFsxWindowsRequestRequestTypeDef = {  # (1)
    "FsxFilesystemArn": ...,
    "SecurityGroupArns": ...,
    "User": ...,
    "Password": ...,
}

parent.create_location_fsx_windows(**kwargs)
```

1. See [:material-code-braces: CreateLocationFsxWindowsRequestRequestTypeDef](./type_defs.md#createlocationfsxwindowsrequestrequesttypedef) 

### create\_location\_hdfs

Creates a transfer <i>location</i> for a Hadoop Distributed File System (HDFS).

Type annotations and code completion for `#!python session.create_client("datasync").create_location_hdfs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/create_location_hdfs.html)

```python
# create_location_hdfs method definition

await def create_location_hdfs(
    self,
    *,
    NameNodes: Sequence[HdfsNameNodeTypeDef],  # (1)
    AuthenticationType: HdfsAuthenticationTypeType,  # (2)
    AgentArns: Sequence[str],
    Subdirectory: str = ...,
    BlockSize: int = ...,
    ReplicationFactor: int = ...,
    KmsKeyProviderUri: str = ...,
    QopConfiguration: QopConfigurationTypeDef = ...,  # (3)
    SimpleUser: str = ...,
    KerberosPrincipal: str = ...,
    KerberosKeytab: BlobTypeDef = ...,
    KerberosKrb5Conf: BlobTypeDef = ...,
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (4)
) -> CreateLocationHdfsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: HdfsNameNodeTypeDef](./type_defs.md#hdfsnamenodetypedef) 
2. See [:material-code-brackets: HdfsAuthenticationTypeType](./literals.md#hdfsauthenticationtypetype) 
3. See [:material-code-braces: QopConfigurationTypeDef](./type_defs.md#qopconfigurationtypedef) 
4. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
5. See [:material-code-braces: CreateLocationHdfsResponseTypeDef](./type_defs.md#createlocationhdfsresponsetypedef) 


```python
# create_location_hdfs method usage example with argument unpacking

kwargs: CreateLocationHdfsRequestRequestTypeDef = {  # (1)
    "NameNodes": ...,
    "AuthenticationType": ...,
    "AgentArns": ...,
}

parent.create_location_hdfs(**kwargs)
```

1. See [:material-code-braces: CreateLocationHdfsRequestRequestTypeDef](./type_defs.md#createlocationhdfsrequestrequesttypedef) 

### create\_location\_nfs

Creates a transfer <i>location</i> for a Network File System (NFS) file server.

Type annotations and code completion for `#!python session.create_client("datasync").create_location_nfs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/create_location_nfs.html)

```python
# create_location_nfs method definition

await def create_location_nfs(
    self,
    *,
    Subdirectory: str,
    ServerHostname: str,
    OnPremConfig: OnPremConfigTypeDef,  # (1)
    MountOptions: NfsMountOptionsTypeDef = ...,  # (2)
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (3)
) -> CreateLocationNfsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: OnPremConfigTypeDef](./type_defs.md#onpremconfigtypedef) 
2. See [:material-code-braces: NfsMountOptionsTypeDef](./type_defs.md#nfsmountoptionstypedef) 
3. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
4. See [:material-code-braces: CreateLocationNfsResponseTypeDef](./type_defs.md#createlocationnfsresponsetypedef) 


```python
# create_location_nfs method usage example with argument unpacking

kwargs: CreateLocationNfsRequestRequestTypeDef = {  # (1)
    "Subdirectory": ...,
    "ServerHostname": ...,
    "OnPremConfig": ...,
}

parent.create_location_nfs(**kwargs)
```

1. See [:material-code-braces: CreateLocationNfsRequestRequestTypeDef](./type_defs.md#createlocationnfsrequestrequesttypedef) 

### create\_location\_object\_storage

Creates a transfer <i>location</i> for an object storage system.

Type annotations and code completion for `#!python session.create_client("datasync").create_location_object_storage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/create_location_object_storage.html)

```python
# create_location_object_storage method definition

await def create_location_object_storage(
    self,
    *,
    ServerHostname: str,
    BucketName: str,
    AgentArns: Sequence[str],
    ServerPort: int = ...,
    ServerProtocol: ObjectStorageServerProtocolType = ...,  # (1)
    Subdirectory: str = ...,
    AccessKey: str = ...,
    SecretKey: str = ...,
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (2)
    ServerCertificate: BlobTypeDef = ...,
) -> CreateLocationObjectStorageResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ObjectStorageServerProtocolType](./literals.md#objectstorageserverprotocoltype) 
2. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
3. See [:material-code-braces: CreateLocationObjectStorageResponseTypeDef](./type_defs.md#createlocationobjectstorageresponsetypedef) 


```python
# create_location_object_storage method usage example with argument unpacking

kwargs: CreateLocationObjectStorageRequestRequestTypeDef = {  # (1)
    "ServerHostname": ...,
    "BucketName": ...,
    "AgentArns": ...,
}

parent.create_location_object_storage(**kwargs)
```

1. See [:material-code-braces: CreateLocationObjectStorageRequestRequestTypeDef](./type_defs.md#createlocationobjectstoragerequestrequesttypedef) 

### create\_location\_s3

Creates a transfer <i>location</i> for an Amazon S3 bucket.

Type annotations and code completion for `#!python session.create_client("datasync").create_location_s3` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/create_location_s3.html)

```python
# create_location_s3 method definition

await def create_location_s3(
    self,
    *,
    S3BucketArn: str,
    S3Config: S3ConfigTypeDef,  # (1)
    Subdirectory: str = ...,
    S3StorageClass: S3StorageClassType = ...,  # (2)
    AgentArns: Sequence[str] = ...,
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (3)
) -> CreateLocationS3ResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: S3ConfigTypeDef](./type_defs.md#s3configtypedef) 
2. See [:material-code-brackets: S3StorageClassType](./literals.md#s3storageclasstype) 
3. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
4. See [:material-code-braces: CreateLocationS3ResponseTypeDef](./type_defs.md#createlocations3responsetypedef) 


```python
# create_location_s3 method usage example with argument unpacking

kwargs: CreateLocationS3RequestRequestTypeDef = {  # (1)
    "S3BucketArn": ...,
    "S3Config": ...,
}

parent.create_location_s3(**kwargs)
```

1. See [:material-code-braces: CreateLocationS3RequestRequestTypeDef](./type_defs.md#createlocations3requestrequesttypedef) 

### create\_location\_smb

Creates a transfer <i>location</i> for a Server Message Block (SMB) file server.

Type annotations and code completion for `#!python session.create_client("datasync").create_location_smb` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/create_location_smb.html)

```python
# create_location_smb method definition

await def create_location_smb(
    self,
    *,
    Subdirectory: str,
    ServerHostname: str,
    User: str,
    Password: str,
    AgentArns: Sequence[str],
    Domain: str = ...,
    MountOptions: SmbMountOptionsTypeDef = ...,  # (1)
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (2)
) -> CreateLocationSmbResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SmbMountOptionsTypeDef](./type_defs.md#smbmountoptionstypedef) 
2. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
3. See [:material-code-braces: CreateLocationSmbResponseTypeDef](./type_defs.md#createlocationsmbresponsetypedef) 


```python
# create_location_smb method usage example with argument unpacking

kwargs: CreateLocationSmbRequestRequestTypeDef = {  # (1)
    "Subdirectory": ...,
    "ServerHostname": ...,
    "User": ...,
    "Password": ...,
    "AgentArns": ...,
}

parent.create_location_smb(**kwargs)
```

1. See [:material-code-braces: CreateLocationSmbRequestRequestTypeDef](./type_defs.md#createlocationsmbrequestrequesttypedef) 

### create\_task

Configures a <i>task</i>, which defines where and how DataSync transfers your
data.

Type annotations and code completion for `#!python session.create_client("datasync").create_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/create_task.html)

```python
# create_task method definition

await def create_task(
    self,
    *,
    SourceLocationArn: str,
    DestinationLocationArn: str,
    CloudWatchLogGroupArn: str = ...,
    Name: str = ...,
    Options: OptionsTypeDef = ...,  # (1)
    Excludes: Sequence[FilterRuleTypeDef] = ...,  # (2)
    Schedule: TaskScheduleTypeDef = ...,  # (3)
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (4)
    Includes: Sequence[FilterRuleTypeDef] = ...,  # (2)
    ManifestConfig: ManifestConfigTypeDef = ...,  # (6)
    TaskReportConfig: TaskReportConfigTypeDef = ...,  # (7)
    TaskMode: TaskModeType = ...,  # (8)
) -> CreateTaskResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: OptionsTypeDef](./type_defs.md#optionstypedef) 
2. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
3. See [:material-code-braces: TaskScheduleTypeDef](./type_defs.md#taskscheduletypedef) 
4. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
5. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
6. See [:material-code-braces: ManifestConfigTypeDef](./type_defs.md#manifestconfigtypedef) 
7. See [:material-code-braces: TaskReportConfigTypeDef](./type_defs.md#taskreportconfigtypedef) 
8. See [:material-code-brackets: TaskModeType](./literals.md#taskmodetype) 
9. See [:material-code-braces: CreateTaskResponseTypeDef](./type_defs.md#createtaskresponsetypedef) 


```python
# create_task method usage example with argument unpacking

kwargs: CreateTaskRequestRequestTypeDef = {  # (1)
    "SourceLocationArn": ...,
    "DestinationLocationArn": ...,
}

parent.create_task(**kwargs)
```

1. See [:material-code-braces: CreateTaskRequestRequestTypeDef](./type_defs.md#createtaskrequestrequesttypedef) 

### delete\_agent

Removes an DataSync agent resource from your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("datasync").delete_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/delete_agent.html)

```python
# delete_agent method definition

await def delete_agent(
    self,
    *,
    AgentArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_agent method usage example with argument unpacking

kwargs: DeleteAgentRequestRequestTypeDef = {  # (1)
    "AgentArn": ...,
}

parent.delete_agent(**kwargs)
```

1. See [:material-code-braces: DeleteAgentRequestRequestTypeDef](./type_defs.md#deleteagentrequestrequesttypedef) 

### delete\_location

Deletes a transfer location resource from DataSync.

Type annotations and code completion for `#!python session.create_client("datasync").delete_location` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/delete_location.html)

```python
# delete_location method definition

await def delete_location(
    self,
    *,
    LocationArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_location method usage example with argument unpacking

kwargs: DeleteLocationRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.delete_location(**kwargs)
```

1. See [:material-code-braces: DeleteLocationRequestRequestTypeDef](./type_defs.md#deletelocationrequestrequesttypedef) 

### delete\_task

Deletes a transfer task resource from DataSync.

Type annotations and code completion for `#!python session.create_client("datasync").delete_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/delete_task.html)

```python
# delete_task method definition

await def delete_task(
    self,
    *,
    TaskArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_task method usage example with argument unpacking

kwargs: DeleteTaskRequestRequestTypeDef = {  # (1)
    "TaskArn": ...,
}

parent.delete_task(**kwargs)
```

1. See [:material-code-braces: DeleteTaskRequestRequestTypeDef](./type_defs.md#deletetaskrequestrequesttypedef) 

### describe\_agent

Returns information about an DataSync agent, such as its name, service endpoint
type, and status.

Type annotations and code completion for `#!python session.create_client("datasync").describe_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_agent.html)

```python
# describe_agent method definition

await def describe_agent(
    self,
    *,
    AgentArn: str,
) -> DescribeAgentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAgentResponseTypeDef](./type_defs.md#describeagentresponsetypedef) 


```python
# describe_agent method usage example with argument unpacking

kwargs: DescribeAgentRequestRequestTypeDef = {  # (1)
    "AgentArn": ...,
}

parent.describe_agent(**kwargs)
```

1. See [:material-code-braces: DescribeAgentRequestRequestTypeDef](./type_defs.md#describeagentrequestrequesttypedef) 

### describe\_discovery\_job

Returns information about a DataSync discovery job.

Type annotations and code completion for `#!python session.create_client("datasync").describe_discovery_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_discovery_job.html)

```python
# describe_discovery_job method definition

await def describe_discovery_job(
    self,
    *,
    DiscoveryJobArn: str,
) -> DescribeDiscoveryJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDiscoveryJobResponseTypeDef](./type_defs.md#describediscoveryjobresponsetypedef) 


```python
# describe_discovery_job method usage example with argument unpacking

kwargs: DescribeDiscoveryJobRequestRequestTypeDef = {  # (1)
    "DiscoveryJobArn": ...,
}

parent.describe_discovery_job(**kwargs)
```

1. See [:material-code-braces: DescribeDiscoveryJobRequestRequestTypeDef](./type_defs.md#describediscoveryjobrequestrequesttypedef) 

### describe\_location\_azure\_blob

Provides details about how an DataSync transfer location for Microsoft Azure
Blob Storage is configured.

Type annotations and code completion for `#!python session.create_client("datasync").describe_location_azure_blob` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_location_azure_blob.html)

```python
# describe_location_azure_blob method definition

await def describe_location_azure_blob(
    self,
    *,
    LocationArn: str,
) -> DescribeLocationAzureBlobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLocationAzureBlobResponseTypeDef](./type_defs.md#describelocationazureblobresponsetypedef) 


```python
# describe_location_azure_blob method usage example with argument unpacking

kwargs: DescribeLocationAzureBlobRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_azure_blob(**kwargs)
```

1. See [:material-code-braces: DescribeLocationAzureBlobRequestRequestTypeDef](./type_defs.md#describelocationazureblobrequestrequesttypedef) 

### describe\_location\_efs

Provides details about how an DataSync transfer location for an Amazon EFS file
system is configured.

Type annotations and code completion for `#!python session.create_client("datasync").describe_location_efs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_location_efs.html)

```python
# describe_location_efs method definition

await def describe_location_efs(
    self,
    *,
    LocationArn: str,
) -> DescribeLocationEfsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLocationEfsResponseTypeDef](./type_defs.md#describelocationefsresponsetypedef) 


```python
# describe_location_efs method usage example with argument unpacking

kwargs: DescribeLocationEfsRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_efs(**kwargs)
```

1. See [:material-code-braces: DescribeLocationEfsRequestRequestTypeDef](./type_defs.md#describelocationefsrequestrequesttypedef) 

### describe\_location\_fsx\_lustre

Provides details about how an DataSync transfer location for an Amazon FSx for
Lustre file system is configured.

Type annotations and code completion for `#!python session.create_client("datasync").describe_location_fsx_lustre` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_location_fsx_lustre.html)

```python
# describe_location_fsx_lustre method definition

await def describe_location_fsx_lustre(
    self,
    *,
    LocationArn: str,
) -> DescribeLocationFsxLustreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLocationFsxLustreResponseTypeDef](./type_defs.md#describelocationfsxlustreresponsetypedef) 


```python
# describe_location_fsx_lustre method usage example with argument unpacking

kwargs: DescribeLocationFsxLustreRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_fsx_lustre(**kwargs)
```

1. See [:material-code-braces: DescribeLocationFsxLustreRequestRequestTypeDef](./type_defs.md#describelocationfsxlustrerequestrequesttypedef) 

### describe\_location\_fsx\_ontap

Provides details about how an DataSync transfer location for an Amazon FSx for
NetApp ONTAP file system is configured.

Type annotations and code completion for `#!python session.create_client("datasync").describe_location_fsx_ontap` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_location_fsx_ontap.html)

```python
# describe_location_fsx_ontap method definition

await def describe_location_fsx_ontap(
    self,
    *,
    LocationArn: str,
) -> DescribeLocationFsxOntapResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLocationFsxOntapResponseTypeDef](./type_defs.md#describelocationfsxontapresponsetypedef) 


```python
# describe_location_fsx_ontap method usage example with argument unpacking

kwargs: DescribeLocationFsxOntapRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_fsx_ontap(**kwargs)
```

1. See [:material-code-braces: DescribeLocationFsxOntapRequestRequestTypeDef](./type_defs.md#describelocationfsxontaprequestrequesttypedef) 

### describe\_location\_fsx\_open\_zfs

Provides details about how an DataSync transfer location for an Amazon FSx for
OpenZFS file system is configured.

Type annotations and code completion for `#!python session.create_client("datasync").describe_location_fsx_open_zfs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_location_fsx_open_zfs.html)

```python
# describe_location_fsx_open_zfs method definition

await def describe_location_fsx_open_zfs(
    self,
    *,
    LocationArn: str,
) -> DescribeLocationFsxOpenZfsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLocationFsxOpenZfsResponseTypeDef](./type_defs.md#describelocationfsxopenzfsresponsetypedef) 


```python
# describe_location_fsx_open_zfs method usage example with argument unpacking

kwargs: DescribeLocationFsxOpenZfsRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_fsx_open_zfs(**kwargs)
```

1. See [:material-code-braces: DescribeLocationFsxOpenZfsRequestRequestTypeDef](./type_defs.md#describelocationfsxopenzfsrequestrequesttypedef) 

### describe\_location\_fsx\_windows

Provides details about how an DataSync transfer location for an Amazon FSx for
Windows File Server file system is configured.

Type annotations and code completion for `#!python session.create_client("datasync").describe_location_fsx_windows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_location_fsx_windows.html)

```python
# describe_location_fsx_windows method definition

await def describe_location_fsx_windows(
    self,
    *,
    LocationArn: str,
) -> DescribeLocationFsxWindowsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLocationFsxWindowsResponseTypeDef](./type_defs.md#describelocationfsxwindowsresponsetypedef) 


```python
# describe_location_fsx_windows method usage example with argument unpacking

kwargs: DescribeLocationFsxWindowsRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_fsx_windows(**kwargs)
```

1. See [:material-code-braces: DescribeLocationFsxWindowsRequestRequestTypeDef](./type_defs.md#describelocationfsxwindowsrequestrequesttypedef) 

### describe\_location\_hdfs

Provides details about how an DataSync transfer location for a Hadoop
Distributed File System (HDFS) is configured.

Type annotations and code completion for `#!python session.create_client("datasync").describe_location_hdfs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_location_hdfs.html)

```python
# describe_location_hdfs method definition

await def describe_location_hdfs(
    self,
    *,
    LocationArn: str,
) -> DescribeLocationHdfsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLocationHdfsResponseTypeDef](./type_defs.md#describelocationhdfsresponsetypedef) 


```python
# describe_location_hdfs method usage example with argument unpacking

kwargs: DescribeLocationHdfsRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_hdfs(**kwargs)
```

1. See [:material-code-braces: DescribeLocationHdfsRequestRequestTypeDef](./type_defs.md#describelocationhdfsrequestrequesttypedef) 

### describe\_location\_nfs

Provides details about how an DataSync transfer location for a Network File
System (NFS) file server is configured.

Type annotations and code completion for `#!python session.create_client("datasync").describe_location_nfs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_location_nfs.html)

```python
# describe_location_nfs method definition

await def describe_location_nfs(
    self,
    *,
    LocationArn: str,
) -> DescribeLocationNfsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLocationNfsResponseTypeDef](./type_defs.md#describelocationnfsresponsetypedef) 


```python
# describe_location_nfs method usage example with argument unpacking

kwargs: DescribeLocationNfsRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_nfs(**kwargs)
```

1. See [:material-code-braces: DescribeLocationNfsRequestRequestTypeDef](./type_defs.md#describelocationnfsrequestrequesttypedef) 

### describe\_location\_object\_storage

Provides details about how an DataSync transfer location for an object storage
system is configured.

Type annotations and code completion for `#!python session.create_client("datasync").describe_location_object_storage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_location_object_storage.html)

```python
# describe_location_object_storage method definition

await def describe_location_object_storage(
    self,
    *,
    LocationArn: str,
) -> DescribeLocationObjectStorageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLocationObjectStorageResponseTypeDef](./type_defs.md#describelocationobjectstorageresponsetypedef) 


```python
# describe_location_object_storage method usage example with argument unpacking

kwargs: DescribeLocationObjectStorageRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_object_storage(**kwargs)
```

1. See [:material-code-braces: DescribeLocationObjectStorageRequestRequestTypeDef](./type_defs.md#describelocationobjectstoragerequestrequesttypedef) 

### describe\_location\_s3

Provides details about how an DataSync transfer location for an S3 bucket is
configured.

Type annotations and code completion for `#!python session.create_client("datasync").describe_location_s3` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_location_s3.html)

```python
# describe_location_s3 method definition

await def describe_location_s3(
    self,
    *,
    LocationArn: str,
) -> DescribeLocationS3ResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLocationS3ResponseTypeDef](./type_defs.md#describelocations3responsetypedef) 


```python
# describe_location_s3 method usage example with argument unpacking

kwargs: DescribeLocationS3RequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_s3(**kwargs)
```

1. See [:material-code-braces: DescribeLocationS3RequestRequestTypeDef](./type_defs.md#describelocations3requestrequesttypedef) 

### describe\_location\_smb

Provides details about how an DataSync transfer location for a Server Message
Block (SMB) file server is configured.

Type annotations and code completion for `#!python session.create_client("datasync").describe_location_smb` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_location_smb.html)

```python
# describe_location_smb method definition

await def describe_location_smb(
    self,
    *,
    LocationArn: str,
) -> DescribeLocationSmbResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLocationSmbResponseTypeDef](./type_defs.md#describelocationsmbresponsetypedef) 


```python
# describe_location_smb method usage example with argument unpacking

kwargs: DescribeLocationSmbRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_smb(**kwargs)
```

1. See [:material-code-braces: DescribeLocationSmbRequestRequestTypeDef](./type_defs.md#describelocationsmbrequestrequesttypedef) 

### describe\_storage\_system

Returns information about an on-premises storage system that you're using with
DataSync Discovery.

Type annotations and code completion for `#!python session.create_client("datasync").describe_storage_system` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_storage_system.html)

```python
# describe_storage_system method definition

await def describe_storage_system(
    self,
    *,
    StorageSystemArn: str,
) -> DescribeStorageSystemResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStorageSystemResponseTypeDef](./type_defs.md#describestoragesystemresponsetypedef) 


```python
# describe_storage_system method usage example with argument unpacking

kwargs: DescribeStorageSystemRequestRequestTypeDef = {  # (1)
    "StorageSystemArn": ...,
}

parent.describe_storage_system(**kwargs)
```

1. See [:material-code-braces: DescribeStorageSystemRequestRequestTypeDef](./type_defs.md#describestoragesystemrequestrequesttypedef) 

### describe\_storage\_system\_resource\_metrics

Returns information, including performance data and capacity usage, which
DataSync Discovery collects about a specific resource in your-premises storage
system.

Type annotations and code completion for `#!python session.create_client("datasync").describe_storage_system_resource_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_storage_system_resource_metrics.html)

```python
# describe_storage_system_resource_metrics method definition

await def describe_storage_system_resource_metrics(
    self,
    *,
    DiscoveryJobArn: str,
    ResourceType: DiscoveryResourceTypeType,  # (1)
    ResourceId: str,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeStorageSystemResourceMetricsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DiscoveryResourceTypeType](./literals.md#discoveryresourcetypetype) 
2. See [:material-code-braces: DescribeStorageSystemResourceMetricsResponseTypeDef](./type_defs.md#describestoragesystemresourcemetricsresponsetypedef) 


```python
# describe_storage_system_resource_metrics method usage example with argument unpacking

kwargs: DescribeStorageSystemResourceMetricsRequestRequestTypeDef = {  # (1)
    "DiscoveryJobArn": ...,
    "ResourceType": ...,
    "ResourceId": ...,
}

parent.describe_storage_system_resource_metrics(**kwargs)
```

1. See [:material-code-braces: DescribeStorageSystemResourceMetricsRequestRequestTypeDef](./type_defs.md#describestoragesystemresourcemetricsrequestrequesttypedef) 

### describe\_storage\_system\_resources

Returns information that DataSync Discovery collects about resources in your
on-premises storage system.

Type annotations and code completion for `#!python session.create_client("datasync").describe_storage_system_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_storage_system_resources.html)

```python
# describe_storage_system_resources method definition

await def describe_storage_system_resources(
    self,
    *,
    DiscoveryJobArn: str,
    ResourceType: DiscoveryResourceTypeType,  # (1)
    ResourceIds: Sequence[str] = ...,
    Filter: Mapping[DiscoveryResourceFilterType, Sequence[str]] = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeStorageSystemResourcesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: DiscoveryResourceTypeType](./literals.md#discoveryresourcetypetype) 
2. See [:material-code-brackets: DiscoveryResourceFilterType](./literals.md#discoveryresourcefiltertype) 
3. See [:material-code-braces: DescribeStorageSystemResourcesResponseTypeDef](./type_defs.md#describestoragesystemresourcesresponsetypedef) 


```python
# describe_storage_system_resources method usage example with argument unpacking

kwargs: DescribeStorageSystemResourcesRequestRequestTypeDef = {  # (1)
    "DiscoveryJobArn": ...,
    "ResourceType": ...,
}

parent.describe_storage_system_resources(**kwargs)
```

1. See [:material-code-braces: DescribeStorageSystemResourcesRequestRequestTypeDef](./type_defs.md#describestoragesystemresourcesrequestrequesttypedef) 

### describe\_task

Provides information about a <i>task</i>, which defines where and how DataSync
transfers your data.

Type annotations and code completion for `#!python session.create_client("datasync").describe_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_task.html)

```python
# describe_task method definition

await def describe_task(
    self,
    *,
    TaskArn: str,
) -> DescribeTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTaskResponseTypeDef](./type_defs.md#describetaskresponsetypedef) 


```python
# describe_task method usage example with argument unpacking

kwargs: DescribeTaskRequestRequestTypeDef = {  # (1)
    "TaskArn": ...,
}

parent.describe_task(**kwargs)
```

1. See [:material-code-braces: DescribeTaskRequestRequestTypeDef](./type_defs.md#describetaskrequestrequesttypedef) 

### describe\_task\_execution

Provides information about an execution of your DataSync task.

Type annotations and code completion for `#!python session.create_client("datasync").describe_task_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/describe_task_execution.html)

```python
# describe_task_execution method definition

await def describe_task_execution(
    self,
    *,
    TaskExecutionArn: str,
) -> DescribeTaskExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTaskExecutionResponseTypeDef](./type_defs.md#describetaskexecutionresponsetypedef) 


```python
# describe_task_execution method usage example with argument unpacking

kwargs: DescribeTaskExecutionRequestRequestTypeDef = {  # (1)
    "TaskExecutionArn": ...,
}

parent.describe_task_execution(**kwargs)
```

1. See [:material-code-braces: DescribeTaskExecutionRequestRequestTypeDef](./type_defs.md#describetaskexecutionrequestrequesttypedef) 

### generate\_recommendations

Creates recommendations about where to migrate your data to in Amazon Web
Services.

Type annotations and code completion for `#!python session.create_client("datasync").generate_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/generate_recommendations.html)

```python
# generate_recommendations method definition

await def generate_recommendations(
    self,
    *,
    DiscoveryJobArn: str,
    ResourceIds: Sequence[str],
    ResourceType: DiscoveryResourceTypeType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: DiscoveryResourceTypeType](./literals.md#discoveryresourcetypetype) 


```python
# generate_recommendations method usage example with argument unpacking

kwargs: GenerateRecommendationsRequestRequestTypeDef = {  # (1)
    "DiscoveryJobArn": ...,
    "ResourceIds": ...,
    "ResourceType": ...,
}

parent.generate_recommendations(**kwargs)
```

1. See [:material-code-braces: GenerateRecommendationsRequestRequestTypeDef](./type_defs.md#generaterecommendationsrequestrequesttypedef) 

### list\_agents

Returns a list of DataSync agents that belong to an Amazon Web Services account
in the Amazon Web Services Region specified in the request.

Type annotations and code completion for `#!python session.create_client("datasync").list_agents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/list_agents.html)

```python
# list_agents method definition

await def list_agents(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAgentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentsResponseTypeDef](./type_defs.md#listagentsresponsetypedef) 


```python
# list_agents method usage example with argument unpacking

kwargs: ListAgentsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_agents(**kwargs)
```

1. See [:material-code-braces: ListAgentsRequestRequestTypeDef](./type_defs.md#listagentsrequestrequesttypedef) 

### list\_discovery\_jobs

Provides a list of the existing discovery jobs in the Amazon Web Services
Region and Amazon Web Services account where you're using DataSync Discovery.

Type annotations and code completion for `#!python session.create_client("datasync").list_discovery_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/list_discovery_jobs.html)

```python
# list_discovery_jobs method definition

await def list_discovery_jobs(
    self,
    *,
    StorageSystemArn: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDiscoveryJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDiscoveryJobsResponseTypeDef](./type_defs.md#listdiscoveryjobsresponsetypedef) 


```python
# list_discovery_jobs method usage example with argument unpacking

kwargs: ListDiscoveryJobsRequestRequestTypeDef = {  # (1)
    "StorageSystemArn": ...,
}

parent.list_discovery_jobs(**kwargs)
```

1. See [:material-code-braces: ListDiscoveryJobsRequestRequestTypeDef](./type_defs.md#listdiscoveryjobsrequestrequesttypedef) 

### list\_locations

Returns a list of source and destination locations.

Type annotations and code completion for `#!python session.create_client("datasync").list_locations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/list_locations.html)

```python
# list_locations method definition

await def list_locations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[LocationFilterTypeDef] = ...,  # (1)
) -> ListLocationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LocationFilterTypeDef](./type_defs.md#locationfiltertypedef) 
2. See [:material-code-braces: ListLocationsResponseTypeDef](./type_defs.md#listlocationsresponsetypedef) 


```python
# list_locations method usage example with argument unpacking

kwargs: ListLocationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_locations(**kwargs)
```

1. See [:material-code-braces: ListLocationsRequestRequestTypeDef](./type_defs.md#listlocationsrequestrequesttypedef) 

### list\_storage\_systems

Lists the on-premises storage systems that you're using with DataSync Discovery.

Type annotations and code completion for `#!python session.create_client("datasync").list_storage_systems` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/list_storage_systems.html)

```python
# list_storage_systems method definition

await def list_storage_systems(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListStorageSystemsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStorageSystemsResponseTypeDef](./type_defs.md#liststoragesystemsresponsetypedef) 


```python
# list_storage_systems method usage example with argument unpacking

kwargs: ListStorageSystemsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_storage_systems(**kwargs)
```

1. See [:material-code-braces: ListStorageSystemsRequestRequestTypeDef](./type_defs.md#liststoragesystemsrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns all the tags associated with an Amazon Web Services resource.

Type annotations and code completion for `#!python session.create_client("datasync").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_task\_executions

Returns a list of executions for an DataSync transfer task.

Type annotations and code completion for `#!python session.create_client("datasync").list_task_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/list_task_executions.html)

```python
# list_task_executions method definition

await def list_task_executions(
    self,
    *,
    TaskArn: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTaskExecutionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTaskExecutionsResponseTypeDef](./type_defs.md#listtaskexecutionsresponsetypedef) 


```python
# list_task_executions method usage example with argument unpacking

kwargs: ListTaskExecutionsRequestRequestTypeDef = {  # (1)
    "TaskArn": ...,
}

parent.list_task_executions(**kwargs)
```

1. See [:material-code-braces: ListTaskExecutionsRequestRequestTypeDef](./type_defs.md#listtaskexecutionsrequestrequesttypedef) 

### list\_tasks

Returns a list of the DataSync tasks you created.

Type annotations and code completion for `#!python session.create_client("datasync").list_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/list_tasks.html)

```python
# list_tasks method definition

await def list_tasks(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[TaskFilterTypeDef] = ...,  # (1)
) -> ListTasksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TaskFilterTypeDef](./type_defs.md#taskfiltertypedef) 
2. See [:material-code-braces: ListTasksResponseTypeDef](./type_defs.md#listtasksresponsetypedef) 


```python
# list_tasks method usage example with argument unpacking

kwargs: ListTasksRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_tasks(**kwargs)
```

1. See [:material-code-braces: ListTasksRequestRequestTypeDef](./type_defs.md#listtasksrequestrequesttypedef) 

### remove\_storage\_system

Permanently removes a storage system resource from DataSync Discovery,
including the associated discovery jobs, collected data, and recommendations.

Type annotations and code completion for `#!python session.create_client("datasync").remove_storage_system` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/remove_storage_system.html)

```python
# remove_storage_system method definition

await def remove_storage_system(
    self,
    *,
    StorageSystemArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# remove_storage_system method usage example with argument unpacking

kwargs: RemoveStorageSystemRequestRequestTypeDef = {  # (1)
    "StorageSystemArn": ...,
}

parent.remove_storage_system(**kwargs)
```

1. See [:material-code-braces: RemoveStorageSystemRequestRequestTypeDef](./type_defs.md#removestoragesystemrequestrequesttypedef) 

### start\_discovery\_job

Runs a DataSync discovery job on your on-premises storage system.

Type annotations and code completion for `#!python session.create_client("datasync").start_discovery_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/start_discovery_job.html)

```python
# start_discovery_job method definition

await def start_discovery_job(
    self,
    *,
    StorageSystemArn: str,
    CollectionDurationMinutes: int,
    ClientToken: str,
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (1)
) -> StartDiscoveryJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
2. See [:material-code-braces: StartDiscoveryJobResponseTypeDef](./type_defs.md#startdiscoveryjobresponsetypedef) 


```python
# start_discovery_job method usage example with argument unpacking

kwargs: StartDiscoveryJobRequestRequestTypeDef = {  # (1)
    "StorageSystemArn": ...,
    "CollectionDurationMinutes": ...,
    "ClientToken": ...,
}

parent.start_discovery_job(**kwargs)
```

1. See [:material-code-braces: StartDiscoveryJobRequestRequestTypeDef](./type_defs.md#startdiscoveryjobrequestrequesttypedef) 

### start\_task\_execution

Starts an DataSync transfer task.

Type annotations and code completion for `#!python session.create_client("datasync").start_task_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/start_task_execution.html)

```python
# start_task_execution method definition

await def start_task_execution(
    self,
    *,
    TaskArn: str,
    OverrideOptions: OptionsTypeDef = ...,  # (1)
    Includes: Sequence[FilterRuleTypeDef] = ...,  # (2)
    Excludes: Sequence[FilterRuleTypeDef] = ...,  # (2)
    ManifestConfig: ManifestConfigTypeDef = ...,  # (4)
    TaskReportConfig: TaskReportConfigTypeDef = ...,  # (5)
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (6)
) -> StartTaskExecutionResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: OptionsTypeDef](./type_defs.md#optionstypedef) 
2. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
3. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
4. See [:material-code-braces: ManifestConfigTypeDef](./type_defs.md#manifestconfigtypedef) 
5. See [:material-code-braces: TaskReportConfigTypeDef](./type_defs.md#taskreportconfigtypedef) 
6. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
7. See [:material-code-braces: StartTaskExecutionResponseTypeDef](./type_defs.md#starttaskexecutionresponsetypedef) 


```python
# start_task_execution method usage example with argument unpacking

kwargs: StartTaskExecutionRequestRequestTypeDef = {  # (1)
    "TaskArn": ...,
}

parent.start_task_execution(**kwargs)
```

1. See [:material-code-braces: StartTaskExecutionRequestRequestTypeDef](./type_defs.md#starttaskexecutionrequestrequesttypedef) 

### stop\_discovery\_job

Stops a running DataSync discovery job.

Type annotations and code completion for `#!python session.create_client("datasync").stop_discovery_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/stop_discovery_job.html)

```python
# stop_discovery_job method definition

await def stop_discovery_job(
    self,
    *,
    DiscoveryJobArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_discovery_job method usage example with argument unpacking

kwargs: StopDiscoveryJobRequestRequestTypeDef = {  # (1)
    "DiscoveryJobArn": ...,
}

parent.stop_discovery_job(**kwargs)
```

1. See [:material-code-braces: StopDiscoveryJobRequestRequestTypeDef](./type_defs.md#stopdiscoveryjobrequestrequesttypedef) 

### tag\_resource

Applies a <i>tag</i> to an Amazon Web Services resource.

Type annotations and code completion for `#!python session.create_client("datasync").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagListEntryTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from an Amazon Web Services resource.

Type annotations and code completion for `#!python session.create_client("datasync").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    Keys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Keys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_agent

Updates the name of an DataSync agent.

Type annotations and code completion for `#!python session.create_client("datasync").update_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_agent.html)

```python
# update_agent method definition

await def update_agent(
    self,
    *,
    AgentArn: str,
    Name: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_agent method usage example with argument unpacking

kwargs: UpdateAgentRequestRequestTypeDef = {  # (1)
    "AgentArn": ...,
}

parent.update_agent(**kwargs)
```

1. See [:material-code-braces: UpdateAgentRequestRequestTypeDef](./type_defs.md#updateagentrequestrequesttypedef) 

### update\_discovery\_job

Edits a DataSync discovery job configuration.

Type annotations and code completion for `#!python session.create_client("datasync").update_discovery_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_discovery_job.html)

```python
# update_discovery_job method definition

await def update_discovery_job(
    self,
    *,
    DiscoveryJobArn: str,
    CollectionDurationMinutes: int,
) -> Dict[str, Any]:
    ...
```



```python
# update_discovery_job method usage example with argument unpacking

kwargs: UpdateDiscoveryJobRequestRequestTypeDef = {  # (1)
    "DiscoveryJobArn": ...,
    "CollectionDurationMinutes": ...,
}

parent.update_discovery_job(**kwargs)
```

1. See [:material-code-braces: UpdateDiscoveryJobRequestRequestTypeDef](./type_defs.md#updatediscoveryjobrequestrequesttypedef) 

### update\_location\_azure\_blob

Modifies some configurations of the Microsoft Azure Blob Storage transfer
location that you're using with DataSync.

Type annotations and code completion for `#!python session.create_client("datasync").update_location_azure_blob` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_location_azure_blob.html)

```python
# update_location_azure_blob method definition

await def update_location_azure_blob(
    self,
    *,
    LocationArn: str,
    Subdirectory: str = ...,
    AuthenticationType: AzureBlobAuthenticationTypeType = ...,  # (1)
    SasConfiguration: AzureBlobSasConfigurationTypeDef = ...,  # (2)
    BlobType: AzureBlobTypeType = ...,  # (3)
    AccessTier: AzureAccessTierType = ...,  # (4)
    AgentArns: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: AzureBlobAuthenticationTypeType](./literals.md#azureblobauthenticationtypetype) 
2. See [:material-code-braces: AzureBlobSasConfigurationTypeDef](./type_defs.md#azureblobsasconfigurationtypedef) 
3. See [:material-code-brackets: AzureBlobTypeType](./literals.md#azureblobtypetype) 
4. See [:material-code-brackets: AzureAccessTierType](./literals.md#azureaccesstiertype) 


```python
# update_location_azure_blob method usage example with argument unpacking

kwargs: UpdateLocationAzureBlobRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_azure_blob(**kwargs)
```

1. See [:material-code-braces: UpdateLocationAzureBlobRequestRequestTypeDef](./type_defs.md#updatelocationazureblobrequestrequesttypedef) 

### update\_location\_hdfs

Updates some parameters of a previously created location for a Hadoop
Distributed File System cluster.

Type annotations and code completion for `#!python session.create_client("datasync").update_location_hdfs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_location_hdfs.html)

```python
# update_location_hdfs method definition

await def update_location_hdfs(
    self,
    *,
    LocationArn: str,
    Subdirectory: str = ...,
    NameNodes: Sequence[HdfsNameNodeTypeDef] = ...,  # (1)
    BlockSize: int = ...,
    ReplicationFactor: int = ...,
    KmsKeyProviderUri: str = ...,
    QopConfiguration: QopConfigurationTypeDef = ...,  # (2)
    AuthenticationType: HdfsAuthenticationTypeType = ...,  # (3)
    SimpleUser: str = ...,
    KerberosPrincipal: str = ...,
    KerberosKeytab: BlobTypeDef = ...,
    KerberosKrb5Conf: BlobTypeDef = ...,
    AgentArns: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: HdfsNameNodeTypeDef](./type_defs.md#hdfsnamenodetypedef) 
2. See [:material-code-braces: QopConfigurationTypeDef](./type_defs.md#qopconfigurationtypedef) 
3. See [:material-code-brackets: HdfsAuthenticationTypeType](./literals.md#hdfsauthenticationtypetype) 


```python
# update_location_hdfs method usage example with argument unpacking

kwargs: UpdateLocationHdfsRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_hdfs(**kwargs)
```

1. See [:material-code-braces: UpdateLocationHdfsRequestRequestTypeDef](./type_defs.md#updatelocationhdfsrequestrequesttypedef) 

### update\_location\_nfs

Modifies some configurations of the Network File System (NFS) transfer location
that you're using with DataSync.

Type annotations and code completion for `#!python session.create_client("datasync").update_location_nfs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_location_nfs.html)

```python
# update_location_nfs method definition

await def update_location_nfs(
    self,
    *,
    LocationArn: str,
    Subdirectory: str = ...,
    OnPremConfig: OnPremConfigTypeDef = ...,  # (1)
    MountOptions: NfsMountOptionsTypeDef = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: OnPremConfigTypeDef](./type_defs.md#onpremconfigtypedef) 
2. See [:material-code-braces: NfsMountOptionsTypeDef](./type_defs.md#nfsmountoptionstypedef) 


```python
# update_location_nfs method usage example with argument unpacking

kwargs: UpdateLocationNfsRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_nfs(**kwargs)
```

1. See [:material-code-braces: UpdateLocationNfsRequestRequestTypeDef](./type_defs.md#updatelocationnfsrequestrequesttypedef) 

### update\_location\_object\_storage

Updates some parameters of an existing DataSync location for an object storage
system.

Type annotations and code completion for `#!python session.create_client("datasync").update_location_object_storage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_location_object_storage.html)

```python
# update_location_object_storage method definition

await def update_location_object_storage(
    self,
    *,
    LocationArn: str,
    ServerPort: int = ...,
    ServerProtocol: ObjectStorageServerProtocolType = ...,  # (1)
    Subdirectory: str = ...,
    AccessKey: str = ...,
    SecretKey: str = ...,
    AgentArns: Sequence[str] = ...,
    ServerCertificate: BlobTypeDef = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ObjectStorageServerProtocolType](./literals.md#objectstorageserverprotocoltype) 


```python
# update_location_object_storage method usage example with argument unpacking

kwargs: UpdateLocationObjectStorageRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_object_storage(**kwargs)
```

1. See [:material-code-braces: UpdateLocationObjectStorageRequestRequestTypeDef](./type_defs.md#updatelocationobjectstoragerequestrequesttypedef) 

### update\_location\_smb

Updates some of the parameters of a Server Message Block (SMB) file server
location that you can use for DataSync transfers.

Type annotations and code completion for `#!python session.create_client("datasync").update_location_smb` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_location_smb.html)

```python
# update_location_smb method definition

await def update_location_smb(
    self,
    *,
    LocationArn: str,
    Subdirectory: str = ...,
    User: str = ...,
    Domain: str = ...,
    Password: str = ...,
    AgentArns: Sequence[str] = ...,
    MountOptions: SmbMountOptionsTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: SmbMountOptionsTypeDef](./type_defs.md#smbmountoptionstypedef) 


```python
# update_location_smb method usage example with argument unpacking

kwargs: UpdateLocationSmbRequestRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_smb(**kwargs)
```

1. See [:material-code-braces: UpdateLocationSmbRequestRequestTypeDef](./type_defs.md#updatelocationsmbrequestrequesttypedef) 

### update\_storage\_system

Modifies some configurations of an on-premises storage system resource that
you're using with DataSync Discovery.

Type annotations and code completion for `#!python session.create_client("datasync").update_storage_system` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_storage_system.html)

```python
# update_storage_system method definition

await def update_storage_system(
    self,
    *,
    StorageSystemArn: str,
    ServerConfiguration: DiscoveryServerConfigurationTypeDef = ...,  # (1)
    AgentArns: Sequence[str] = ...,
    Name: str = ...,
    CloudWatchLogGroupArn: str = ...,
    Credentials: CredentialsTypeDef = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: DiscoveryServerConfigurationTypeDef](./type_defs.md#discoveryserverconfigurationtypedef) 
2. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 


```python
# update_storage_system method usage example with argument unpacking

kwargs: UpdateStorageSystemRequestRequestTypeDef = {  # (1)
    "StorageSystemArn": ...,
}

parent.update_storage_system(**kwargs)
```

1. See [:material-code-braces: UpdateStorageSystemRequestRequestTypeDef](./type_defs.md#updatestoragesystemrequestrequesttypedef) 

### update\_task

Updates the configuration of a <i>task</i>, which defines where and how
DataSync transfers your data.

Type annotations and code completion for `#!python session.create_client("datasync").update_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_task.html)

```python
# update_task method definition

await def update_task(
    self,
    *,
    TaskArn: str,
    Options: OptionsTypeDef = ...,  # (1)
    Excludes: Sequence[FilterRuleTypeDef] = ...,  # (2)
    Schedule: TaskScheduleTypeDef = ...,  # (3)
    Name: str = ...,
    CloudWatchLogGroupArn: str = ...,
    Includes: Sequence[FilterRuleTypeDef] = ...,  # (2)
    ManifestConfig: ManifestConfigTypeDef = ...,  # (5)
    TaskReportConfig: TaskReportConfigTypeDef = ...,  # (6)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: OptionsTypeDef](./type_defs.md#optionstypedef) 
2. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
3. See [:material-code-braces: TaskScheduleTypeDef](./type_defs.md#taskscheduletypedef) 
4. See [:material-code-braces: FilterRuleTypeDef](./type_defs.md#filterruletypedef) 
5. See [:material-code-braces: ManifestConfigTypeDef](./type_defs.md#manifestconfigtypedef) 
6. See [:material-code-braces: TaskReportConfigTypeDef](./type_defs.md#taskreportconfigtypedef) 


```python
# update_task method usage example with argument unpacking

kwargs: UpdateTaskRequestRequestTypeDef = {  # (1)
    "TaskArn": ...,
}

parent.update_task(**kwargs)
```

1. See [:material-code-braces: UpdateTaskRequestRequestTypeDef](./type_defs.md#updatetaskrequestrequesttypedef) 

### update\_task\_execution

Updates the configuration of a running DataSync task execution.

Type annotations and code completion for `#!python session.create_client("datasync").update_task_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_task_execution.html)

```python
# update_task_execution method definition

await def update_task_execution(
    self,
    *,
    TaskExecutionArn: str,
    Options: OptionsTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: OptionsTypeDef](./type_defs.md#optionstypedef) 


```python
# update_task_execution method usage example with argument unpacking

kwargs: UpdateTaskExecutionRequestRequestTypeDef = {  # (1)
    "TaskExecutionArn": ...,
    "Options": ...,
}

parent.update_task_execution(**kwargs)
```

1. See [:material-code-braces: UpdateTaskExecutionRequestRequestTypeDef](./type_defs.md#updatetaskexecutionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("datasync").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "DataSyncClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("datasync").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client)

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

Type annotations and code completion for `#!python session.create_client("datasync").get_paginator` method with overloads.

- `client.get_paginator("describe_storage_system_resource_metrics")` -> [DescribeStorageSystemResourceMetricsPaginator](./paginators.md#describestoragesystemresourcemetricspaginator)
- `client.get_paginator("list_agents")` -> [ListAgentsPaginator](./paginators.md#listagentspaginator)
- `client.get_paginator("list_discovery_jobs")` -> [ListDiscoveryJobsPaginator](./paginators.md#listdiscoveryjobspaginator)
- `client.get_paginator("list_locations")` -> [ListLocationsPaginator](./paginators.md#listlocationspaginator)
- `client.get_paginator("list_storage_systems")` -> [ListStorageSystemsPaginator](./paginators.md#liststoragesystemspaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- `client.get_paginator("list_task_executions")` -> [ListTaskExecutionsPaginator](./paginators.md#listtaskexecutionspaginator)
- `client.get_paginator("list_tasks")` -> [ListTasksPaginator](./paginators.md#listtaskspaginator)



