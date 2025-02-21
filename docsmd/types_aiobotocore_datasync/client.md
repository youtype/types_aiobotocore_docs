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

kwargs: AddStorageSystemRequestTypeDef = {  # (1)
    "ServerConfiguration": ...,
    "SystemType": ...,
    "AgentArns": ...,
    "ClientToken": ...,
    "Credentials": ...,
}

parent.add_storage_system(**kwargs)
```

1. See [:material-code-braces: AddStorageSystemRequestTypeDef](./type_defs.md#addstoragesystemrequesttypedef) 

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

kwargs: CancelTaskExecutionRequestTypeDef = {  # (1)
    "TaskExecutionArn": ...,
}

parent.cancel_task_execution(**kwargs)
```

1. See [:material-code-braces: CancelTaskExecutionRequestTypeDef](./type_defs.md#canceltaskexecutionrequesttypedef) 

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

kwargs: CreateAgentRequestTypeDef = {  # (1)
    "ActivationKey": ...,
}

parent.create_agent(**kwargs)
```

1. See [:material-code-braces: CreateAgentRequestTypeDef](./type_defs.md#createagentrequesttypedef) 

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

kwargs: CreateLocationAzureBlobRequestTypeDef = {  # (1)
    "ContainerUrl": ...,
    "AuthenticationType": ...,
    "AgentArns": ...,
}

parent.create_location_azure_blob(**kwargs)
```

1. See [:material-code-braces: CreateLocationAzureBlobRequestTypeDef](./type_defs.md#createlocationazureblobrequesttypedef) 

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
    Ec2Config: Ec2ConfigUnionTypeDef,  # (1)
    Subdirectory: str = ...,
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (2)
    AccessPointArn: str = ...,
    FileSystemAccessRoleArn: str = ...,
    InTransitEncryption: EfsInTransitEncryptionType = ...,  # (3)
) -> CreateLocationEfsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: Ec2ConfigTypeDef](./type_defs.md#ec2configtypedef) [:material-code-braces: Ec2ConfigOutputTypeDef](./type_defs.md#ec2configoutputtypedef) 
2. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
3. See [:material-code-brackets: EfsInTransitEncryptionType](./literals.md#efsintransitencryptiontype) 
4. See [:material-code-braces: CreateLocationEfsResponseTypeDef](./type_defs.md#createlocationefsresponsetypedef) 


```python
# create_location_efs method usage example with argument unpacking

kwargs: CreateLocationEfsRequestTypeDef = {  # (1)
    "EfsFilesystemArn": ...,
    "Ec2Config": ...,
}

parent.create_location_efs(**kwargs)
```

1. See [:material-code-braces: CreateLocationEfsRequestTypeDef](./type_defs.md#createlocationefsrequesttypedef) 

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

kwargs: CreateLocationFsxLustreRequestTypeDef = {  # (1)
    "FsxFilesystemArn": ...,
    "SecurityGroupArns": ...,
}

parent.create_location_fsx_lustre(**kwargs)
```

1. See [:material-code-braces: CreateLocationFsxLustreRequestTypeDef](./type_defs.md#createlocationfsxlustrerequesttypedef) 

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

kwargs: CreateLocationFsxOntapRequestTypeDef = {  # (1)
    "Protocol": ...,
    "SecurityGroupArns": ...,
    "StorageVirtualMachineArn": ...,
}

parent.create_location_fsx_ontap(**kwargs)
```

1. See [:material-code-braces: CreateLocationFsxOntapRequestTypeDef](./type_defs.md#createlocationfsxontaprequesttypedef) 

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

kwargs: CreateLocationFsxOpenZfsRequestTypeDef = {  # (1)
    "FsxFilesystemArn": ...,
    "Protocol": ...,
    "SecurityGroupArns": ...,
}

parent.create_location_fsx_open_zfs(**kwargs)
```

1. See [:material-code-braces: CreateLocationFsxOpenZfsRequestTypeDef](./type_defs.md#createlocationfsxopenzfsrequesttypedef) 

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

kwargs: CreateLocationFsxWindowsRequestTypeDef = {  # (1)
    "FsxFilesystemArn": ...,
    "SecurityGroupArns": ...,
    "User": ...,
    "Password": ...,
}

parent.create_location_fsx_windows(**kwargs)
```

1. See [:material-code-braces: CreateLocationFsxWindowsRequestTypeDef](./type_defs.md#createlocationfsxwindowsrequesttypedef) 

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

kwargs: CreateLocationHdfsRequestTypeDef = {  # (1)
    "NameNodes": ...,
    "AuthenticationType": ...,
    "AgentArns": ...,
}

parent.create_location_hdfs(**kwargs)
```

1. See [:material-code-braces: CreateLocationHdfsRequestTypeDef](./type_defs.md#createlocationhdfsrequesttypedef) 

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
    OnPremConfig: OnPremConfigUnionTypeDef,  # (1)
    MountOptions: NfsMountOptionsTypeDef = ...,  # (2)
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (3)
) -> CreateLocationNfsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: OnPremConfigTypeDef](./type_defs.md#onpremconfigtypedef) [:material-code-braces: OnPremConfigOutputTypeDef](./type_defs.md#onpremconfigoutputtypedef) 
2. See [:material-code-braces: NfsMountOptionsTypeDef](./type_defs.md#nfsmountoptionstypedef) 
3. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
4. See [:material-code-braces: CreateLocationNfsResponseTypeDef](./type_defs.md#createlocationnfsresponsetypedef) 


```python
# create_location_nfs method usage example with argument unpacking

kwargs: CreateLocationNfsRequestTypeDef = {  # (1)
    "Subdirectory": ...,
    "ServerHostname": ...,
    "OnPremConfig": ...,
}

parent.create_location_nfs(**kwargs)
```

1. See [:material-code-braces: CreateLocationNfsRequestTypeDef](./type_defs.md#createlocationnfsrequesttypedef) 

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

kwargs: CreateLocationObjectStorageRequestTypeDef = {  # (1)
    "ServerHostname": ...,
    "BucketName": ...,
    "AgentArns": ...,
}

parent.create_location_object_storage(**kwargs)
```

1. See [:material-code-braces: CreateLocationObjectStorageRequestTypeDef](./type_defs.md#createlocationobjectstoragerequesttypedef) 

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

kwargs: CreateLocationS3RequestTypeDef = {  # (1)
    "S3BucketArn": ...,
    "S3Config": ...,
}

parent.create_location_s3(**kwargs)
```

1. See [:material-code-braces: CreateLocationS3RequestTypeDef](./type_defs.md#createlocations3requesttypedef) 

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
    AgentArns: Sequence[str],
    User: str = ...,
    Domain: str = ...,
    Password: str = ...,
    MountOptions: SmbMountOptionsTypeDef = ...,  # (1)
    Tags: Sequence[TagListEntryTypeDef] = ...,  # (2)
    AuthenticationType: SmbAuthenticationTypeType = ...,  # (3)
    DnsIpAddresses: Sequence[str] = ...,
    KerberosPrincipal: str = ...,
    KerberosKeytab: BlobTypeDef = ...,
    KerberosKrb5Conf: BlobTypeDef = ...,
) -> CreateLocationSmbResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: SmbMountOptionsTypeDef](./type_defs.md#smbmountoptionstypedef) 
2. See [:material-code-braces: TagListEntryTypeDef](./type_defs.md#taglistentrytypedef) 
3. See [:material-code-brackets: SmbAuthenticationTypeType](./literals.md#smbauthenticationtypetype) 
4. See [:material-code-braces: CreateLocationSmbResponseTypeDef](./type_defs.md#createlocationsmbresponsetypedef) 


```python
# create_location_smb method usage example with argument unpacking

kwargs: CreateLocationSmbRequestTypeDef = {  # (1)
    "Subdirectory": ...,
    "ServerHostname": ...,
    "AgentArns": ...,
}

parent.create_location_smb(**kwargs)
```

1. See [:material-code-braces: CreateLocationSmbRequestTypeDef](./type_defs.md#createlocationsmbrequesttypedef) 

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

kwargs: CreateTaskRequestTypeDef = {  # (1)
    "SourceLocationArn": ...,
    "DestinationLocationArn": ...,
}

parent.create_task(**kwargs)
```

1. See [:material-code-braces: CreateTaskRequestTypeDef](./type_defs.md#createtaskrequesttypedef) 

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

kwargs: DeleteAgentRequestTypeDef = {  # (1)
    "AgentArn": ...,
}

parent.delete_agent(**kwargs)
```

1. See [:material-code-braces: DeleteAgentRequestTypeDef](./type_defs.md#deleteagentrequesttypedef) 

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

kwargs: DeleteLocationRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.delete_location(**kwargs)
```

1. See [:material-code-braces: DeleteLocationRequestTypeDef](./type_defs.md#deletelocationrequesttypedef) 

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

kwargs: DeleteTaskRequestTypeDef = {  # (1)
    "TaskArn": ...,
}

parent.delete_task(**kwargs)
```

1. See [:material-code-braces: DeleteTaskRequestTypeDef](./type_defs.md#deletetaskrequesttypedef) 

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

kwargs: DescribeAgentRequestTypeDef = {  # (1)
    "AgentArn": ...,
}

parent.describe_agent(**kwargs)
```

1. See [:material-code-braces: DescribeAgentRequestTypeDef](./type_defs.md#describeagentrequesttypedef) 

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

kwargs: DescribeDiscoveryJobRequestTypeDef = {  # (1)
    "DiscoveryJobArn": ...,
}

parent.describe_discovery_job(**kwargs)
```

1. See [:material-code-braces: DescribeDiscoveryJobRequestTypeDef](./type_defs.md#describediscoveryjobrequesttypedef) 

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

kwargs: DescribeLocationAzureBlobRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_azure_blob(**kwargs)
```

1. See [:material-code-braces: DescribeLocationAzureBlobRequestTypeDef](./type_defs.md#describelocationazureblobrequesttypedef) 

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

kwargs: DescribeLocationEfsRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_efs(**kwargs)
```

1. See [:material-code-braces: DescribeLocationEfsRequestTypeDef](./type_defs.md#describelocationefsrequesttypedef) 

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

kwargs: DescribeLocationFsxLustreRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_fsx_lustre(**kwargs)
```

1. See [:material-code-braces: DescribeLocationFsxLustreRequestTypeDef](./type_defs.md#describelocationfsxlustrerequesttypedef) 

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

kwargs: DescribeLocationFsxOntapRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_fsx_ontap(**kwargs)
```

1. See [:material-code-braces: DescribeLocationFsxOntapRequestTypeDef](./type_defs.md#describelocationfsxontaprequesttypedef) 

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

kwargs: DescribeLocationFsxOpenZfsRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_fsx_open_zfs(**kwargs)
```

1. See [:material-code-braces: DescribeLocationFsxOpenZfsRequestTypeDef](./type_defs.md#describelocationfsxopenzfsrequesttypedef) 

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

kwargs: DescribeLocationFsxWindowsRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_fsx_windows(**kwargs)
```

1. See [:material-code-braces: DescribeLocationFsxWindowsRequestTypeDef](./type_defs.md#describelocationfsxwindowsrequesttypedef) 

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

kwargs: DescribeLocationHdfsRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_hdfs(**kwargs)
```

1. See [:material-code-braces: DescribeLocationHdfsRequestTypeDef](./type_defs.md#describelocationhdfsrequesttypedef) 

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

kwargs: DescribeLocationNfsRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_nfs(**kwargs)
```

1. See [:material-code-braces: DescribeLocationNfsRequestTypeDef](./type_defs.md#describelocationnfsrequesttypedef) 

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

kwargs: DescribeLocationObjectStorageRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_object_storage(**kwargs)
```

1. See [:material-code-braces: DescribeLocationObjectStorageRequestTypeDef](./type_defs.md#describelocationobjectstoragerequesttypedef) 

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

kwargs: DescribeLocationS3RequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_s3(**kwargs)
```

1. See [:material-code-braces: DescribeLocationS3RequestTypeDef](./type_defs.md#describelocations3requesttypedef) 

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

kwargs: DescribeLocationSmbRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.describe_location_smb(**kwargs)
```

1. See [:material-code-braces: DescribeLocationSmbRequestTypeDef](./type_defs.md#describelocationsmbrequesttypedef) 

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

kwargs: DescribeStorageSystemRequestTypeDef = {  # (1)
    "StorageSystemArn": ...,
}

parent.describe_storage_system(**kwargs)
```

1. See [:material-code-braces: DescribeStorageSystemRequestTypeDef](./type_defs.md#describestoragesystemrequesttypedef) 

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

kwargs: DescribeStorageSystemResourceMetricsRequestTypeDef = {  # (1)
    "DiscoveryJobArn": ...,
    "ResourceType": ...,
    "ResourceId": ...,
}

parent.describe_storage_system_resource_metrics(**kwargs)
```

1. See [:material-code-braces: DescribeStorageSystemResourceMetricsRequestTypeDef](./type_defs.md#describestoragesystemresourcemetricsrequesttypedef) 

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

kwargs: DescribeStorageSystemResourcesRequestTypeDef = {  # (1)
    "DiscoveryJobArn": ...,
    "ResourceType": ...,
}

parent.describe_storage_system_resources(**kwargs)
```

1. See [:material-code-braces: DescribeStorageSystemResourcesRequestTypeDef](./type_defs.md#describestoragesystemresourcesrequesttypedef) 

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

kwargs: DescribeTaskRequestTypeDef = {  # (1)
    "TaskArn": ...,
}

parent.describe_task(**kwargs)
```

1. See [:material-code-braces: DescribeTaskRequestTypeDef](./type_defs.md#describetaskrequesttypedef) 

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

kwargs: DescribeTaskExecutionRequestTypeDef = {  # (1)
    "TaskExecutionArn": ...,
}

parent.describe_task_execution(**kwargs)
```

1. See [:material-code-braces: DescribeTaskExecutionRequestTypeDef](./type_defs.md#describetaskexecutionrequesttypedef) 

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

kwargs: GenerateRecommendationsRequestTypeDef = {  # (1)
    "DiscoveryJobArn": ...,
    "ResourceIds": ...,
    "ResourceType": ...,
}

parent.generate_recommendations(**kwargs)
```

1. See [:material-code-braces: GenerateRecommendationsRequestTypeDef](./type_defs.md#generaterecommendationsrequesttypedef) 

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

kwargs: ListAgentsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_agents(**kwargs)
```

1. See [:material-code-braces: ListAgentsRequestTypeDef](./type_defs.md#listagentsrequesttypedef) 

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

kwargs: ListDiscoveryJobsRequestTypeDef = {  # (1)
    "StorageSystemArn": ...,
}

parent.list_discovery_jobs(**kwargs)
```

1. See [:material-code-braces: ListDiscoveryJobsRequestTypeDef](./type_defs.md#listdiscoveryjobsrequesttypedef) 

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

kwargs: ListLocationsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_locations(**kwargs)
```

1. See [:material-code-braces: ListLocationsRequestTypeDef](./type_defs.md#listlocationsrequesttypedef) 

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

kwargs: ListStorageSystemsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_storage_systems(**kwargs)
```

1. See [:material-code-braces: ListStorageSystemsRequestTypeDef](./type_defs.md#liststoragesystemsrequesttypedef) 

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

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

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

kwargs: ListTaskExecutionsRequestTypeDef = {  # (1)
    "TaskArn": ...,
}

parent.list_task_executions(**kwargs)
```

1. See [:material-code-braces: ListTaskExecutionsRequestTypeDef](./type_defs.md#listtaskexecutionsrequesttypedef) 

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

kwargs: ListTasksRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_tasks(**kwargs)
```

1. See [:material-code-braces: ListTasksRequestTypeDef](./type_defs.md#listtasksrequesttypedef) 

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

kwargs: RemoveStorageSystemRequestTypeDef = {  # (1)
    "StorageSystemArn": ...,
}

parent.remove_storage_system(**kwargs)
```

1. See [:material-code-braces: RemoveStorageSystemRequestTypeDef](./type_defs.md#removestoragesystemrequesttypedef) 

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

kwargs: StartDiscoveryJobRequestTypeDef = {  # (1)
    "StorageSystemArn": ...,
    "CollectionDurationMinutes": ...,
    "ClientToken": ...,
}

parent.start_discovery_job(**kwargs)
```

1. See [:material-code-braces: StartDiscoveryJobRequestTypeDef](./type_defs.md#startdiscoveryjobrequesttypedef) 

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

kwargs: StartTaskExecutionRequestTypeDef = {  # (1)
    "TaskArn": ...,
}

parent.start_task_execution(**kwargs)
```

1. See [:material-code-braces: StartTaskExecutionRequestTypeDef](./type_defs.md#starttaskexecutionrequesttypedef) 

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

kwargs: StopDiscoveryJobRequestTypeDef = {  # (1)
    "DiscoveryJobArn": ...,
}

parent.stop_discovery_job(**kwargs)
```

1. See [:material-code-braces: StopDiscoveryJobRequestTypeDef](./type_defs.md#stopdiscoveryjobrequesttypedef) 

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

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

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

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Keys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

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

kwargs: UpdateAgentRequestTypeDef = {  # (1)
    "AgentArn": ...,
}

parent.update_agent(**kwargs)
```

1. See [:material-code-braces: UpdateAgentRequestTypeDef](./type_defs.md#updateagentrequesttypedef) 

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

kwargs: UpdateDiscoveryJobRequestTypeDef = {  # (1)
    "DiscoveryJobArn": ...,
    "CollectionDurationMinutes": ...,
}

parent.update_discovery_job(**kwargs)
```

1. See [:material-code-braces: UpdateDiscoveryJobRequestTypeDef](./type_defs.md#updatediscoveryjobrequesttypedef) 

### update\_location\_azure\_blob

Modifies the following configurations of the Microsoft Azure Blob Storage
transfer location that you're using with DataSync.

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

kwargs: UpdateLocationAzureBlobRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_azure_blob(**kwargs)
```

1. See [:material-code-braces: UpdateLocationAzureBlobRequestTypeDef](./type_defs.md#updatelocationazureblobrequesttypedef) 

### update\_location\_efs

Modifies the following configuration parameters of the Amazon EFS transfer
location that you're using with DataSync.

Type annotations and code completion for `#!python session.create_client("datasync").update_location_efs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_location_efs.html)

```python
# update_location_efs method definition

await def update_location_efs(
    self,
    *,
    LocationArn: str,
    Subdirectory: str = ...,
    AccessPointArn: str = ...,
    FileSystemAccessRoleArn: str = ...,
    InTransitEncryption: EfsInTransitEncryptionType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: EfsInTransitEncryptionType](./literals.md#efsintransitencryptiontype) 


```python
# update_location_efs method usage example with argument unpacking

kwargs: UpdateLocationEfsRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_efs(**kwargs)
```

1. See [:material-code-braces: UpdateLocationEfsRequestTypeDef](./type_defs.md#updatelocationefsrequesttypedef) 

### update\_location\_fsx\_lustre

Modifies the following configuration parameters of the Amazon FSx for Lustre
transfer location that you're using with DataSync.

Type annotations and code completion for `#!python session.create_client("datasync").update_location_fsx_lustre` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_location_fsx_lustre.html)

```python
# update_location_fsx_lustre method definition

await def update_location_fsx_lustre(
    self,
    *,
    LocationArn: str,
    Subdirectory: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_location_fsx_lustre method usage example with argument unpacking

kwargs: UpdateLocationFsxLustreRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_fsx_lustre(**kwargs)
```

1. See [:material-code-braces: UpdateLocationFsxLustreRequestTypeDef](./type_defs.md#updatelocationfsxlustrerequesttypedef) 

### update\_location\_fsx\_ontap

Modifies the following configuration parameters of the Amazon FSx for NetApp
ONTAP transfer location that you're using with DataSync.

Type annotations and code completion for `#!python session.create_client("datasync").update_location_fsx_ontap` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_location_fsx_ontap.html)

```python
# update_location_fsx_ontap method definition

await def update_location_fsx_ontap(
    self,
    *,
    LocationArn: str,
    Protocol: FsxUpdateProtocolTypeDef = ...,  # (1)
    Subdirectory: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: FsxUpdateProtocolTypeDef](./type_defs.md#fsxupdateprotocoltypedef) 


```python
# update_location_fsx_ontap method usage example with argument unpacking

kwargs: UpdateLocationFsxOntapRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_fsx_ontap(**kwargs)
```

1. See [:material-code-braces: UpdateLocationFsxOntapRequestTypeDef](./type_defs.md#updatelocationfsxontaprequesttypedef) 

### update\_location\_fsx\_open\_zfs

Modifies the following configuration parameters of the Amazon FSx for OpenZFS
transfer location that you're using with DataSync.

Type annotations and code completion for `#!python session.create_client("datasync").update_location_fsx_open_zfs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_location_fsx_open_zfs.html)

```python
# update_location_fsx_open_zfs method definition

await def update_location_fsx_open_zfs(
    self,
    *,
    LocationArn: str,
    Protocol: FsxProtocolTypeDef = ...,  # (1)
    Subdirectory: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: FsxProtocolTypeDef](./type_defs.md#fsxprotocoltypedef) 


```python
# update_location_fsx_open_zfs method usage example with argument unpacking

kwargs: UpdateLocationFsxOpenZfsRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_fsx_open_zfs(**kwargs)
```

1. See [:material-code-braces: UpdateLocationFsxOpenZfsRequestTypeDef](./type_defs.md#updatelocationfsxopenzfsrequesttypedef) 

### update\_location\_fsx\_windows

Modifies the following configuration parameters of the Amazon FSx for Windows
File Server transfer location that you're using with DataSync.

Type annotations and code completion for `#!python session.create_client("datasync").update_location_fsx_windows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_location_fsx_windows.html)

```python
# update_location_fsx_windows method definition

await def update_location_fsx_windows(
    self,
    *,
    LocationArn: str,
    Subdirectory: str = ...,
    Domain: str = ...,
    User: str = ...,
    Password: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_location_fsx_windows method usage example with argument unpacking

kwargs: UpdateLocationFsxWindowsRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_fsx_windows(**kwargs)
```

1. See [:material-code-braces: UpdateLocationFsxWindowsRequestTypeDef](./type_defs.md#updatelocationfsxwindowsrequesttypedef) 

### update\_location\_hdfs

Modifies the following configuration parameters of the Hadoop Distributed File
System (HDFS) transfer location that you're using with DataSync.

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

kwargs: UpdateLocationHdfsRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_hdfs(**kwargs)
```

1. See [:material-code-braces: UpdateLocationHdfsRequestTypeDef](./type_defs.md#updatelocationhdfsrequesttypedef) 

### update\_location\_nfs

Modifies the following configuration parameters of the Network File System
(NFS) transfer location that you're using with DataSync.

Type annotations and code completion for `#!python session.create_client("datasync").update_location_nfs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_location_nfs.html)

```python
# update_location_nfs method definition

await def update_location_nfs(
    self,
    *,
    LocationArn: str,
    Subdirectory: str = ...,
    OnPremConfig: OnPremConfigUnionTypeDef = ...,  # (1)
    MountOptions: NfsMountOptionsTypeDef = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: OnPremConfigTypeDef](./type_defs.md#onpremconfigtypedef) [:material-code-braces: OnPremConfigOutputTypeDef](./type_defs.md#onpremconfigoutputtypedef) 
2. See [:material-code-braces: NfsMountOptionsTypeDef](./type_defs.md#nfsmountoptionstypedef) 


```python
# update_location_nfs method usage example with argument unpacking

kwargs: UpdateLocationNfsRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_nfs(**kwargs)
```

1. See [:material-code-braces: UpdateLocationNfsRequestTypeDef](./type_defs.md#updatelocationnfsrequesttypedef) 

### update\_location\_object\_storage

Modifies the following configuration parameters of the object storage transfer
location that you're using with DataSync.

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

kwargs: UpdateLocationObjectStorageRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_object_storage(**kwargs)
```

1. See [:material-code-braces: UpdateLocationObjectStorageRequestTypeDef](./type_defs.md#updatelocationobjectstoragerequesttypedef) 

### update\_location\_s3

Modifies the following configuration parameters of the Amazon S3 transfer
location that you're using with DataSync.

Type annotations and code completion for `#!python session.create_client("datasync").update_location_s3` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/client/update_location_s3.html)

```python
# update_location_s3 method definition

await def update_location_s3(
    self,
    *,
    LocationArn: str,
    Subdirectory: str = ...,
    S3StorageClass: S3StorageClassType = ...,  # (1)
    S3Config: S3ConfigTypeDef = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: S3StorageClassType](./literals.md#s3storageclasstype) 
2. See [:material-code-braces: S3ConfigTypeDef](./type_defs.md#s3configtypedef) 


```python
# update_location_s3 method usage example with argument unpacking

kwargs: UpdateLocationS3RequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_s3(**kwargs)
```

1. See [:material-code-braces: UpdateLocationS3RequestTypeDef](./type_defs.md#updatelocations3requesttypedef) 

### update\_location\_smb

Modifies the following configuration parameters of the Server Message Block
(SMB) transfer location that you're using with DataSync.

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
    AuthenticationType: SmbAuthenticationTypeType = ...,  # (2)
    DnsIpAddresses: Sequence[str] = ...,
    KerberosPrincipal: str = ...,
    KerberosKeytab: BlobTypeDef = ...,
    KerberosKrb5Conf: BlobTypeDef = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: SmbMountOptionsTypeDef](./type_defs.md#smbmountoptionstypedef) 
2. See [:material-code-brackets: SmbAuthenticationTypeType](./literals.md#smbauthenticationtypetype) 


```python
# update_location_smb method usage example with argument unpacking

kwargs: UpdateLocationSmbRequestTypeDef = {  # (1)
    "LocationArn": ...,
}

parent.update_location_smb(**kwargs)
```

1. See [:material-code-braces: UpdateLocationSmbRequestTypeDef](./type_defs.md#updatelocationsmbrequesttypedef) 

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

kwargs: UpdateStorageSystemRequestTypeDef = {  # (1)
    "StorageSystemArn": ...,
}

parent.update_storage_system(**kwargs)
```

1. See [:material-code-braces: UpdateStorageSystemRequestTypeDef](./type_defs.md#updatestoragesystemrequesttypedef) 

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

kwargs: UpdateTaskRequestTypeDef = {  # (1)
    "TaskArn": ...,
}

parent.update_task(**kwargs)
```

1. See [:material-code-braces: UpdateTaskRequestTypeDef](./type_defs.md#updatetaskrequesttypedef) 

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

kwargs: UpdateTaskExecutionRequestTypeDef = {  # (1)
    "TaskExecutionArn": ...,
    "Options": ...,
}

parent.update_task_execution(**kwargs)
```

1. See [:material-code-braces: UpdateTaskExecutionRequestTypeDef](./type_defs.md#updatetaskexecutionrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("datasync").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("datasync").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
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



