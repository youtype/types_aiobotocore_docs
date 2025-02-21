# GlacierServiceResource

> [Index](../README.md) > [Glacier](./README.md) > GlacierServiceResource

!!! note ""

    Auto-generated documentation for [Glacier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#glacier)
    type annotations stubs module [types-aiobotocore-glacier](https://pypi.org/project/types-aiobotocore-glacier/).

## GlacierServiceResource

Type annotations and code completion for `#!python session.resource("glacier")`, included resources and collections.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/service-resource/index.html)

```python
# GlacierServiceResource usage example

from types_aiobotocore_glacier.service_resource import GlacierServiceResource

def get_glacier_resource() -> GlacierServiceResource:
    return session.resource("glacier")
```


## Attributes


- `meta`: `GlacierResourceMeta`

- `vaults`: `ServiceResourceVaultsCollection`




## Collections

### ServiceResourceVaultsCollection

Provides access to [Vault](#vault) resource.

Type annotations and code completion for `#!python session.resource("glacier").vaults` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/service-resource/vaults.html#Glacier.ServiceResource.vaults)

```python
# ServiceResourceVaultsCollection usage example

from types_aiobotocore_glacier.service_resource import ServiceResourceVaultsCollection

def get_collection() -> ServiceResourceVaultsCollection:
    return session.resource("glacier").vaults
```



## Methods

### GlacierServiceResource.get\_available\_subresources method

Returns a list of all the available sub-resources for this resource.

Type annotations and code completion for `#!python session.resource("glacier").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/service-resource/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


### GlacierServiceResource.create\_vault method

This operation creates a new vault with the specified name.

Type annotations and code completion for `#!python session.resource("glacier").create_vault` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/service-resource/create_vault.html)

```python
# create_vault method definition

await def create_vault(
    self,
    *,
    vaultName: str,
    accountId: str = '-',
) -> _Vault:
    ...
```



```python
# create_vault method usage example with argument unpacking

kwargs: CreateVaultInputServiceResourceCreateVaultTypeDef = {  # (1)
    "vaultName": ...,
}

parent.create_vault(**kwargs)
```

1. See [:material-code-braces: CreateVaultInputServiceResourceCreateVaultTypeDef](./type_defs.md#createvaultinputserviceresourcecreatevaulttypedef) 

### GlacierServiceResource.Account method

Creates a Account resource.

Type annotations and code completion for `#!python session.resource("glacier").Account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/service-resource/Account.html)

```python
# Account method definition

await def Account(
    self,
    id: str,
) -> _Account:
    ...
```


### GlacierServiceResource.Archive method

Creates a Archive resource.

Type annotations and code completion for `#!python session.resource("glacier").Archive` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/service-resource/Archive.html)

```python
# Archive method definition

await def Archive(
    self,
    account_id: str,
    vault_name: str,
    id: str,
) -> _Archive:
    ...
```


### GlacierServiceResource.Job method

Creates a Job resource.

Type annotations and code completion for `#!python session.resource("glacier").Job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/service-resource/Job.html)

```python
# Job method definition

await def Job(
    self,
    account_id: str,
    vault_name: str,
    id: str,
) -> _Job:
    ...
```


### GlacierServiceResource.MultipartUpload method

Creates a MultipartUpload resource.

Type annotations and code completion for `#!python session.resource("glacier").MultipartUpload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/service-resource/MultipartUpload.html)

```python
# MultipartUpload method definition

await def MultipartUpload(
    self,
    account_id: str,
    vault_name: str,
    id: str,
) -> _MultipartUpload:
    ...
```


### GlacierServiceResource.Notification method

Creates a Notification resource.

Type annotations and code completion for `#!python session.resource("glacier").Notification` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/service-resource/Notification.html)

```python
# Notification method definition

await def Notification(
    self,
    account_id: str,
    vault_name: str,
) -> _Notification:
    ...
```


### GlacierServiceResource.Vault method

Creates a Vault resource.

Type annotations and code completion for `#!python session.resource("glacier").Vault` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/service-resource/Vault.html)

```python
# Vault method definition

await def Vault(
    self,
    account_id: str,
    name: str,
) -> _Vault:
    ...
```




## Account

Type annotations and code completion for `#!python session.resource("glacier").Account` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/account/index.html#Glacier.Account)

```python
# Account usage example

from types_aiobotocore_glacier.service_resource import Account

def get_resource() -> Account:
    return session.resource("glacier").Account(...)
```


### Account attributes


- `id`: `str`
- `vaults`: `AccountVaultsCollection`
- `meta`: `GlacierResourceMeta`



### Account collections


#### Account.vaults

Provides access to [Vault](#vault) resource.

Type annotations and code completion for `#!python session.resource("glacier").Account(...).vaults` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/account/vaults.html#Glacier.Account.vaults)

```python
# AccountVaultsCollection usage example

from types_aiobotocore_glacier.service_resource import AccountVaultsCollection

def get_collection() -> AccountVaultsCollection:
    resource = session.resource("glacier").Account(...)
    return resource.vaults
```




### Account methods


#### Account.get\_available\_subresources method

Returns a list of all the available sub-resources for this Account.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/account/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Account.create\_vault method

This operation creates a new vault with the specified name.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").create_vault` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/account/create_vault.html)

```python
# create_vault method definition

await def create_vault(
    self,
    *,
    vaultName: str,
) -> _Vault:
    ...
```



```python
# create_vault method usage example with argument unpacking

kwargs: CreateVaultInputAccountCreateVaultTypeDef = {  # (1)
    "vaultName": ...,
}

parent.create_vault(**kwargs)
```

1. See [:material-code-braces: CreateVaultInputAccountCreateVaultTypeDef](./type_defs.md#createvaultinputaccountcreatevaulttypedef) 

#### Account.Vault method

Creates a Vault resource.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").Vault` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/account/Vault.html)

```python
# Vault method definition

await def Vault(
    self,
    name: str,
) -> _Vault:
    ...
```





## Archive

Type annotations and code completion for `#!python session.resource("glacier").Archive` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/archive/index.html#Glacier.Archive)

```python
# Archive usage example

from types_aiobotocore_glacier.service_resource import Archive

def get_resource() -> Archive:
    return session.resource("glacier").Archive(...)
```


### Archive attributes


- `account_id`: `str`
- `vault_name`: `str`
- `id`: `str`
- `meta`: `GlacierResourceMeta`





### Archive methods


#### Archive.get\_available\_subresources method

Returns a list of all the available sub-resources for this Archive.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/archive/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Archive.delete method

This operation deletes an archive from a vault.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/archive/delete.html)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Archive.initiate\_archive\_retrieval method

This operation initiates a job of the specified type, which can be a select, an
archival retrieval, or a vault retrieval.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").initiate_archive_retrieval` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/archive/initiate_archive_retrieval.html)

```python
# initiate_archive_retrieval method definition

await def initiate_archive_retrieval(
    self,
) -> _Job:
    ...
```


#### Archive.Vault method

Creates a Vault resource.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").Vault` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/archive/Vault.html)

```python
# Vault method definition

await def Vault(
    self,
) -> _Vault:
    ...
```





## Job

Type annotations and code completion for `#!python session.resource("glacier").Job` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/job/index.html#Glacier.Job)

```python
# Job usage example

from types_aiobotocore_glacier.service_resource import Job

def get_resource() -> Job:
    return session.resource("glacier").Job(...)
```


### Job attributes


- `account_id`: `str`
- `vault_name`: `str`
- `id`: `str`
- `job_id`: `Awaitable`[`str`]
- `job_description`: `Awaitable`[`str`]
- `action`: `Awaitable`[[ActionCodeType](./literals.md#actioncodetype)]
- `archive_id`: `Awaitable`[`str`]
- `vault_arn`: `Awaitable`[`str`]
- `creation_date`: `Awaitable`[`str`]
- `completed`: `Awaitable`[`bool`]
- `status_code`: `Awaitable`[[StatusCodeType](./literals.md#statuscodetype)]
- `status_message`: `Awaitable`[`str`]
- `archive_size_in_bytes`: `Awaitable`[`int`]
- `inventory_size_in_bytes`: `Awaitable`[`int`]
- `sns_topic`: `Awaitable`[`str`]
- `completion_date`: `Awaitable`[`str`]
- `sha256_tree_hash`: `Awaitable`[`str`]
- `archive_sha256_tree_hash`: `Awaitable`[`str`]
- `retrieval_byte_range`: `Awaitable`[`str`]
- `tier`: `Awaitable`[`str`]
- `inventory_retrieval_parameters`: `Awaitable`[[InventoryRetrievalJobDescriptionTypeDef](./type_defs.md#inventoryretrievaljobdescriptiontypedef)]
- `job_output_path`: `Awaitable`[`str`]
- `select_parameters`: `Awaitable`[[SelectParametersTypeDef](./type_defs.md#selectparameterstypedef)]
- `output_location`: `Awaitable`[[OutputLocationOutputTypeDef](./type_defs.md#outputlocationoutputtypedef)]
- `meta`: `GlacierResourceMeta`





### Job methods


#### Job.get\_available\_subresources method

Returns a list of all the available sub-resources for this Job.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/job/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Job.get\_output method

This operation downloads the output of the job you initiated using
<a>InitiateJob</a>.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").get_output` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/job/get_output.html)

```python
# get_output method definition

await def get_output(
    self,
    *,
    range: str = ...,
) -> GetJobOutputOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobOutputOutputTypeDef](./type_defs.md#getjoboutputoutputtypedef) 


```python
# get_output method usage example with argument unpacking

kwargs: GetJobOutputInputJobGetOutputTypeDef = {  # (1)
    "range": ...,
}

parent.get_output(**kwargs)
```

1. See [:material-code-braces: GetJobOutputInputJobGetOutputTypeDef](./type_defs.md#getjoboutputinputjobgetoutputtypedef) 

#### Job.Vault method

Creates a Vault resource.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").Vault` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/job/Vault.html)

```python
# Vault method definition

await def Vault(
    self,
) -> _Vault:
    ...
```


#### Job.load method



Type annotations and code completion for `#!python aiobotocore.resource("glacier").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/job/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Job.reload method



Type annotations and code completion for `#!python aiobotocore.resource("glacier").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/job/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## MultipartUpload

Type annotations and code completion for `#!python session.resource("glacier").MultipartUpload` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/multipartupload/index.html#Glacier.MultipartUpload)

```python
# MultipartUpload usage example

from types_aiobotocore_glacier.service_resource import MultipartUpload

def get_resource() -> MultipartUpload:
    return session.resource("glacier").MultipartUpload(...)
```


### MultipartUpload attributes


- `account_id`: `str`
- `vault_name`: `str`
- `id`: `str`
- `multipart_upload_id`: `Awaitable`[`str`]
- `vault_arn`: `Awaitable`[`str`]
- `archive_description`: `Awaitable`[`str`]
- `part_size_in_bytes`: `Awaitable`[`int`]
- `creation_date`: `Awaitable`[`str`]
- `meta`: `GlacierResourceMeta`





### MultipartUpload methods


#### MultipartUpload.get\_available\_subresources method

Returns a list of all the available sub-resources for this MultipartUpload.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/multipartupload/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### MultipartUpload.abort method

This operation aborts a multipart upload identified by the upload ID.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").abort` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/multipartupload/abort.html)

```python
# abort method definition

await def abort(
    self,
) -> None:
    ...
```


#### MultipartUpload.complete method

You call this operation to inform Amazon S3 Glacier (Glacier) that all the
archive parts have been uploaded and that Glacier can now assemble the archive
from the uploaded parts.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").complete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/multipartupload/complete.html)

```python
# complete method definition

await def complete(
    self,
    *,
    archiveSize: str = ...,
    checksum: str = ...,
) -> ArchiveCreationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ArchiveCreationOutputTypeDef](./type_defs.md#archivecreationoutputtypedef) 


```python
# complete method usage example with argument unpacking

kwargs: CompleteMultipartUploadInputMultipartUploadCompleteTypeDef = {  # (1)
    "archiveSize": ...,
}

parent.complete(**kwargs)
```

1. See [:material-code-braces: CompleteMultipartUploadInputMultipartUploadCompleteTypeDef](./type_defs.md#completemultipartuploadinputmultipartuploadcompletetypedef) 

#### MultipartUpload.parts method

This operation lists the parts of an archive that have been uploaded in a
specific multipart upload.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").parts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/multipartupload/parts.html)

```python
# parts method definition

await def parts(
    self,
    *,
    marker: str = ...,
    limit: str = ...,
) -> ListPartsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPartsOutputTypeDef](./type_defs.md#listpartsoutputtypedef) 


```python
# parts method usage example with argument unpacking

kwargs: ListPartsInputMultipartUploadPartsTypeDef = {  # (1)
    "marker": ...,
}

parent.parts(**kwargs)
```

1. See [:material-code-braces: ListPartsInputMultipartUploadPartsTypeDef](./type_defs.md#listpartsinputmultipartuploadpartstypedef) 

#### MultipartUpload.upload\_part method

This operation uploads a part of an archive.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").upload_part` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/multipartupload/upload_part.html)

```python
# upload_part method definition

await def upload_part(
    self,
    *,
    checksum: str = ...,
    range: str = ...,
    body: BlobTypeDef = ...,
) -> UploadMultipartPartOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UploadMultipartPartOutputTypeDef](./type_defs.md#uploadmultipartpartoutputtypedef) 


```python
# upload_part method usage example with argument unpacking

kwargs: UploadMultipartPartInputMultipartUploadUploadPartTypeDef = {  # (1)
    "checksum": ...,
}

parent.upload_part(**kwargs)
```

1. See [:material-code-braces: UploadMultipartPartInputMultipartUploadUploadPartTypeDef](./type_defs.md#uploadmultipartpartinputmultipartuploaduploadparttypedef) 

#### MultipartUpload.Vault method

Creates a Vault resource.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").Vault` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/multipartupload/Vault.html)

```python
# Vault method definition

await def Vault(
    self,
) -> _Vault:
    ...
```





## Notification

Type annotations and code completion for `#!python session.resource("glacier").Notification` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/notification/index.html#Glacier.Notification)

```python
# Notification usage example

from types_aiobotocore_glacier.service_resource import Notification

def get_resource() -> Notification:
    return session.resource("glacier").Notification(...)
```


### Notification attributes


- `account_id`: `str`
- `vault_name`: `str`
- `sns_topic`: `Awaitable`[`str`]
- `events`: `Awaitable`[`List`[`str`]]
- `meta`: `GlacierResourceMeta`





### Notification methods


#### Notification.get\_available\_subresources method

Returns a list of all the available sub-resources for this Notification.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/notification/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Notification.delete method

This operation deletes the notification configuration set for a vault.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/notification/delete.html)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Notification.set method

This operation configures notifications that will be sent when specific events
happen to a vault.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/notification/set.html)

```python
# set method definition

await def set(
    self,
    *,
    vaultNotificationConfig: VaultNotificationConfigUnionTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: VaultNotificationConfigTypeDef](./type_defs.md#vaultnotificationconfigtypedef) [:material-code-braces: VaultNotificationConfigOutputTypeDef](./type_defs.md#vaultnotificationconfigoutputtypedef) 


```python
# set method usage example with argument unpacking

kwargs: SetVaultNotificationsInputNotificationSetTypeDef = {  # (1)
    "vaultNotificationConfig": ...,
}

parent.set(**kwargs)
```

1. See [:material-code-braces: SetVaultNotificationsInputNotificationSetTypeDef](./type_defs.md#setvaultnotificationsinputnotificationsettypedef) 

#### Notification.Vault method

Creates a Vault resource.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").Vault` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/notification/Vault.html)

```python
# Vault method definition

await def Vault(
    self,
) -> _Vault:
    ...
```


#### Notification.load method



Type annotations and code completion for `#!python aiobotocore.resource("glacier").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/notification/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Notification.reload method



Type annotations and code completion for `#!python aiobotocore.resource("glacier").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/notification/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## Vault

Type annotations and code completion for `#!python session.resource("glacier").Vault` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/index.html#Glacier.Vault)

```python
# Vault usage example

from types_aiobotocore_glacier.service_resource import Vault

def get_resource() -> Vault:
    return session.resource("glacier").Vault(...)
```


### Vault attributes


- `account_id`: `str`
- `name`: `str`
- `completed_jobs`: `VaultCompletedJobsCollection`
- `failed_jobs`: `VaultFailedJobsCollection`
- `jobs`: `VaultJobsCollection`
- `jobs_in_progress`: `VaultJobsInProgressCollection`
- `multipart_uplaods`: `VaultMultipartUplaodsCollection`
- `multipart_uploads`: `VaultMultipartUploadsCollection`
- `succeeded_jobs`: `VaultSucceededJobsCollection`
- `vault_arn`: `Awaitable`[`str`]
- `vault_name`: `Awaitable`[`str`]
- `creation_date`: `Awaitable`[`str`]
- `last_inventory_date`: `Awaitable`[`str`]
- `number_of_archives`: `Awaitable`[`int`]
- `size_in_bytes`: `Awaitable`[`int`]
- `meta`: `GlacierResourceMeta`



### Vault collections


#### Vault.completed_jobs

Provides access to [Job](#job) resource.

Type annotations and code completion for `#!python session.resource("glacier").Vault(...).completed_jobs` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/completed_jobs.html#Glacier.Vault.completed_jobs)

```python
# VaultCompletedJobsCollection usage example

from types_aiobotocore_glacier.service_resource import VaultCompletedJobsCollection

def get_collection() -> VaultCompletedJobsCollection:
    resource = session.resource("glacier").Vault(...)
    return resource.completed_jobs
```

#### Vault.failed_jobs

Provides access to [Job](#job) resource.

Type annotations and code completion for `#!python session.resource("glacier").Vault(...).failed_jobs` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/failed_jobs.html#Glacier.Vault.failed_jobs)

```python
# VaultFailedJobsCollection usage example

from types_aiobotocore_glacier.service_resource import VaultFailedJobsCollection

def get_collection() -> VaultFailedJobsCollection:
    resource = session.resource("glacier").Vault(...)
    return resource.failed_jobs
```

#### Vault.jobs

Provides access to [Job](#job) resource.

Type annotations and code completion for `#!python session.resource("glacier").Vault(...).jobs` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/jobs.html#Glacier.Vault.jobs)

```python
# VaultJobsCollection usage example

from types_aiobotocore_glacier.service_resource import VaultJobsCollection

def get_collection() -> VaultJobsCollection:
    resource = session.resource("glacier").Vault(...)
    return resource.jobs
```

#### Vault.jobs_in_progress

Provides access to [Job](#job) resource.

Type annotations and code completion for `#!python session.resource("glacier").Vault(...).jobs_in_progress` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/jobs_in_progress.html#Glacier.Vault.jobs_in_progress)

```python
# VaultJobsInProgressCollection usage example

from types_aiobotocore_glacier.service_resource import VaultJobsInProgressCollection

def get_collection() -> VaultJobsInProgressCollection:
    resource = session.resource("glacier").Vault(...)
    return resource.jobs_in_progress
```

#### Vault.multipart_uplaods

Provides access to [MultipartUpload](#multipartupload) resource.

Type annotations and code completion for `#!python session.resource("glacier").Vault(...).multipart_uplaods` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/multipart_uplaods.html#Glacier.Vault.multipart_uplaods)

```python
# VaultMultipartUplaodsCollection usage example

from types_aiobotocore_glacier.service_resource import VaultMultipartUplaodsCollection

def get_collection() -> VaultMultipartUplaodsCollection:
    resource = session.resource("glacier").Vault(...)
    return resource.multipart_uplaods
```

#### Vault.multipart_uploads

Provides access to [MultipartUpload](#multipartupload) resource.

Type annotations and code completion for `#!python session.resource("glacier").Vault(...).multipart_uploads` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/multipart_uploads.html#Glacier.Vault.multipart_uploads)

```python
# VaultMultipartUploadsCollection usage example

from types_aiobotocore_glacier.service_resource import VaultMultipartUploadsCollection

def get_collection() -> VaultMultipartUploadsCollection:
    resource = session.resource("glacier").Vault(...)
    return resource.multipart_uploads
```

#### Vault.succeeded_jobs

Provides access to [Job](#job) resource.

Type annotations and code completion for `#!python session.resource("glacier").Vault(...).succeeded_jobs` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/succeeded_jobs.html#Glacier.Vault.succeeded_jobs)

```python
# VaultSucceededJobsCollection usage example

from types_aiobotocore_glacier.service_resource import VaultSucceededJobsCollection

def get_collection() -> VaultSucceededJobsCollection:
    resource = session.resource("glacier").Vault(...)
    return resource.succeeded_jobs
```




### Vault methods


#### Vault.get\_available\_subresources method

Returns a list of all the available sub-resources for this Vault.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Vault.create method

This operation creates a new vault with the specified name.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").create` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/create.html)

```python
# create method definition

await def create(
    self,
) -> CreateVaultOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateVaultOutputTypeDef](./type_defs.md#createvaultoutputtypedef) 

#### Vault.delete method

This operation deletes a vault.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/delete.html)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Vault.initiate\_inventory\_retrieval method

This operation initiates a job of the specified type, which can be a select, an
archival retrieval, or a vault retrieval.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").initiate_inventory_retrieval` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/initiate_inventory_retrieval.html)

```python
# initiate_inventory_retrieval method definition

await def initiate_inventory_retrieval(
    self,
) -> _Job:
    ...
```


#### Vault.initiate\_multipart\_upload method

This operation initiates a multipart upload.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").initiate_multipart_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/initiate_multipart_upload.html)

```python
# initiate_multipart_upload method definition

await def initiate_multipart_upload(
    self,
    *,
    archiveDescription: str = ...,
    partSize: str = ...,
) -> _MultipartUpload:
    ...
```



```python
# initiate_multipart_upload method usage example with argument unpacking

kwargs: InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef = {  # (1)
    "archiveDescription": ...,
}

parent.initiate_multipart_upload(**kwargs)
```

1. See [:material-code-braces: InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef](./type_defs.md#initiatemultipartuploadinputvaultinitiatemultipartuploadtypedef) 

#### Vault.upload\_archive method

This operation adds an archive to a vault.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").upload_archive` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/upload_archive.html)

```python
# upload_archive method definition

await def upload_archive(
    self,
    *,
    archiveDescription: str = ...,
    checksum: str = ...,
    body: BlobTypeDef = ...,
) -> _Archive:
    ...
```



```python
# upload_archive method usage example with argument unpacking

kwargs: UploadArchiveInputVaultUploadArchiveTypeDef = {  # (1)
    "archiveDescription": ...,
}

parent.upload_archive(**kwargs)
```

1. See [:material-code-braces: UploadArchiveInputVaultUploadArchiveTypeDef](./type_defs.md#uploadarchiveinputvaultuploadarchivetypedef) 

#### Vault.Account method

Creates a Account resource.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").Account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/Account.html)

```python
# Account method definition

await def Account(
    self,
) -> _Account:
    ...
```


#### Vault.Archive method

Creates a Archive resource.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").Archive` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/Archive.html)

```python
# Archive method definition

await def Archive(
    self,
    id: str,
) -> _Archive:
    ...
```


#### Vault.Job method

Creates a Job resource.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").Job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/Job.html)

```python
# Job method definition

await def Job(
    self,
    id: str,
) -> _Job:
    ...
```


#### Vault.MultipartUpload method

Creates a MultipartUpload resource.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").MultipartUpload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/MultipartUpload.html)

```python
# MultipartUpload method definition

await def MultipartUpload(
    self,
    id: str,
) -> _MultipartUpload:
    ...
```


#### Vault.Notification method

Creates a Notification resource.

Type annotations and code completion for `#!python aiobotocore.resource("glacier").Notification` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/Notification.html)

```python
# Notification method definition

await def Notification(
    self,
) -> _Notification:
    ...
```


#### Vault.load method



Type annotations and code completion for `#!python aiobotocore.resource("glacier").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Vault.reload method



Type annotations and code completion for `#!python aiobotocore.resource("glacier").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier/vault/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```




