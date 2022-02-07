<a id="cloudhsmv2client-for-aiobotocore-cloudhsmv2-module"></a>

# CloudHSMV2Client for aiobotocore CloudHSMV2 module

> [Index](..) > [CloudHSMV2](.) > CloudHSMV2Client

Auto-generated documentation for
[CloudHSMV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
type annotations stubs module
[types-aiobotocore-cloudhsmv2](https://pypi.org/project/types-aiobotocore-cloudhsmv2/).

- [CloudHSMV2Client for aiobotocore CloudHSMV2 module](#cloudhsmv2client-for-aiobotocore-cloudhsmv2-module)
  - [CloudHSMV2Client](#cloudhsmv2client)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [copy_backup_to_region](#copy_backup_to_region)
    - [create_cluster](#create_cluster)
    - [create_hsm](#create_hsm)
    - [delete_backup](#delete_backup)
    - [delete_cluster](#delete_cluster)
    - [delete_hsm](#delete_hsm)
    - [describe_backups](#describe_backups)
    - [describe_clusters](#describe_clusters)
    - [generate_presigned_url](#generate_presigned_url)
    - [initialize_cluster](#initialize_cluster)
    - [list_tags](#list_tags)
    - [modify_backup_attributes](#modify_backup_attributes)
    - [modify_cluster](#modify_cluster)
    - [restore_backup](#restore_backup)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="cloudhsmv2client"></a>

## CloudHSMV2Client

Type annotations for `session.create_client("cloudhsmv2")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_cloudhsmv2.client import CloudHSMV2Client

session = get_session()
async with session.create_client("cloudhsmv2") as client:
    client: CloudHSMV2Client
```

Boto3 documentation:
[CloudHSMV2.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_cloudhsmv2.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.CloudHsmAccessDeniedException`
- `Exceptions.CloudHsmInternalFailureException`
- `Exceptions.CloudHsmInvalidRequestException`
- `Exceptions.CloudHsmResourceNotFoundException`
- `Exceptions.CloudHsmServiceException`
- `Exceptions.CloudHsmTagException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

CloudHSMV2Client exceptions.

Type annotations for `session.create_client("cloudhsmv2").exceptions` method.

Boto3 documentation:
[CloudHSMV2.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("cloudhsmv2").can_paginate` method.

Boto3 documentation:
[CloudHSMV2.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="copy_backup_to_region"></a>

### copy_backup_to_region

Copy an AWS CloudHSM cluster backup to a different region.

Type annotations for
`session.create_client("cloudhsmv2").copy_backup_to_region` method.

Boto3 documentation:
[CloudHSMV2.Client.copy_backup_to_region](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.copy_backup_to_region)

Asynchronous method. Use `await copy_backup_to_region(...)` for a synchronous
call.

Arguments mapping described in
[CopyBackupToRegionRequestRequestTypeDef](./type_defs.md#copybackuptoregionrequestrequesttypedef).

Keyword-only arguments:

- `DestinationRegion`: `str` *(required)*
- `BackupId`: `str` *(required)*
- `TagList`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CopyBackupToRegionResponseTypeDef](./type_defs.md#copybackuptoregionresponsetypedef).

<a id="create_cluster"></a>

### create_cluster

Creates a new AWS CloudHSM cluster.

Type annotations for `session.create_client("cloudhsmv2").create_cluster`
method.

Boto3 documentation:
[CloudHSMV2.Client.create_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.create_cluster)

Asynchronous method. Use `await create_cluster(...)` for a synchronous call.

Arguments mapping described in
[CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef).

Keyword-only arguments:

- `HsmType`: `str` *(required)*
- `SubnetIds`: `Sequence`\[`str`\] *(required)*
- `BackupRetentionPolicy`:
  [BackupRetentionPolicyTypeDef](./type_defs.md#backupretentionpolicytypedef)
- `SourceBackupId`: `str`
- `TagList`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef).

<a id="create_hsm"></a>

### create_hsm

Creates a new hardware security module (HSM) in the specified AWS CloudHSM
cluster.

Type annotations for `session.create_client("cloudhsmv2").create_hsm` method.

Boto3 documentation:
[CloudHSMV2.Client.create_hsm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.create_hsm)

Asynchronous method. Use `await create_hsm(...)` for a synchronous call.

Arguments mapping described in
[CreateHsmRequestRequestTypeDef](./type_defs.md#createhsmrequestrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `AvailabilityZone`: `str` *(required)*
- `IpAddress`: `str`

Returns a `Coroutine` for
[CreateHsmResponseTypeDef](./type_defs.md#createhsmresponsetypedef).

<a id="delete_backup"></a>

### delete_backup

Deletes a specified AWS CloudHSM backup.

Type annotations for `session.create_client("cloudhsmv2").delete_backup`
method.

Boto3 documentation:
[CloudHSMV2.Client.delete_backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.delete_backup)

Asynchronous method. Use `await delete_backup(...)` for a synchronous call.

Arguments mapping described in
[DeleteBackupRequestRequestTypeDef](./type_defs.md#deletebackuprequestrequesttypedef).

Keyword-only arguments:

- `BackupId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteBackupResponseTypeDef](./type_defs.md#deletebackupresponsetypedef).

<a id="delete_cluster"></a>

### delete_cluster

Deletes the specified AWS CloudHSM cluster.

Type annotations for `session.create_client("cloudhsmv2").delete_cluster`
method.

Boto3 documentation:
[CloudHSMV2.Client.delete_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.delete_cluster)

Asynchronous method. Use `await delete_cluster(...)` for a synchronous call.

Arguments mapping described in
[DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteClusterResponseTypeDef](./type_defs.md#deleteclusterresponsetypedef).

<a id="delete_hsm"></a>

### delete_hsm

Deletes the specified HSM.

Type annotations for `session.create_client("cloudhsmv2").delete_hsm` method.

Boto3 documentation:
[CloudHSMV2.Client.delete_hsm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.delete_hsm)

Asynchronous method. Use `await delete_hsm(...)` for a synchronous call.

Arguments mapping described in
[DeleteHsmRequestRequestTypeDef](./type_defs.md#deletehsmrequestrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `HsmId`: `str`
- `EniId`: `str`
- `EniIp`: `str`

Returns a `Coroutine` for
[DeleteHsmResponseTypeDef](./type_defs.md#deletehsmresponsetypedef).

<a id="describe_backups"></a>

### describe_backups

Gets information about backups of AWS CloudHSM clusters.

Type annotations for `session.create_client("cloudhsmv2").describe_backups`
method.

Boto3 documentation:
[CloudHSMV2.Client.describe_backups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.describe_backups)

Asynchronous method. Use `await describe_backups(...)` for a synchronous call.

Arguments mapping described in
[DescribeBackupsRequestRequestTypeDef](./type_defs.md#describebackupsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `Filters`: `Mapping`\[`str`, `Sequence`\[`str`\]\]
- `SortAscending`: `bool`

Returns a `Coroutine` for
[DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef).

<a id="describe_clusters"></a>

### describe_clusters

Gets information about AWS CloudHSM clusters.

Type annotations for `session.create_client("cloudhsmv2").describe_clusters`
method.

Boto3 documentation:
[CloudHSMV2.Client.describe_clusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.describe_clusters)

Asynchronous method. Use `await describe_clusters(...)` for a synchronous call.

Arguments mapping described in
[DescribeClustersRequestRequestTypeDef](./type_defs.md#describeclustersrequestrequesttypedef).

Keyword-only arguments:

- `Filters`: `Mapping`\[`str`, `Sequence`\[`str`\]\]
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("cloudhsmv2").generate_presigned_url` method.

Boto3 documentation:
[CloudHSMV2.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="initialize_cluster"></a>

### initialize_cluster

Claims an AWS CloudHSM cluster by submitting the cluster certificate issued by
your issuing certificate authority (CA) and the CA's root certificate.

Type annotations for `session.create_client("cloudhsmv2").initialize_cluster`
method.

Boto3 documentation:
[CloudHSMV2.Client.initialize_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.initialize_cluster)

Asynchronous method. Use `await initialize_cluster(...)` for a synchronous
call.

Arguments mapping described in
[InitializeClusterRequestRequestTypeDef](./type_defs.md#initializeclusterrequestrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `SignedCert`: `str` *(required)*
- `TrustAnchor`: `str` *(required)*

Returns a `Coroutine` for
[InitializeClusterResponseTypeDef](./type_defs.md#initializeclusterresponsetypedef).

<a id="list_tags"></a>

### list_tags

Gets a list of tags for the specified AWS CloudHSM cluster.

Type annotations for `session.create_client("cloudhsmv2").list_tags` method.

Boto3 documentation:
[CloudHSMV2.Client.list_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.list_tags)

Asynchronous method. Use `await list_tags(...)` for a synchronous call.

Arguments mapping described in
[ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef).

Keyword-only arguments:

- `ResourceId`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef).

<a id="modify_backup_attributes"></a>

### modify_backup_attributes

Modifies attributes for AWS CloudHSM backup.

Type annotations for
`session.create_client("cloudhsmv2").modify_backup_attributes` method.

Boto3 documentation:
[CloudHSMV2.Client.modify_backup_attributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.modify_backup_attributes)

Asynchronous method. Use `await modify_backup_attributes(...)` for a
synchronous call.

Arguments mapping described in
[ModifyBackupAttributesRequestRequestTypeDef](./type_defs.md#modifybackupattributesrequestrequesttypedef).

Keyword-only arguments:

- `BackupId`: `str` *(required)*
- `NeverExpires`: `bool` *(required)*

Returns a `Coroutine` for
[ModifyBackupAttributesResponseTypeDef](./type_defs.md#modifybackupattributesresponsetypedef).

<a id="modify_cluster"></a>

### modify_cluster

Modifies AWS CloudHSM cluster.

Type annotations for `session.create_client("cloudhsmv2").modify_cluster`
method.

Boto3 documentation:
[CloudHSMV2.Client.modify_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.modify_cluster)

Asynchronous method. Use `await modify_cluster(...)` for a synchronous call.

Arguments mapping described in
[ModifyClusterRequestRequestTypeDef](./type_defs.md#modifyclusterrequestrequesttypedef).

Keyword-only arguments:

- `BackupRetentionPolicy`:
  [BackupRetentionPolicyTypeDef](./type_defs.md#backupretentionpolicytypedef)
  *(required)*
- `ClusterId`: `str` *(required)*

Returns a `Coroutine` for
[ModifyClusterResponseTypeDef](./type_defs.md#modifyclusterresponsetypedef).

<a id="restore_backup"></a>

### restore_backup

Restores a specified AWS CloudHSM backup that is in the `PENDING_DELETION`
state.

Type annotations for `session.create_client("cloudhsmv2").restore_backup`
method.

Boto3 documentation:
[CloudHSMV2.Client.restore_backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.restore_backup)

Asynchronous method. Use `await restore_backup(...)` for a synchronous call.

Arguments mapping described in
[RestoreBackupRequestRequestTypeDef](./type_defs.md#restorebackuprequestrequesttypedef).

Keyword-only arguments:

- `BackupId`: `str` *(required)*

Returns a `Coroutine` for
[RestoreBackupResponseTypeDef](./type_defs.md#restorebackupresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Adds or overwrites one or more tags for the specified AWS CloudHSM cluster.

Type annotations for `session.create_client("cloudhsmv2").tag_resource` method.

Boto3 documentation:
[CloudHSMV2.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceId`: `str` *(required)*
- `TagList`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes the specified tag or tags from the specified AWS CloudHSM cluster.

Type annotations for `session.create_client("cloudhsmv2").untag_resource`
method.

Boto3 documentation:
[CloudHSMV2.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceId`: `str` *(required)*
- `TagKeyList`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("cloudhsmv2").__aenter__` method.

Boto3 documentation:
[CloudHSMV2.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [CloudHSMV2Client](#cloudhsmv2client).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("cloudhsmv2").__aexit__` method.

Boto3 documentation:
[CloudHSMV2.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("cloudhsmv2").get_paginator` method
with overloads.

- `client.get_paginator("describe_backups")` ->
  [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
- `client.get_paginator("describe_clusters")` ->
  [DescribeClustersPaginator](./paginators.md#describeclusterspaginator)
- `client.get_paginator("list_tags")` ->
  [ListTagsPaginator](./paginators.md#listtagspaginator)
