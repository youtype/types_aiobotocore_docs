<a id="opsworkscmclient-for-aiobotocore-opsworkscm-module"></a>

# OpsWorksCMClient for aiobotocore OpsWorksCM module

> [Index](..) > [OpsWorksCM](.) > OpsWorksCMClient

Auto-generated documentation for
[OpsWorksCM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
type annotations stubs module
[types-aiobotocore-opsworkscm](https://pypi.org/project/types-aiobotocore-opsworkscm/).

- [OpsWorksCMClient for aiobotocore OpsWorksCM module](#opsworkscmclient-for-aiobotocore-opsworkscm-module)
  - [OpsWorksCMClient](#opsworkscmclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [associate_node](#associate_node)
    - [can_paginate](#can_paginate)
    - [create_backup](#create_backup)
    - [create_server](#create_server)
    - [delete_backup](#delete_backup)
    - [delete_server](#delete_server)
    - [describe_account_attributes](#describe_account_attributes)
    - [describe_backups](#describe_backups)
    - [describe_events](#describe_events)
    - [describe_node_association_status](#describe_node_association_status)
    - [describe_servers](#describe_servers)
    - [disassociate_node](#disassociate_node)
    - [export_server_engine_attribute](#export_server_engine_attribute)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [restore_server](#restore_server)
    - [start_maintenance](#start_maintenance)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_server](#update_server)
    - [update_server_engine_attributes](#update_server_engine_attributes)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="opsworkscmclient"></a>

## OpsWorksCMClient

Type annotations for `session.create_client("opsworkscm")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_opsworkscm.client import OpsWorksCMClient

session = get_session()
async with session.create_client("opsworkscm") as client:
    client: OpsWorksCMClient
```

Boto3 documentation:
[OpsWorksCM.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_opsworkscm.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InvalidNextTokenException`
- `Exceptions.InvalidStateException`
- `Exceptions.LimitExceededException`
- `Exceptions.ResourceAlreadyExistsException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

OpsWorksCMClient exceptions.

Type annotations for `session.create_client("opsworkscm").exceptions` method.

Boto3 documentation:
[OpsWorksCM.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="associate_node"></a>

### associate_node

Associates a new node with the server.

Type annotations for `session.create_client("opsworkscm").associate_node`
method.

Boto3 documentation:
[OpsWorksCM.Client.associate_node](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.associate_node)

Asynchronous method. Use `await associate_node(...)` for a synchronous call.

Arguments mapping described in
[AssociateNodeRequestRequestTypeDef](./type_defs.md#associatenoderequestrequesttypedef).

Keyword-only arguments:

- `ServerName`: `str` *(required)*
- `NodeName`: `str` *(required)*
- `EngineAttributes`:
  `Sequence`\[[EngineAttributeTypeDef](./type_defs.md#engineattributetypedef)\]
  *(required)*

Returns a `Coroutine` for
[AssociateNodeResponseTypeDef](./type_defs.md#associatenoderesponsetypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("opsworkscm").can_paginate` method.

Boto3 documentation:
[OpsWorksCM.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_backup"></a>

### create_backup

Creates an application-level backup of a server.

Type annotations for `session.create_client("opsworkscm").create_backup`
method.

Boto3 documentation:
[OpsWorksCM.Client.create_backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.create_backup)

Asynchronous method. Use `await create_backup(...)` for a synchronous call.

Arguments mapping described in
[CreateBackupRequestRequestTypeDef](./type_defs.md#createbackuprequestrequesttypedef).

Keyword-only arguments:

- `ServerName`: `str` *(required)*
- `Description`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateBackupResponseTypeDef](./type_defs.md#createbackupresponsetypedef).

<a id="create_server"></a>

### create_server

Creates and immedately starts a new server.

Type annotations for `session.create_client("opsworkscm").create_server`
method.

Boto3 documentation:
[OpsWorksCM.Client.create_server](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.create_server)

Asynchronous method. Use `await create_server(...)` for a synchronous call.

Arguments mapping described in
[CreateServerRequestRequestTypeDef](./type_defs.md#createserverrequestrequesttypedef).

Keyword-only arguments:

- `Engine`: `str` *(required)*
- `ServerName`: `str` *(required)*
- `InstanceProfileArn`: `str` *(required)*
- `InstanceType`: `str` *(required)*
- `ServiceRoleArn`: `str` *(required)*
- `AssociatePublicIpAddress`: `bool`
- `CustomDomain`: `str`
- `CustomCertificate`: `str`
- `CustomPrivateKey`: `str`
- `DisableAutomatedBackup`: `bool`
- `EngineModel`: `str`
- `EngineVersion`: `str`
- `EngineAttributes`:
  `Sequence`\[[EngineAttributeTypeDef](./type_defs.md#engineattributetypedef)\]
- `BackupRetentionCount`: `int`
- `KeyPair`: `str`
- `PreferredMaintenanceWindow`: `str`
- `PreferredBackupWindow`: `str`
- `SecurityGroupIds`: `Sequence`\[`str`\]
- `SubnetIds`: `Sequence`\[`str`\]
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `BackupId`: `str`

Returns a `Coroutine` for
[CreateServerResponseTypeDef](./type_defs.md#createserverresponsetypedef).

<a id="delete_backup"></a>

### delete_backup

Deletes a backup.

Type annotations for `session.create_client("opsworkscm").delete_backup`
method.

Boto3 documentation:
[OpsWorksCM.Client.delete_backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.delete_backup)

Asynchronous method. Use `await delete_backup(...)` for a synchronous call.

Arguments mapping described in
[DeleteBackupRequestRequestTypeDef](./type_defs.md#deletebackuprequestrequesttypedef).

Keyword-only arguments:

- `BackupId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_server"></a>

### delete_server

Deletes the server and the underlying AWS CloudFormation stacks (including the
server's EC2 instance).

Type annotations for `session.create_client("opsworkscm").delete_server`
method.

Boto3 documentation:
[OpsWorksCM.Client.delete_server](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.delete_server)

Asynchronous method. Use `await delete_server(...)` for a synchronous call.

Arguments mapping described in
[DeleteServerRequestRequestTypeDef](./type_defs.md#deleteserverrequestrequesttypedef).

Keyword-only arguments:

- `ServerName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_account_attributes"></a>

### describe_account_attributes

Describes your OpsWorks-CM account attributes.

Type annotations for
`session.create_client("opsworkscm").describe_account_attributes` method.

Boto3 documentation:
[OpsWorksCM.Client.describe_account_attributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.describe_account_attributes)

Asynchronous method. Use `await describe_account_attributes(...)` for a
synchronous call.

Returns a `Coroutine` for
[DescribeAccountAttributesResponseTypeDef](./type_defs.md#describeaccountattributesresponsetypedef).

<a id="describe_backups"></a>

### describe_backups

Describes backups.

Type annotations for `session.create_client("opsworkscm").describe_backups`
method.

Boto3 documentation:
[OpsWorksCM.Client.describe_backups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.describe_backups)

Asynchronous method. Use `await describe_backups(...)` for a synchronous call.

Arguments mapping described in
[DescribeBackupsRequestRequestTypeDef](./type_defs.md#describebackupsrequestrequesttypedef).

Keyword-only arguments:

- `BackupId`: `str`
- `ServerName`: `str`
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef).

<a id="describe_events"></a>

### describe_events

Describes events for a specified server.

Type annotations for `session.create_client("opsworkscm").describe_events`
method.

Boto3 documentation:
[OpsWorksCM.Client.describe_events](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.describe_events)

Asynchronous method. Use `await describe_events(...)` for a synchronous call.

Arguments mapping described in
[DescribeEventsRequestRequestTypeDef](./type_defs.md#describeeventsrequestrequesttypedef).

Keyword-only arguments:

- `ServerName`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef).

<a id="describe_node_association_status"></a>

### describe_node_association_status

Returns the current status of an existing association or disassociation
request.

Type annotations for
`session.create_client("opsworkscm").describe_node_association_status` method.

Boto3 documentation:
[OpsWorksCM.Client.describe_node_association_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.describe_node_association_status)

Asynchronous method. Use `await describe_node_association_status(...)` for a
synchronous call.

Arguments mapping described in
[DescribeNodeAssociationStatusRequestRequestTypeDef](./type_defs.md#describenodeassociationstatusrequestrequesttypedef).

Keyword-only arguments:

- `NodeAssociationStatusToken`: `str` *(required)*
- `ServerName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeNodeAssociationStatusResponseTypeDef](./type_defs.md#describenodeassociationstatusresponsetypedef).

<a id="describe_servers"></a>

### describe_servers

Lists all configuration management servers that are identified with your
account.

Type annotations for `session.create_client("opsworkscm").describe_servers`
method.

Boto3 documentation:
[OpsWorksCM.Client.describe_servers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.describe_servers)

Asynchronous method. Use `await describe_servers(...)` for a synchronous call.

Arguments mapping described in
[DescribeServersRequestRequestTypeDef](./type_defs.md#describeserversrequestrequesttypedef).

Keyword-only arguments:

- `ServerName`: `str`
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[DescribeServersResponseTypeDef](./type_defs.md#describeserversresponsetypedef).

<a id="disassociate_node"></a>

### disassociate_node

Disassociates a node from an AWS OpsWorks CM server, and removes the node from
the server's managed nodes.

Type annotations for `session.create_client("opsworkscm").disassociate_node`
method.

Boto3 documentation:
[OpsWorksCM.Client.disassociate_node](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.disassociate_node)

Asynchronous method. Use `await disassociate_node(...)` for a synchronous call.

Arguments mapping described in
[DisassociateNodeRequestRequestTypeDef](./type_defs.md#disassociatenoderequestrequesttypedef).

Keyword-only arguments:

- `ServerName`: `str` *(required)*
- `NodeName`: `str` *(required)*
- `EngineAttributes`:
  `Sequence`\[[EngineAttributeTypeDef](./type_defs.md#engineattributetypedef)\]

Returns a `Coroutine` for
[DisassociateNodeResponseTypeDef](./type_defs.md#disassociatenoderesponsetypedef).

<a id="export_server_engine_attribute"></a>

### export_server_engine_attribute

Exports a specified server engine attribute as a base64-encoded string.

Type annotations for
`session.create_client("opsworkscm").export_server_engine_attribute` method.

Boto3 documentation:
[OpsWorksCM.Client.export_server_engine_attribute](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.export_server_engine_attribute)

Asynchronous method. Use `await export_server_engine_attribute(...)` for a
synchronous call.

Arguments mapping described in
[ExportServerEngineAttributeRequestRequestTypeDef](./type_defs.md#exportserverengineattributerequestrequesttypedef).

Keyword-only arguments:

- `ExportAttributeName`: `str` *(required)*
- `ServerName`: `str` *(required)*
- `InputAttributes`:
  `Sequence`\[[EngineAttributeTypeDef](./type_defs.md#engineattributetypedef)\]

Returns a `Coroutine` for
[ExportServerEngineAttributeResponseTypeDef](./type_defs.md#exportserverengineattributeresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("opsworkscm").generate_presigned_url` method.

Boto3 documentation:
[OpsWorksCM.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.generate_presigned_url)

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

Returns a list of tags that are applied to the specified AWS OpsWorks for Chef
Automate or AWS OpsWorks for Puppet Enterprise servers or backups.

Type annotations for
`session.create_client("opsworkscm").list_tags_for_resource` method.

Boto3 documentation:
[OpsWorksCM.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="restore_server"></a>

### restore_server

Restores a backup to a server that is in a `CONNECTION_LOST` , `HEALTHY` ,
`RUNNING` , `UNHEALTHY` , or `TERMINATED` state.

Type annotations for `session.create_client("opsworkscm").restore_server`
method.

Boto3 documentation:
[OpsWorksCM.Client.restore_server](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.restore_server)

Asynchronous method. Use `await restore_server(...)` for a synchronous call.

Arguments mapping described in
[RestoreServerRequestRequestTypeDef](./type_defs.md#restoreserverrequestrequesttypedef).

Keyword-only arguments:

- `BackupId`: `str` *(required)*
- `ServerName`: `str` *(required)*
- `InstanceType`: `str`
- `KeyPair`: `str`

Returns a `Coroutine` for
[RestoreServerResponseTypeDef](./type_defs.md#restoreserverresponsetypedef).

<a id="start_maintenance"></a>

### start_maintenance

Manually starts server maintenance.

Type annotations for `session.create_client("opsworkscm").start_maintenance`
method.

Boto3 documentation:
[OpsWorksCM.Client.start_maintenance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.start_maintenance)

Asynchronous method. Use `await start_maintenance(...)` for a synchronous call.

Arguments mapping described in
[StartMaintenanceRequestRequestTypeDef](./type_defs.md#startmaintenancerequestrequesttypedef).

Keyword-only arguments:

- `ServerName`: `str` *(required)*
- `EngineAttributes`:
  `Sequence`\[[EngineAttributeTypeDef](./type_defs.md#engineattributetypedef)\]

Returns a `Coroutine` for
[StartMaintenanceResponseTypeDef](./type_defs.md#startmaintenanceresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Applies tags to an AWS OpsWorks for Chef Automate or AWS OpsWorks for Puppet
Enterprise server, or to server backups.

Type annotations for `session.create_client("opsworkscm").tag_resource` method.

Boto3 documentation:
[OpsWorksCM.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes specified tags from an AWS OpsWorks-CM server or backup.

Type annotations for `session.create_client("opsworkscm").untag_resource`
method.

Boto3 documentation:
[OpsWorksCM.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_server"></a>

### update_server

Updates settings for a server.

Type annotations for `session.create_client("opsworkscm").update_server`
method.

Boto3 documentation:
[OpsWorksCM.Client.update_server](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.update_server)

Asynchronous method. Use `await update_server(...)` for a synchronous call.

Arguments mapping described in
[UpdateServerRequestRequestTypeDef](./type_defs.md#updateserverrequestrequesttypedef).

Keyword-only arguments:

- `ServerName`: `str` *(required)*
- `DisableAutomatedBackup`: `bool`
- `BackupRetentionCount`: `int`
- `PreferredMaintenanceWindow`: `str`
- `PreferredBackupWindow`: `str`

Returns a `Coroutine` for
[UpdateServerResponseTypeDef](./type_defs.md#updateserverresponsetypedef).

<a id="update_server_engine_attributes"></a>

### update_server_engine_attributes

Updates engine-specific attributes on a specified server.

Type annotations for
`session.create_client("opsworkscm").update_server_engine_attributes` method.

Boto3 documentation:
[OpsWorksCM.Client.update_server_engine_attributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.update_server_engine_attributes)

Asynchronous method. Use `await update_server_engine_attributes(...)` for a
synchronous call.

Arguments mapping described in
[UpdateServerEngineAttributesRequestRequestTypeDef](./type_defs.md#updateserverengineattributesrequestrequesttypedef).

Keyword-only arguments:

- `ServerName`: `str` *(required)*
- `AttributeName`: `str` *(required)*
- `AttributeValue`: `str`

Returns a `Coroutine` for
[UpdateServerEngineAttributesResponseTypeDef](./type_defs.md#updateserverengineattributesresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("opsworkscm").__aenter__` method.

Boto3 documentation:
[OpsWorksCM.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [OpsWorksCMClient](#opsworkscmclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("opsworkscm").__aexit__` method.

Boto3 documentation:
[OpsWorksCM.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("opsworkscm").get_paginator` method
with overloads.

- `client.get_paginator("describe_backups")` ->
  [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
- `client.get_paginator("describe_events")` ->
  [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
- `client.get_paginator("describe_servers")` ->
  [DescribeServersPaginator](./paginators.md#describeserverspaginator)
- `client.get_paginator("list_tags_for_resource")` ->
  [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("opsworkscm").get_waiter` method
with overloads.

- `client.get_waiter("node_associated")` ->
  [NodeAssociatedWaiter](./waiters.md#nodeassociatedwaiter)
