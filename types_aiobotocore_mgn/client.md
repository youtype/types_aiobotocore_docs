<a id="mgnclient-for-aiobotocore-mgn-module"></a>

# mgnClient for aiobotocore mgn module

> [Index](..) > [mgn](.) > mgnClient

Auto-generated documentation for
[mgn](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
type annotations stubs module
[types-aiobotocore-mgn](https://pypi.org/project/types-aiobotocore-mgn/).

- [mgnClient for aiobotocore mgn module](#mgnclient-for-aiobotocore-mgn-module)
  - [mgnClient](#mgnclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [change_server_life_cycle_state](#change_server_life_cycle_state)
    - [create_replication_configuration_template](#create_replication_configuration_template)
    - [delete_job](#delete_job)
    - [delete_replication_configuration_template](#delete_replication_configuration_template)
    - [delete_source_server](#delete_source_server)
    - [delete_vcenter_client](#delete_vcenter_client)
    - [describe_job_log_items](#describe_job_log_items)
    - [describe_jobs](#describe_jobs)
    - [describe_replication_configuration_templates](#describe_replication_configuration_templates)
    - [describe_source_servers](#describe_source_servers)
    - [describe_vcenter_clients](#describe_vcenter_clients)
    - [disconnect_from_service](#disconnect_from_service)
    - [finalize_cutover](#finalize_cutover)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_launch_configuration](#get_launch_configuration)
    - [get_replication_configuration](#get_replication_configuration)
    - [initialize_service](#initialize_service)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [mark_as_archived](#mark_as_archived)
    - [retry_data_replication](#retry_data_replication)
    - [start_cutover](#start_cutover)
    - [start_replication](#start_replication)
    - [start_test](#start_test)
    - [tag_resource](#tag_resource)
    - [terminate_target_instances](#terminate_target_instances)
    - [untag_resource](#untag_resource)
    - [update_launch_configuration](#update_launch_configuration)
    - [update_replication_configuration](#update_replication_configuration)
    - [update_replication_configuration_template](#update_replication_configuration_template)
    - [update_source_server_replication_type](#update_source_server_replication_type)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="mgnclient"></a>

## mgnClient

Type annotations for `session.create_client("mgn")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_mgn.client import mgnClient

session = get_session()
async with session.create_client("mgn") as client:
    client: mgnClient
```

Boto3 documentation:
[mgn.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_mgn.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.UninitializedAccountException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

mgnClient exceptions.

Type annotations for `session.create_client("mgn").exceptions` method.

Boto3 documentation:
[mgn.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("mgn").can_paginate` method.

Boto3 documentation:
[mgn.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="change_server_life_cycle_state"></a>

### change_server_life_cycle_state

Allows the user to set the SourceServer.LifeCycle.state property for specific
Source Server IDs to one of the following: READY_FOR_TEST or READY_FOR_CUTOVER.

Type annotations for
`session.create_client("mgn").change_server_life_cycle_state` method.

Boto3 documentation:
[mgn.Client.change_server_life_cycle_state](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.change_server_life_cycle_state)

Asynchronous method. Use `await change_server_life_cycle_state(...)` for a
synchronous call.

Arguments mapping described in
[ChangeServerLifeCycleStateRequestRequestTypeDef](./type_defs.md#changeserverlifecyclestaterequestrequesttypedef).

Keyword-only arguments:

- `lifeCycle`:
  [ChangeServerLifeCycleStateSourceServerLifecycleTypeDef](./type_defs.md#changeserverlifecyclestatesourceserverlifecycletypedef)
  *(required)*
- `sourceServerID`: `str` *(required)*

Returns a `Coroutine` for
[SourceServerResponseMetadataTypeDef](./type_defs.md#sourceserverresponsemetadatatypedef).

<a id="create_replication_configuration_template"></a>

### create_replication_configuration_template

Creates a new ReplicationConfigurationTemplate.

Type annotations for
`session.create_client("mgn").create_replication_configuration_template`
method.

Boto3 documentation:
[mgn.Client.create_replication_configuration_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_replication_configuration_template)

Asynchronous method. Use `await create_replication_configuration_template(...)`
for a synchronous call.

Arguments mapping described in
[CreateReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#createreplicationconfigurationtemplaterequestrequesttypedef).

Keyword-only arguments:

- `associateDefaultSecurityGroup`: `bool` *(required)*
- `bandwidthThrottling`: `int` *(required)*
- `createPublicIP`: `bool` *(required)*
- `dataPlaneRouting`:
  [ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype)
  *(required)*
- `defaultLargeStagingDiskType`:
  [ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype)
  *(required)*
- `ebsEncryption`:
  [ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype)
  *(required)*
- `replicationServerInstanceType`: `str` *(required)*
- `replicationServersSecurityGroupsIDs`: `Sequence`\[`str`\] *(required)*
- `stagingAreaSubnetId`: `str` *(required)*
- `stagingAreaTags`: `Mapping`\[`str`, `str`\] *(required)*
- `useDedicatedReplicationServer`: `bool` *(required)*
- `ebsEncryptionKeyArn`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[ReplicationConfigurationTemplateResponseMetadataTypeDef](./type_defs.md#replicationconfigurationtemplateresponsemetadatatypedef).

<a id="delete_job"></a>

### delete_job

Deletes a single Job by ID.

Type annotations for `session.create_client("mgn").delete_job` method.

Boto3 documentation:
[mgn.Client.delete_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_job)

Asynchronous method. Use `await delete_job(...)` for a synchronous call.

Arguments mapping described in
[DeleteJobRequestRequestTypeDef](./type_defs.md#deletejobrequestrequesttypedef).

Keyword-only arguments:

- `jobID`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_replication_configuration_template"></a>

### delete_replication_configuration_template

Deletes a single Replication Configuration Template by ID See also:
[AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/mgn-2020-02-26/DeleteReplicationConfigurationTemplate).

Type annotations for
`session.create_client("mgn").delete_replication_configuration_template`
method.

Boto3 documentation:
[mgn.Client.delete_replication_configuration_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_replication_configuration_template)

Asynchronous method. Use `await delete_replication_configuration_template(...)`
for a synchronous call.

Arguments mapping described in
[DeleteReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#deletereplicationconfigurationtemplaterequestrequesttypedef).

Keyword-only arguments:

- `replicationConfigurationTemplateID`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_source_server"></a>

### delete_source_server

Deletes a single source server by ID.

Type annotations for `session.create_client("mgn").delete_source_server`
method.

Boto3 documentation:
[mgn.Client.delete_source_server](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_source_server)

Asynchronous method. Use `await delete_source_server(...)` for a synchronous
call.

Arguments mapping described in
[DeleteSourceServerRequestRequestTypeDef](./type_defs.md#deletesourceserverrequestrequesttypedef).

Keyword-only arguments:

- `sourceServerID`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_vcenter_client"></a>

### delete_vcenter_client

Deletes a single vCenter client by ID.

Type annotations for `session.create_client("mgn").delete_vcenter_client`
method.

Boto3 documentation:
[mgn.Client.delete_vcenter_client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_vcenter_client)

Asynchronous method. Use `await delete_vcenter_client(...)` for a synchronous
call.

Arguments mapping described in
[DeleteVcenterClientRequestRequestTypeDef](./type_defs.md#deletevcenterclientrequestrequesttypedef).

Keyword-only arguments:

- `vcenterClientID`: `str` *(required)*

<a id="describe_job_log_items"></a>

### describe_job_log_items

Retrieves detailed Job log with paging.

Type annotations for `session.create_client("mgn").describe_job_log_items`
method.

Boto3 documentation:
[mgn.Client.describe_job_log_items](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_job_log_items)

Asynchronous method. Use `await describe_job_log_items(...)` for a synchronous
call.

Arguments mapping described in
[DescribeJobLogItemsRequestRequestTypeDef](./type_defs.md#describejoblogitemsrequestrequesttypedef).

Keyword-only arguments:

- `jobID`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef).

<a id="describe_jobs"></a>

### describe_jobs

Returns a list of Jobs.

Type annotations for `session.create_client("mgn").describe_jobs` method.

Boto3 documentation:
[mgn.Client.describe_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_jobs)

Asynchronous method. Use `await describe_jobs(...)` for a synchronous call.

Arguments mapping described in
[DescribeJobsRequestRequestTypeDef](./type_defs.md#describejobsrequestrequesttypedef).

Keyword-only arguments:

- `filters`:
  [DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef)
  *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef).

<a id="describe_replication_configuration_templates"></a>

### describe_replication_configuration_templates

Lists all ReplicationConfigurationTemplates, filtered by Source Server IDs.

Type annotations for
`session.create_client("mgn").describe_replication_configuration_templates`
method.

Boto3 documentation:
[mgn.Client.describe_replication_configuration_templates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_replication_configuration_templates)

Asynchronous method. Use
`await describe_replication_configuration_templates(...)` for a synchronous
call.

Arguments mapping described in
[DescribeReplicationConfigurationTemplatesRequestRequestTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequestrequesttypedef).

Keyword-only arguments:

- `replicationConfigurationTemplateIDs`: `Sequence`\[`str`\] *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef).

<a id="describe_source_servers"></a>

### describe_source_servers

Retrieves all SourceServers or multiple SourceServers by ID.

Type annotations for `session.create_client("mgn").describe_source_servers`
method.

Boto3 documentation:
[mgn.Client.describe_source_servers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_source_servers)

Asynchronous method. Use `await describe_source_servers(...)` for a synchronous
call.

Arguments mapping described in
[DescribeSourceServersRequestRequestTypeDef](./type_defs.md#describesourceserversrequestrequesttypedef).

Keyword-only arguments:

- `filters`:
  [DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef)
  *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef).

<a id="describe_vcenter_clients"></a>

### describe_vcenter_clients

Lists all vCenter clients.

Type annotations for `session.create_client("mgn").describe_vcenter_clients`
method.

Boto3 documentation:
[mgn.Client.describe_vcenter_clients](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_vcenter_clients)

Asynchronous method. Use `await describe_vcenter_clients(...)` for a
synchronous call.

Arguments mapping described in
[DescribeVcenterClientsRequestRequestTypeDef](./type_defs.md#describevcenterclientsrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[DescribeVcenterClientsResponseTypeDef](./type_defs.md#describevcenterclientsresponsetypedef).

<a id="disconnect_from_service"></a>

### disconnect_from_service

Disconnects specific Source Servers from Application Migration Service.

Type annotations for `session.create_client("mgn").disconnect_from_service`
method.

Boto3 documentation:
[mgn.Client.disconnect_from_service](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disconnect_from_service)

Asynchronous method. Use `await disconnect_from_service(...)` for a synchronous
call.

Arguments mapping described in
[DisconnectFromServiceRequestRequestTypeDef](./type_defs.md#disconnectfromservicerequestrequesttypedef).

Keyword-only arguments:

- `sourceServerID`: `str` *(required)*

Returns a `Coroutine` for
[SourceServerResponseMetadataTypeDef](./type_defs.md#sourceserverresponsemetadatatypedef).

<a id="finalize_cutover"></a>

### finalize_cutover

Finalizes the cutover immediately for specific Source Servers.

Type annotations for `session.create_client("mgn").finalize_cutover` method.

Boto3 documentation:
[mgn.Client.finalize_cutover](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.finalize_cutover)

Asynchronous method. Use `await finalize_cutover(...)` for a synchronous call.

Arguments mapping described in
[FinalizeCutoverRequestRequestTypeDef](./type_defs.md#finalizecutoverrequestrequesttypedef).

Keyword-only arguments:

- `sourceServerID`: `str` *(required)*

Returns a `Coroutine` for
[SourceServerResponseMetadataTypeDef](./type_defs.md#sourceserverresponsemetadatatypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("mgn").generate_presigned_url`
method.

Boto3 documentation:
[mgn.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_launch_configuration"></a>

### get_launch_configuration

Lists all LaunchConfigurations available, filtered by Source Server IDs.

Type annotations for `session.create_client("mgn").get_launch_configuration`
method.

Boto3 documentation:
[mgn.Client.get_launch_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_launch_configuration)

Asynchronous method. Use `await get_launch_configuration(...)` for a
synchronous call.

Arguments mapping described in
[GetLaunchConfigurationRequestRequestTypeDef](./type_defs.md#getlaunchconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `sourceServerID`: `str` *(required)*

Returns a `Coroutine` for
[LaunchConfigurationTypeDef](./type_defs.md#launchconfigurationtypedef).

<a id="get_replication_configuration"></a>

### get_replication_configuration

Lists all ReplicationConfigurations, filtered by Source Server ID.

Type annotations for
`session.create_client("mgn").get_replication_configuration` method.

Boto3 documentation:
[mgn.Client.get_replication_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_replication_configuration)

Asynchronous method. Use `await get_replication_configuration(...)` for a
synchronous call.

Arguments mapping described in
[GetReplicationConfigurationRequestRequestTypeDef](./type_defs.md#getreplicationconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `sourceServerID`: `str` *(required)*

Returns a `Coroutine` for
[ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef).

<a id="initialize_service"></a>

### initialize_service

Initialize Application Migration Service.

Type annotations for `session.create_client("mgn").initialize_service` method.

Boto3 documentation:
[mgn.Client.initialize_service](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.initialize_service)

Asynchronous method. Use `await initialize_service(...)` for a synchronous
call.

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

List all tags for your Application Migration Service resources.

Type annotations for `session.create_client("mgn").list_tags_for_resource`
method.

Boto3 documentation:
[mgn.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="mark_as_archived"></a>

### mark_as_archived

Archives specific Source Servers by setting the SourceServer.isArchived
property to true for specified SourceServers by ID.

Type annotations for `session.create_client("mgn").mark_as_archived` method.

Boto3 documentation:
[mgn.Client.mark_as_archived](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.mark_as_archived)

Asynchronous method. Use `await mark_as_archived(...)` for a synchronous call.

Arguments mapping described in
[MarkAsArchivedRequestRequestTypeDef](./type_defs.md#markasarchivedrequestrequesttypedef).

Keyword-only arguments:

- `sourceServerID`: `str` *(required)*

Returns a `Coroutine` for
[SourceServerResponseMetadataTypeDef](./type_defs.md#sourceserverresponsemetadatatypedef).

<a id="retry_data_replication"></a>

### retry_data_replication

Causes the data replication initiation sequence to begin immediately upon next
Handshake for specified SourceServer IDs, regardless of when the previous
initiation started.

Type annotations for `session.create_client("mgn").retry_data_replication`
method.

Boto3 documentation:
[mgn.Client.retry_data_replication](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.retry_data_replication)

Asynchronous method. Use `await retry_data_replication(...)` for a synchronous
call.

Arguments mapping described in
[RetryDataReplicationRequestRequestTypeDef](./type_defs.md#retrydatareplicationrequestrequesttypedef).

Keyword-only arguments:

- `sourceServerID`: `str` *(required)*

Returns a `Coroutine` for
[SourceServerResponseMetadataTypeDef](./type_defs.md#sourceserverresponsemetadatatypedef).

<a id="start_cutover"></a>

### start_cutover

Launches a Cutover Instance for specific Source Servers.

Type annotations for `session.create_client("mgn").start_cutover` method.

Boto3 documentation:
[mgn.Client.start_cutover](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_cutover)

Asynchronous method. Use `await start_cutover(...)` for a synchronous call.

Arguments mapping described in
[StartCutoverRequestRequestTypeDef](./type_defs.md#startcutoverrequestrequesttypedef).

Keyword-only arguments:

- `sourceServerIDs`: `Sequence`\[`str`\] *(required)*
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[StartCutoverResponseTypeDef](./type_defs.md#startcutoverresponsetypedef).

<a id="start_replication"></a>

### start_replication

Starts replication on source server by ID.

Type annotations for `session.create_client("mgn").start_replication` method.

Boto3 documentation:
[mgn.Client.start_replication](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_replication)

Asynchronous method. Use `await start_replication(...)` for a synchronous call.

Arguments mapping described in
[StartReplicationRequestRequestTypeDef](./type_defs.md#startreplicationrequestrequesttypedef).

Keyword-only arguments:

- `sourceServerID`: `str` *(required)*

Returns a `Coroutine` for
[SourceServerResponseMetadataTypeDef](./type_defs.md#sourceserverresponsemetadatatypedef).

<a id="start_test"></a>

### start_test

Lauches a Test Instance for specific Source Servers.

Type annotations for `session.create_client("mgn").start_test` method.

Boto3 documentation:
[mgn.Client.start_test](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_test)

Asynchronous method. Use `await start_test(...)` for a synchronous call.

Arguments mapping described in
[StartTestRequestRequestTypeDef](./type_defs.md#starttestrequestrequesttypedef).

Keyword-only arguments:

- `sourceServerIDs`: `Sequence`\[`str`\] *(required)*
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[StartTestResponseTypeDef](./type_defs.md#starttestresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Adds or overwrites only the specified tags for the specified Application
Migration Service resource or resources.

Type annotations for `session.create_client("mgn").tag_resource` method.

Boto3 documentation:
[mgn.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

<a id="terminate_target_instances"></a>

### terminate_target_instances

Starts a job that terminates specific launched EC2 Test and Cutover instances.

Type annotations for `session.create_client("mgn").terminate_target_instances`
method.

Boto3 documentation:
[mgn.Client.terminate_target_instances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.terminate_target_instances)

Asynchronous method. Use `await terminate_target_instances(...)` for a
synchronous call.

Arguments mapping described in
[TerminateTargetInstancesRequestRequestTypeDef](./type_defs.md#terminatetargetinstancesrequestrequesttypedef).

Keyword-only arguments:

- `sourceServerIDs`: `Sequence`\[`str`\] *(required)*
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[TerminateTargetInstancesResponseTypeDef](./type_defs.md#terminatetargetinstancesresponsetypedef).

<a id="untag_resource"></a>

### untag_resource

Deletes the specified set of tags from the specified set of Application
Migration Service resources.

Type annotations for `session.create_client("mgn").untag_resource` method.

Boto3 documentation:
[mgn.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

<a id="update_launch_configuration"></a>

### update_launch_configuration

Updates multiple LaunchConfigurations by Source Server ID.

Type annotations for `session.create_client("mgn").update_launch_configuration`
method.

Boto3 documentation:
[mgn.Client.update_launch_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration)

Asynchronous method. Use `await update_launch_configuration(...)` for a
synchronous call.

Arguments mapping described in
[UpdateLaunchConfigurationRequestRequestTypeDef](./type_defs.md#updatelaunchconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `sourceServerID`: `str` *(required)*
- `copyPrivateIp`: `bool`
- `copyTags`: `bool`
- `launchDisposition`:
  [LaunchDispositionType](./literals.md#launchdispositiontype)
- `licensing`: [LicensingTypeDef](./type_defs.md#licensingtypedef)
- `name`: `str`
- `targetInstanceTypeRightSizingMethod`:
  [TargetInstanceTypeRightSizingMethodType](./literals.md#targetinstancetyperightsizingmethodtype)

Returns a `Coroutine` for
[LaunchConfigurationTypeDef](./type_defs.md#launchconfigurationtypedef).

<a id="update_replication_configuration"></a>

### update_replication_configuration

Allows you to update multiple ReplicationConfigurations by Source Server ID.

Type annotations for
`session.create_client("mgn").update_replication_configuration` method.

Boto3 documentation:
[mgn.Client.update_replication_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration)

Asynchronous method. Use `await update_replication_configuration(...)` for a
synchronous call.

Arguments mapping described in
[UpdateReplicationConfigurationRequestRequestTypeDef](./type_defs.md#updatereplicationconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `sourceServerID`: `str` *(required)*
- `associateDefaultSecurityGroup`: `bool`
- `bandwidthThrottling`: `int`
- `createPublicIP`: `bool`
- `dataPlaneRouting`:
  [ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype)
- `defaultLargeStagingDiskType`:
  [ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype)
- `ebsEncryption`:
  [ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype)
- `ebsEncryptionKeyArn`: `str`
- `name`: `str`
- `replicatedDisks`:
  `Sequence`\[[ReplicationConfigurationReplicatedDiskTypeDef](./type_defs.md#replicationconfigurationreplicateddisktypedef)\]
- `replicationServerInstanceType`: `str`
- `replicationServersSecurityGroupsIDs`: `Sequence`\[`str`\]
- `stagingAreaSubnetId`: `str`
- `stagingAreaTags`: `Mapping`\[`str`, `str`\]
- `useDedicatedReplicationServer`: `bool`

Returns a `Coroutine` for
[ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef).

<a id="update_replication_configuration_template"></a>

### update_replication_configuration_template

Updates multiple ReplicationConfigurationTemplates by ID.

Type annotations for
`session.create_client("mgn").update_replication_configuration_template`
method.

Boto3 documentation:
[mgn.Client.update_replication_configuration_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration_template)

Asynchronous method. Use `await update_replication_configuration_template(...)`
for a synchronous call.

Arguments mapping described in
[UpdateReplicationConfigurationTemplateRequestRequestTypeDef](./type_defs.md#updatereplicationconfigurationtemplaterequestrequesttypedef).

Keyword-only arguments:

- `replicationConfigurationTemplateID`: `str` *(required)*
- `arn`: `str`
- `associateDefaultSecurityGroup`: `bool`
- `bandwidthThrottling`: `int`
- `createPublicIP`: `bool`
- `dataPlaneRouting`:
  [ReplicationConfigurationDataPlaneRoutingType](./literals.md#replicationconfigurationdataplaneroutingtype)
- `defaultLargeStagingDiskType`:
  [ReplicationConfigurationDefaultLargeStagingDiskTypeType](./literals.md#replicationconfigurationdefaultlargestagingdisktypetype)
- `ebsEncryption`:
  [ReplicationConfigurationEbsEncryptionType](./literals.md#replicationconfigurationebsencryptiontype)
- `ebsEncryptionKeyArn`: `str`
- `replicationServerInstanceType`: `str`
- `replicationServersSecurityGroupsIDs`: `Sequence`\[`str`\]
- `stagingAreaSubnetId`: `str`
- `stagingAreaTags`: `Mapping`\[`str`, `str`\]
- `useDedicatedReplicationServer`: `bool`

Returns a `Coroutine` for
[ReplicationConfigurationTemplateResponseMetadataTypeDef](./type_defs.md#replicationconfigurationtemplateresponsemetadatatypedef).

<a id="update_source_server_replication_type"></a>

### update_source_server_replication_type

Updates source server Replication Type by ID.

Type annotations for
`session.create_client("mgn").update_source_server_replication_type` method.

Boto3 documentation:
[mgn.Client.update_source_server_replication_type](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_source_server_replication_type)

Asynchronous method. Use `await update_source_server_replication_type(...)` for
a synchronous call.

Arguments mapping described in
[UpdateSourceServerReplicationTypeRequestRequestTypeDef](./type_defs.md#updatesourceserverreplicationtyperequestrequesttypedef).

Keyword-only arguments:

- `replicationType`: [ReplicationTypeType](./literals.md#replicationtypetype)
  *(required)*
- `sourceServerID`: `str` *(required)*

Returns a `Coroutine` for
[SourceServerResponseMetadataTypeDef](./type_defs.md#sourceserverresponsemetadatatypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("mgn").__aenter__` method.

Boto3 documentation:
[mgn.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [mgnClient](#mgnclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("mgn").__aexit__` method.

Boto3 documentation:
[mgn.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("mgn").get_paginator` method with
overloads.

- `client.get_paginator("describe_job_log_items")` ->
  [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
- `client.get_paginator("describe_jobs")` ->
  [DescribeJobsPaginator](./paginators.md#describejobspaginator)
- `client.get_paginator("describe_replication_configuration_templates")` ->
  [DescribeReplicationConfigurationTemplatesPaginator](./paginators.md#describereplicationconfigurationtemplatespaginator)
- `client.get_paginator("describe_source_servers")` ->
  [DescribeSourceServersPaginator](./paginators.md#describesourceserverspaginator)
- `client.get_paginator("describe_vcenter_clients")` ->
  [DescribeVcenterClientsPaginator](./paginators.md#describevcenterclientspaginator)
