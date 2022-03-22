<a id="glacierclient-for-aiobotocore-glacier-module"></a>

# GlacierClient for aiobotocore Glacier module

> [Index](../README.md) > [Glacier](./README.md) > GlacierClient

Auto-generated documentation for
[Glacier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
type annotations stubs module
[types-aiobotocore-glacier](https://pypi.org/project/types-aiobotocore-glacier/).

- [GlacierClient for aiobotocore Glacier module](#glacierclient-for-aiobotocore-glacier-module)
  - [GlacierClient](#glacierclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [abort_multipart_upload](#abort_multipart_upload)
    - [abort_vault_lock](#abort_vault_lock)
    - [add_tags_to_vault](#add_tags_to_vault)
    - [can_paginate](#can_paginate)
    - [complete_multipart_upload](#complete_multipart_upload)
    - [complete_vault_lock](#complete_vault_lock)
    - [create_vault](#create_vault)
    - [delete_archive](#delete_archive)
    - [delete_vault](#delete_vault)
    - [delete_vault_access_policy](#delete_vault_access_policy)
    - [delete_vault_notifications](#delete_vault_notifications)
    - [describe_job](#describe_job)
    - [describe_vault](#describe_vault)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_data_retrieval_policy](#get_data_retrieval_policy)
    - [get_job_output](#get_job_output)
    - [get_vault_access_policy](#get_vault_access_policy)
    - [get_vault_lock](#get_vault_lock)
    - [get_vault_notifications](#get_vault_notifications)
    - [initiate_job](#initiate_job)
    - [initiate_multipart_upload](#initiate_multipart_upload)
    - [initiate_vault_lock](#initiate_vault_lock)
    - [list_jobs](#list_jobs)
    - [list_multipart_uploads](#list_multipart_uploads)
    - [list_parts](#list_parts)
    - [list_provisioned_capacity](#list_provisioned_capacity)
    - [list_tags_for_vault](#list_tags_for_vault)
    - [list_vaults](#list_vaults)
    - [purchase_provisioned_capacity](#purchase_provisioned_capacity)
    - [remove_tags_from_vault](#remove_tags_from_vault)
    - [set_data_retrieval_policy](#set_data_retrieval_policy)
    - [set_vault_access_policy](#set_vault_access_policy)
    - [set_vault_notifications](#set_vault_notifications)
    - [upload_archive](#upload_archive)
    - [upload_multipart_part](#upload_multipart_part)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="glacierclient"></a>

## GlacierClient

Type annotations for `session.create_client("glacier")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_glacier.client import GlacierClient

session = get_session()
async with session.create_client("glacier") as client:
    client: GlacierClient
```

Boto3 documentation:
[Glacier.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_glacier.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InsufficientCapacityException`
- `Exceptions.InvalidParameterValueException`
- `Exceptions.LimitExceededException`
- `Exceptions.MissingParameterValueException`
- `Exceptions.PolicyEnforcedException`
- `Exceptions.RequestTimeoutException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceUnavailableException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

GlacierClient exceptions.

Type annotations for `session.create_client("glacier").exceptions` method.

Boto3 documentation:
[Glacier.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="abort\_multipart\_upload"></a>

### abort_multipart_upload

This operation aborts a multipart upload identified by the upload ID.

Type annotations for `session.create_client("glacier").abort_multipart_upload`
method.

Boto3 documentation:
[Glacier.Client.abort_multipart_upload](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.abort_multipart_upload)

Asynchronous method. Use `await abort_multipart_upload(...)` for a synchronous
call.

Arguments mapping described in
[AbortMultipartUploadInputRequestTypeDef](./type_defs.md#abortmultipartuploadinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `uploadId`: `str` *(required)*
- `accountId`: `str`

<a id="abort\_vault\_lock"></a>

### abort_vault_lock

This operation aborts the vault locking process if the vault lock is not in the
`Locked` state.

Type annotations for `session.create_client("glacier").abort_vault_lock`
method.

Boto3 documentation:
[Glacier.Client.abort_vault_lock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.abort_vault_lock)

Asynchronous method. Use `await abort_vault_lock(...)` for a synchronous call.

Arguments mapping described in
[AbortVaultLockInputRequestTypeDef](./type_defs.md#abortvaultlockinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`

<a id="add\_tags\_to\_vault"></a>

### add_tags_to_vault

This operation adds the specified tags to a vault.

Type annotations for `session.create_client("glacier").add_tags_to_vault`
method.

Boto3 documentation:
[Glacier.Client.add_tags_to_vault](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.add_tags_to_vault)

Asynchronous method. Use `await add_tags_to_vault(...)` for a synchronous call.

Arguments mapping described in
[AddTagsToVaultInputRequestTypeDef](./type_defs.md#addtagstovaultinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("glacier").can_paginate` method.

Boto3 documentation:
[Glacier.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="complete\_multipart\_upload"></a>

### complete_multipart_upload

You call this operation to inform Amazon S3 Glacier (Glacier) that all the
archive parts have been uploaded and that Glacier can now assemble the archive
from the uploaded parts.

Type annotations for
`session.create_client("glacier").complete_multipart_upload` method.

Boto3 documentation:
[Glacier.Client.complete_multipart_upload](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.complete_multipart_upload)

Asynchronous method. Use `await complete_multipart_upload(...)` for a
synchronous call.

Arguments mapping described in
[CompleteMultipartUploadInputRequestTypeDef](./type_defs.md#completemultipartuploadinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `uploadId`: `str` *(required)*
- `accountId`: `str`
- `archiveSize`: `str`
- `checksum`: `str`

Returns a `Coroutine` for
[ArchiveCreationOutputTypeDef](./type_defs.md#archivecreationoutputtypedef).

<a id="complete\_vault\_lock"></a>

### complete_vault_lock

This operation completes the vault locking process by transitioning the vault
lock from the `InProgress` state to the `Locked` state, which causes the vault
lock policy to become unchangeable.

Type annotations for `session.create_client("glacier").complete_vault_lock`
method.

Boto3 documentation:
[Glacier.Client.complete_vault_lock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.complete_vault_lock)

Asynchronous method. Use `await complete_vault_lock(...)` for a synchronous
call.

Arguments mapping described in
[CompleteVaultLockInputRequestTypeDef](./type_defs.md#completevaultlockinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `lockId`: `str` *(required)*
- `accountId`: `str`

<a id="create\_vault"></a>

### create_vault

This operation creates a new vault with the specified name.

Type annotations for `session.create_client("glacier").create_vault` method.

Boto3 documentation:
[Glacier.Client.create_vault](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.create_vault)

Asynchronous method. Use `await create_vault(...)` for a synchronous call.

Arguments mapping described in
[CreateVaultInputRequestTypeDef](./type_defs.md#createvaultinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`

Returns a `Coroutine` for
[CreateVaultOutputTypeDef](./type_defs.md#createvaultoutputtypedef).

<a id="delete\_archive"></a>

### delete_archive

This operation deletes an archive from a vault.

Type annotations for `session.create_client("glacier").delete_archive` method.

Boto3 documentation:
[Glacier.Client.delete_archive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.delete_archive)

Asynchronous method. Use `await delete_archive(...)` for a synchronous call.

Arguments mapping described in
[DeleteArchiveInputRequestTypeDef](./type_defs.md#deletearchiveinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `archiveId`: `str` *(required)*
- `accountId`: `str`

<a id="delete\_vault"></a>

### delete_vault

This operation deletes a vault.

Type annotations for `session.create_client("glacier").delete_vault` method.

Boto3 documentation:
[Glacier.Client.delete_vault](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.delete_vault)

Asynchronous method. Use `await delete_vault(...)` for a synchronous call.

Arguments mapping described in
[DeleteVaultInputRequestTypeDef](./type_defs.md#deletevaultinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`

<a id="delete\_vault\_access\_policy"></a>

### delete_vault_access_policy

This operation deletes the access policy associated with the specified vault.

Type annotations for
`session.create_client("glacier").delete_vault_access_policy` method.

Boto3 documentation:
[Glacier.Client.delete_vault_access_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.delete_vault_access_policy)

Asynchronous method. Use `await delete_vault_access_policy(...)` for a
synchronous call.

Arguments mapping described in
[DeleteVaultAccessPolicyInputRequestTypeDef](./type_defs.md#deletevaultaccesspolicyinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`

<a id="delete\_vault\_notifications"></a>

### delete_vault_notifications

This operation deletes the notification configuration set for a vault.

Type annotations for
`session.create_client("glacier").delete_vault_notifications` method.

Boto3 documentation:
[Glacier.Client.delete_vault_notifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.delete_vault_notifications)

Asynchronous method. Use `await delete_vault_notifications(...)` for a
synchronous call.

Arguments mapping described in
[DeleteVaultNotificationsInputRequestTypeDef](./type_defs.md#deletevaultnotificationsinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`

<a id="describe\_job"></a>

### describe_job

This operation returns information about a job you previously initiated,
including the job initiation date, the user who initiated the job, the job
status code/message and the Amazon SNS topic to notify after Amazon S3 Glacier
(Glacier) completes the job.

Type annotations for `session.create_client("glacier").describe_job` method.

Boto3 documentation:
[Glacier.Client.describe_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.describe_job)

Asynchronous method. Use `await describe_job(...)` for a synchronous call.

Arguments mapping described in
[DescribeJobInputRequestTypeDef](./type_defs.md#describejobinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `jobId`: `str` *(required)*
- `accountId`: `str`

Returns a `Coroutine` for
[GlacierJobDescriptionResponseMetadataTypeDef](./type_defs.md#glacierjobdescriptionresponsemetadatatypedef).

<a id="describe\_vault"></a>

### describe_vault

This operation returns information about a vault, including the vault's Amazon
Resource Name (ARN), the date the vault was created, the number of archives it
contains, and the total size of all the archives in the vault.

Type annotations for `session.create_client("glacier").describe_vault` method.

Boto3 documentation:
[Glacier.Client.describe_vault](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.describe_vault)

Asynchronous method. Use `await describe_vault(...)` for a synchronous call.

Arguments mapping described in
[DescribeVaultInputRequestTypeDef](./type_defs.md#describevaultinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`

Returns a `Coroutine` for
[DescribeVaultOutputResponseMetadataTypeDef](./type_defs.md#describevaultoutputresponsemetadatatypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("glacier").generate_presigned_url`
method.

Boto3 documentation:
[Glacier.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_data\_retrieval\_policy"></a>

### get_data_retrieval_policy

This operation returns the current data retrieval policy for the account and
region specified in the GET request.

Type annotations for
`session.create_client("glacier").get_data_retrieval_policy` method.

Boto3 documentation:
[Glacier.Client.get_data_retrieval_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.get_data_retrieval_policy)

Asynchronous method. Use `await get_data_retrieval_policy(...)` for a
synchronous call.

Arguments mapping described in
[GetDataRetrievalPolicyInputRequestTypeDef](./type_defs.md#getdataretrievalpolicyinputrequesttypedef).

Keyword-only arguments:

- `accountId`: `str`

Returns a `Coroutine` for
[GetDataRetrievalPolicyOutputTypeDef](./type_defs.md#getdataretrievalpolicyoutputtypedef).

<a id="get\_job\_output"></a>

### get_job_output

This operation downloads the output of the job you initiated using InitiateJob.

Type annotations for `session.create_client("glacier").get_job_output` method.

Boto3 documentation:
[Glacier.Client.get_job_output](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.get_job_output)

Asynchronous method. Use `await get_job_output(...)` for a synchronous call.

Arguments mapping described in
[GetJobOutputInputRequestTypeDef](./type_defs.md#getjoboutputinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `jobId`: `str` *(required)*
- `accountId`: `str`
- `range`: `str`

Returns a `Coroutine` for
[GetJobOutputOutputTypeDef](./type_defs.md#getjoboutputoutputtypedef).

<a id="get\_vault\_access\_policy"></a>

### get_vault_access_policy

This operation retrieves the `access-policy` subresource set on the vault; for
more information on setting this subresource, see \[Set Vault Access Policy
(PUT access-policy)\](https://docs.aws.amazon.com/amazonglacier/latest/dev/api-
SetVaultAccessPolicy.html)\_.

Type annotations for `session.create_client("glacier").get_vault_access_policy`
method.

Boto3 documentation:
[Glacier.Client.get_vault_access_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.get_vault_access_policy)

Asynchronous method. Use `await get_vault_access_policy(...)` for a synchronous
call.

Arguments mapping described in
[GetVaultAccessPolicyInputRequestTypeDef](./type_defs.md#getvaultaccesspolicyinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`

Returns a `Coroutine` for
[GetVaultAccessPolicyOutputTypeDef](./type_defs.md#getvaultaccesspolicyoutputtypedef).

<a id="get\_vault\_lock"></a>

### get_vault_lock

This operation retrieves the following attributes from the `lock-policy`
subresource set on the specified vault * The vault lock policy set on the
vault.

Type annotations for `session.create_client("glacier").get_vault_lock` method.

Boto3 documentation:
[Glacier.Client.get_vault_lock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.get_vault_lock)

Asynchronous method. Use `await get_vault_lock(...)` for a synchronous call.

Arguments mapping described in
[GetVaultLockInputRequestTypeDef](./type_defs.md#getvaultlockinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`

Returns a `Coroutine` for
[GetVaultLockOutputTypeDef](./type_defs.md#getvaultlockoutputtypedef).

<a id="get\_vault\_notifications"></a>

### get_vault_notifications

This operation retrieves the `notification-configuration` subresource of the
specified vault.

Type annotations for `session.create_client("glacier").get_vault_notifications`
method.

Boto3 documentation:
[Glacier.Client.get_vault_notifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.get_vault_notifications)

Asynchronous method. Use `await get_vault_notifications(...)` for a synchronous
call.

Arguments mapping described in
[GetVaultNotificationsInputRequestTypeDef](./type_defs.md#getvaultnotificationsinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`

Returns a `Coroutine` for
[GetVaultNotificationsOutputTypeDef](./type_defs.md#getvaultnotificationsoutputtypedef).

<a id="initiate\_job"></a>

### initiate_job

This operation initiates a job of the specified type, which can be a select, an
archival retrieval, or a vault retrieval.

Type annotations for `session.create_client("glacier").initiate_job` method.

Boto3 documentation:
[Glacier.Client.initiate_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.initiate_job)

Asynchronous method. Use `await initiate_job(...)` for a synchronous call.

Arguments mapping described in
[InitiateJobInputRequestTypeDef](./type_defs.md#initiatejobinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`
- `jobParameters`: [JobParametersTypeDef](./type_defs.md#jobparameterstypedef)

Returns a `Coroutine` for
[InitiateJobOutputTypeDef](./type_defs.md#initiatejoboutputtypedef).

<a id="initiate\_multipart\_upload"></a>

### initiate_multipart_upload

This operation initiates a multipart upload.

Type annotations for
`session.create_client("glacier").initiate_multipart_upload` method.

Boto3 documentation:
[Glacier.Client.initiate_multipart_upload](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.initiate_multipart_upload)

Asynchronous method. Use `await initiate_multipart_upload(...)` for a
synchronous call.

Arguments mapping described in
[InitiateMultipartUploadInputRequestTypeDef](./type_defs.md#initiatemultipartuploadinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`
- `archiveDescription`: `str`
- `partSize`: `str`

Returns a `Coroutine` for
[InitiateMultipartUploadOutputTypeDef](./type_defs.md#initiatemultipartuploadoutputtypedef).

<a id="initiate\_vault\_lock"></a>

### initiate_vault_lock

This operation initiates the vault locking process by doing the following \*
Installing a vault lock policy on the specified vault.

Type annotations for `session.create_client("glacier").initiate_vault_lock`
method.

Boto3 documentation:
[Glacier.Client.initiate_vault_lock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.initiate_vault_lock)

Asynchronous method. Use `await initiate_vault_lock(...)` for a synchronous
call.

Arguments mapping described in
[InitiateVaultLockInputRequestTypeDef](./type_defs.md#initiatevaultlockinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`
- `policy`: [VaultLockPolicyTypeDef](./type_defs.md#vaultlockpolicytypedef)

Returns a `Coroutine` for
[InitiateVaultLockOutputTypeDef](./type_defs.md#initiatevaultlockoutputtypedef).

<a id="list\_jobs"></a>

### list_jobs

This operation lists jobs for a vault, including jobs that are in-progress and
jobs that have recently finished.

Type annotations for `session.create_client("glacier").list_jobs` method.

Boto3 documentation:
[Glacier.Client.list_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.list_jobs)

Asynchronous method. Use `await list_jobs(...)` for a synchronous call.

Arguments mapping described in
[ListJobsInputRequestTypeDef](./type_defs.md#listjobsinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`
- `limit`: `str`
- `marker`: `str`
- `statuscode`: `str`
- `completed`: `str`

Returns a `Coroutine` for
[ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef).

<a id="list\_multipart\_uploads"></a>

### list_multipart_uploads

This operation lists in-progress multipart uploads for the specified vault.

Type annotations for `session.create_client("glacier").list_multipart_uploads`
method.

Boto3 documentation:
[Glacier.Client.list_multipart_uploads](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.list_multipart_uploads)

Asynchronous method. Use `await list_multipart_uploads(...)` for a synchronous
call.

Arguments mapping described in
[ListMultipartUploadsInputRequestTypeDef](./type_defs.md#listmultipartuploadsinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`
- `marker`: `str`
- `limit`: `str`

Returns a `Coroutine` for
[ListMultipartUploadsOutputTypeDef](./type_defs.md#listmultipartuploadsoutputtypedef).

<a id="list\_parts"></a>

### list_parts

This operation lists the parts of an archive that have been uploaded in a
specific multipart upload.

Type annotations for `session.create_client("glacier").list_parts` method.

Boto3 documentation:
[Glacier.Client.list_parts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.list_parts)

Asynchronous method. Use `await list_parts(...)` for a synchronous call.

Arguments mapping described in
[ListPartsInputRequestTypeDef](./type_defs.md#listpartsinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `uploadId`: `str` *(required)*
- `accountId`: `str`
- `marker`: `str`
- `limit`: `str`

Returns a `Coroutine` for
[ListPartsOutputTypeDef](./type_defs.md#listpartsoutputtypedef).

<a id="list\_provisioned\_capacity"></a>

### list_provisioned_capacity

This operation lists the provisioned capacity units for the specified AWS
account.

Type annotations for
`session.create_client("glacier").list_provisioned_capacity` method.

Boto3 documentation:
[Glacier.Client.list_provisioned_capacity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.list_provisioned_capacity)

Asynchronous method. Use `await list_provisioned_capacity(...)` for a
synchronous call.

Arguments mapping described in
[ListProvisionedCapacityInputRequestTypeDef](./type_defs.md#listprovisionedcapacityinputrequesttypedef).

Keyword-only arguments:

- `accountId`: `str`

Returns a `Coroutine` for
[ListProvisionedCapacityOutputTypeDef](./type_defs.md#listprovisionedcapacityoutputtypedef).

<a id="list\_tags\_for\_vault"></a>

### list_tags_for_vault

This operation lists all the tags attached to a vault.

Type annotations for `session.create_client("glacier").list_tags_for_vault`
method.

Boto3 documentation:
[Glacier.Client.list_tags_for_vault](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.list_tags_for_vault)

Asynchronous method. Use `await list_tags_for_vault(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForVaultInputRequestTypeDef](./type_defs.md#listtagsforvaultinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`

Returns a `Coroutine` for
[ListTagsForVaultOutputTypeDef](./type_defs.md#listtagsforvaultoutputtypedef).

<a id="list\_vaults"></a>

### list_vaults

This operation lists all vaults owned by the calling user's account.

Type annotations for `session.create_client("glacier").list_vaults` method.

Boto3 documentation:
[Glacier.Client.list_vaults](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.list_vaults)

Asynchronous method. Use `await list_vaults(...)` for a synchronous call.

Arguments mapping described in
[ListVaultsInputRequestTypeDef](./type_defs.md#listvaultsinputrequesttypedef).

Keyword-only arguments:

- `accountId`: `str`
- `marker`: `str`
- `limit`: `str`

Returns a `Coroutine` for
[ListVaultsOutputTypeDef](./type_defs.md#listvaultsoutputtypedef).

<a id="purchase\_provisioned\_capacity"></a>

### purchase_provisioned_capacity

This operation purchases a provisioned capacity unit for an AWS account.

Type annotations for
`session.create_client("glacier").purchase_provisioned_capacity` method.

Boto3 documentation:
[Glacier.Client.purchase_provisioned_capacity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.purchase_provisioned_capacity)

Asynchronous method. Use `await purchase_provisioned_capacity(...)` for a
synchronous call.

Arguments mapping described in
[PurchaseProvisionedCapacityInputRequestTypeDef](./type_defs.md#purchaseprovisionedcapacityinputrequesttypedef).

Keyword-only arguments:

- `accountId`: `str`

Returns a `Coroutine` for
[PurchaseProvisionedCapacityOutputTypeDef](./type_defs.md#purchaseprovisionedcapacityoutputtypedef).

<a id="remove\_tags\_from\_vault"></a>

### remove_tags_from_vault

This operation removes one or more tags from the set of tags attached to a
vault.

Type annotations for `session.create_client("glacier").remove_tags_from_vault`
method.

Boto3 documentation:
[Glacier.Client.remove_tags_from_vault](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.remove_tags_from_vault)

Asynchronous method. Use `await remove_tags_from_vault(...)` for a synchronous
call.

Arguments mapping described in
[RemoveTagsFromVaultInputRequestTypeDef](./type_defs.md#removetagsfromvaultinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`
- `TagKeys`: `Sequence`\[`str`\]

<a id="set\_data\_retrieval\_policy"></a>

### set_data_retrieval_policy

This operation sets and then enacts a data retrieval policy in the region
specified in the PUT request.

Type annotations for
`session.create_client("glacier").set_data_retrieval_policy` method.

Boto3 documentation:
[Glacier.Client.set_data_retrieval_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_data_retrieval_policy)

Asynchronous method. Use `await set_data_retrieval_policy(...)` for a
synchronous call.

Arguments mapping described in
[SetDataRetrievalPolicyInputRequestTypeDef](./type_defs.md#setdataretrievalpolicyinputrequesttypedef).

Keyword-only arguments:

- `accountId`: `str`
- `Policy`:
  [DataRetrievalPolicyTypeDef](./type_defs.md#dataretrievalpolicytypedef)

<a id="set\_vault\_access\_policy"></a>

### set_vault_access_policy

This operation configures an access policy for a vault and will overwrite an
existing policy.

Type annotations for `session.create_client("glacier").set_vault_access_policy`
method.

Boto3 documentation:
[Glacier.Client.set_vault_access_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_vault_access_policy)

Asynchronous method. Use `await set_vault_access_policy(...)` for a synchronous
call.

Arguments mapping described in
[SetVaultAccessPolicyInputRequestTypeDef](./type_defs.md#setvaultaccesspolicyinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`
- `policy`: [VaultAccessPolicyTypeDef](./type_defs.md#vaultaccesspolicytypedef)

<a id="set\_vault\_notifications"></a>

### set_vault_notifications

This operation configures notifications that will be sent when specific events
happen to a vault.

Type annotations for `session.create_client("glacier").set_vault_notifications`
method.

Boto3 documentation:
[Glacier.Client.set_vault_notifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_vault_notifications)

Asynchronous method. Use `await set_vault_notifications(...)` for a synchronous
call.

Arguments mapping described in
[SetVaultNotificationsInputRequestTypeDef](./type_defs.md#setvaultnotificationsinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`
- `vaultNotificationConfig`:
  [VaultNotificationConfigTypeDef](./type_defs.md#vaultnotificationconfigtypedef)

<a id="upload\_archive"></a>

### upload_archive

This operation adds an archive to a vault.

Type annotations for `session.create_client("glacier").upload_archive` method.

Boto3 documentation:
[Glacier.Client.upload_archive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.upload_archive)

Asynchronous method. Use `await upload_archive(...)` for a synchronous call.

Arguments mapping described in
[UploadArchiveInputRequestTypeDef](./type_defs.md#uploadarchiveinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `accountId`: `str`
- `archiveDescription`: `str`
- `checksum`: `str`
- `body`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]

Returns a `Coroutine` for
[ArchiveCreationOutputTypeDef](./type_defs.md#archivecreationoutputtypedef).

<a id="upload\_multipart\_part"></a>

### upload_multipart_part

This operation uploads a part of an archive.

Type annotations for `session.create_client("glacier").upload_multipart_part`
method.

Boto3 documentation:
[Glacier.Client.upload_multipart_part](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.upload_multipart_part)

Asynchronous method. Use `await upload_multipart_part(...)` for a synchronous
call.

Arguments mapping described in
[UploadMultipartPartInputRequestTypeDef](./type_defs.md#uploadmultipartpartinputrequesttypedef).

Keyword-only arguments:

- `vaultName`: `str` *(required)*
- `uploadId`: `str` *(required)*
- `accountId`: `str`
- `checksum`: `str`
- `range`: `str`
- `body`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]

Returns a `Coroutine` for
[UploadMultipartPartOutputTypeDef](./type_defs.md#uploadmultipartpartoutputtypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("glacier").__aenter__` method.

Boto3 documentation:
[Glacier.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [GlacierClient](#glacierclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("glacier").__aexit__` method.

Boto3 documentation:
[Glacier.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("glacier").get_paginator` method
with overloads.

- `client.get_paginator("list_jobs")` ->
  [ListJobsPaginator](./paginators.md#listjobspaginator)
- `client.get_paginator("list_multipart_uploads")` ->
  [ListMultipartUploadsPaginator](./paginators.md#listmultipartuploadspaginator)
- `client.get_paginator("list_parts")` ->
  [ListPartsPaginator](./paginators.md#listpartspaginator)
- `client.get_paginator("list_vaults")` ->
  [ListVaultsPaginator](./paginators.md#listvaultspaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("glacier").get_waiter` method with
overloads.

- `client.get_waiter("vault_exists")` ->
  [VaultExistsWaiter](./waiters.md#vaultexistswaiter)
- `client.get_waiter("vault_not_exists")` ->
  [VaultNotExistsWaiter](./waiters.md#vaultnotexistswaiter)
