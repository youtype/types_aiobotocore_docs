<a id="emrclient-for-aiobotocore-emr-module"></a>

# EMRClient for aiobotocore EMR module

> [Index](../README.md) > [EMR](./README.md) > EMRClient

Auto-generated documentation for
[EMR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
type annotations stubs module
[types-aiobotocore-emr](https://pypi.org/project/types-aiobotocore-emr/).

- [EMRClient for aiobotocore EMR module](#emrclient-for-aiobotocore-emr-module)
  - [EMRClient](#emrclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [add_instance_fleet](#add_instance_fleet)
    - [add_instance_groups](#add_instance_groups)
    - [add_job_flow_steps](#add_job_flow_steps)
    - [add_tags](#add_tags)
    - [can_paginate](#can_paginate)
    - [cancel_steps](#cancel_steps)
    - [create_security_configuration](#create_security_configuration)
    - [create_studio](#create_studio)
    - [create_studio_session_mapping](#create_studio_session_mapping)
    - [delete_security_configuration](#delete_security_configuration)
    - [delete_studio](#delete_studio)
    - [delete_studio_session_mapping](#delete_studio_session_mapping)
    - [describe_cluster](#describe_cluster)
    - [describe_job_flows](#describe_job_flows)
    - [describe_notebook_execution](#describe_notebook_execution)
    - [describe_release_label](#describe_release_label)
    - [describe_security_configuration](#describe_security_configuration)
    - [describe_step](#describe_step)
    - [describe_studio](#describe_studio)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_auto_termination_policy](#get_auto_termination_policy)
    - [get_block_public_access_configuration](#get_block_public_access_configuration)
    - [get_managed_scaling_policy](#get_managed_scaling_policy)
    - [get_studio_session_mapping](#get_studio_session_mapping)
    - [list_bootstrap_actions](#list_bootstrap_actions)
    - [list_clusters](#list_clusters)
    - [list_instance_fleets](#list_instance_fleets)
    - [list_instance_groups](#list_instance_groups)
    - [list_instances](#list_instances)
    - [list_notebook_executions](#list_notebook_executions)
    - [list_release_labels](#list_release_labels)
    - [list_security_configurations](#list_security_configurations)
    - [list_steps](#list_steps)
    - [list_studio_session_mappings](#list_studio_session_mappings)
    - [list_studios](#list_studios)
    - [modify_cluster](#modify_cluster)
    - [modify_instance_fleet](#modify_instance_fleet)
    - [modify_instance_groups](#modify_instance_groups)
    - [put_auto_scaling_policy](#put_auto_scaling_policy)
    - [put_auto_termination_policy](#put_auto_termination_policy)
    - [put_block_public_access_configuration](#put_block_public_access_configuration)
    - [put_managed_scaling_policy](#put_managed_scaling_policy)
    - [remove_auto_scaling_policy](#remove_auto_scaling_policy)
    - [remove_auto_termination_policy](#remove_auto_termination_policy)
    - [remove_managed_scaling_policy](#remove_managed_scaling_policy)
    - [remove_tags](#remove_tags)
    - [run_job_flow](#run_job_flow)
    - [set_termination_protection](#set_termination_protection)
    - [set_visible_to_all_users](#set_visible_to_all_users)
    - [start_notebook_execution](#start_notebook_execution)
    - [stop_notebook_execution](#stop_notebook_execution)
    - [terminate_job_flows](#terminate_job_flows)
    - [update_studio](#update_studio)
    - [update_studio_session_mapping](#update_studio_session_mapping)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="emrclient"></a>

## EMRClient

Type annotations for `session.create_client("emr")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_emr.client import EMRClient

session = get_session()
async with session.create_client("emr") as client:
    client: EMRClient
```

Boto3 documentation:
[EMR.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_emr.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InternalServerError`
- `Exceptions.InternalServerException`
- `Exceptions.InvalidRequestException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

EMRClient exceptions.

Type annotations for `session.create_client("emr").exceptions` method.

Boto3 documentation:
[EMR.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="add\_instance\_fleet"></a>

### add_instance_fleet

Adds an instance fleet to a running cluster.

Type annotations for `session.create_client("emr").add_instance_fleet` method.

Boto3 documentation:
[EMR.Client.add_instance_fleet](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_instance_fleet)

Asynchronous method. Use `await add_instance_fleet(...)` for a synchronous
call.

Arguments mapping described in
[AddInstanceFleetInputRequestTypeDef](./type_defs.md#addinstancefleetinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `InstanceFleet`:
  [InstanceFleetConfigTypeDef](./type_defs.md#instancefleetconfigtypedef)
  *(required)*

Returns a `Coroutine` for
[AddInstanceFleetOutputTypeDef](./type_defs.md#addinstancefleetoutputtypedef).

<a id="add\_instance\_groups"></a>

### add_instance_groups

Adds one or more instance groups to a running cluster.

Type annotations for `session.create_client("emr").add_instance_groups` method.

Boto3 documentation:
[EMR.Client.add_instance_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_instance_groups)

Asynchronous method. Use `await add_instance_groups(...)` for a synchronous
call.

Arguments mapping described in
[AddInstanceGroupsInputRequestTypeDef](./type_defs.md#addinstancegroupsinputrequesttypedef).

Keyword-only arguments:

- `InstanceGroups`:
  `Sequence`\[[InstanceGroupConfigTypeDef](./type_defs.md#instancegroupconfigtypedef)\]
  *(required)*
- `JobFlowId`: `str` *(required)*

Returns a `Coroutine` for
[AddInstanceGroupsOutputTypeDef](./type_defs.md#addinstancegroupsoutputtypedef).

<a id="add\_job\_flow\_steps"></a>

### add_job_flow_steps

AddJobFlowSteps adds new steps to a running cluster.

Type annotations for `session.create_client("emr").add_job_flow_steps` method.

Boto3 documentation:
[EMR.Client.add_job_flow_steps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_job_flow_steps)

Asynchronous method. Use `await add_job_flow_steps(...)` for a synchronous
call.

Arguments mapping described in
[AddJobFlowStepsInputRequestTypeDef](./type_defs.md#addjobflowstepsinputrequesttypedef).

Keyword-only arguments:

- `JobFlowId`: `str` *(required)*
- `Steps`: `Sequence`\[[StepConfigTypeDef](./type_defs.md#stepconfigtypedef)\]
  *(required)*

Returns a `Coroutine` for
[AddJobFlowStepsOutputTypeDef](./type_defs.md#addjobflowstepsoutputtypedef).

<a id="add\_tags"></a>

### add_tags

Adds tags to an Amazon EMR resource, such as a cluster or an Amazon EMR Studio.

Type annotations for `session.create_client("emr").add_tags` method.

Boto3 documentation:
[EMR.Client.add_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_tags)

Asynchronous method. Use `await add_tags(...)` for a synchronous call.

Arguments mapping described in
[AddTagsInputRequestTypeDef](./type_defs.md#addtagsinputrequesttypedef).

Keyword-only arguments:

- `ResourceId`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("emr").can_paginate` method.

Boto3 documentation:
[EMR.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel\_steps"></a>

### cancel_steps

Cancels a pending step or steps in a running cluster.

Type annotations for `session.create_client("emr").cancel_steps` method.

Boto3 documentation:
[EMR.Client.cancel_steps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.cancel_steps)

Asynchronous method. Use `await cancel_steps(...)` for a synchronous call.

Arguments mapping described in
[CancelStepsInputRequestTypeDef](./type_defs.md#cancelstepsinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `StepIds`: `Sequence`\[`str`\] *(required)*
- `StepCancellationOption`:
  [StepCancellationOptionType](./literals.md#stepcancellationoptiontype)

Returns a `Coroutine` for
[CancelStepsOutputTypeDef](./type_defs.md#cancelstepsoutputtypedef).

<a id="create\_security\_configuration"></a>

### create_security_configuration

Creates a security configuration, which is stored in the service and can be
specified when a cluster is created.

Type annotations for
`session.create_client("emr").create_security_configuration` method.

Boto3 documentation:
[EMR.Client.create_security_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.create_security_configuration)

Asynchronous method. Use `await create_security_configuration(...)` for a
synchronous call.

Arguments mapping described in
[CreateSecurityConfigurationInputRequestTypeDef](./type_defs.md#createsecurityconfigurationinputrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `SecurityConfiguration`: `str` *(required)*

Returns a `Coroutine` for
[CreateSecurityConfigurationOutputTypeDef](./type_defs.md#createsecurityconfigurationoutputtypedef).

<a id="create\_studio"></a>

### create_studio

Creates a new Amazon EMR Studio.

Type annotations for `session.create_client("emr").create_studio` method.

Boto3 documentation:
[EMR.Client.create_studio](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.create_studio)

Asynchronous method. Use `await create_studio(...)` for a synchronous call.

Arguments mapping described in
[CreateStudioInputRequestTypeDef](./type_defs.md#createstudioinputrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `AuthMode`: [AuthModeType](./literals.md#authmodetype) *(required)*
- `VpcId`: `str` *(required)*
- `SubnetIds`: `Sequence`\[`str`\] *(required)*
- `ServiceRole`: `str` *(required)*
- `WorkspaceSecurityGroupId`: `str` *(required)*
- `EngineSecurityGroupId`: `str` *(required)*
- `DefaultS3Location`: `str` *(required)*
- `Description`: `str`
- `UserRole`: `str`
- `IdpAuthUrl`: `str`
- `IdpRelayStateParameterName`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateStudioOutputTypeDef](./type_defs.md#createstudiooutputtypedef).

<a id="create\_studio\_session\_mapping"></a>

### create_studio_session_mapping

Maps a user or group to the Amazon EMR Studio specified by `StudioId` , and
applies a session policy to refine Studio permissions for that user or group.

Type annotations for
`session.create_client("emr").create_studio_session_mapping` method.

Boto3 documentation:
[EMR.Client.create_studio_session_mapping](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.create_studio_session_mapping)

Asynchronous method. Use `await create_studio_session_mapping(...)` for a
synchronous call.

Arguments mapping described in
[CreateStudioSessionMappingInputRequestTypeDef](./type_defs.md#createstudiosessionmappinginputrequesttypedef).

Keyword-only arguments:

- `StudioId`: `str` *(required)*
- `IdentityType`: [IdentityTypeType](./literals.md#identitytypetype)
  *(required)*
- `SessionPolicyArn`: `str` *(required)*
- `IdentityId`: `str`
- `IdentityName`: `str`

<a id="delete\_security\_configuration"></a>

### delete_security_configuration

Deletes a security configuration.

Type annotations for
`session.create_client("emr").delete_security_configuration` method.

Boto3 documentation:
[EMR.Client.delete_security_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.delete_security_configuration)

Asynchronous method. Use `await delete_security_configuration(...)` for a
synchronous call.

Arguments mapping described in
[DeleteSecurityConfigurationInputRequestTypeDef](./type_defs.md#deletesecurityconfigurationinputrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_studio"></a>

### delete_studio

Removes an Amazon EMR Studio from the Studio metadata store.

Type annotations for `session.create_client("emr").delete_studio` method.

Boto3 documentation:
[EMR.Client.delete_studio](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.delete_studio)

Asynchronous method. Use `await delete_studio(...)` for a synchronous call.

Arguments mapping described in
[DeleteStudioInputRequestTypeDef](./type_defs.md#deletestudioinputrequesttypedef).

Keyword-only arguments:

- `StudioId`: `str` *(required)*

<a id="delete\_studio\_session\_mapping"></a>

### delete_studio_session_mapping

Removes a user or group from an Amazon EMR Studio.

Type annotations for
`session.create_client("emr").delete_studio_session_mapping` method.

Boto3 documentation:
[EMR.Client.delete_studio_session_mapping](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.delete_studio_session_mapping)

Asynchronous method. Use `await delete_studio_session_mapping(...)` for a
synchronous call.

Arguments mapping described in
[DeleteStudioSessionMappingInputRequestTypeDef](./type_defs.md#deletestudiosessionmappinginputrequesttypedef).

Keyword-only arguments:

- `StudioId`: `str` *(required)*
- `IdentityType`: [IdentityTypeType](./literals.md#identitytypetype)
  *(required)*
- `IdentityId`: `str`
- `IdentityName`: `str`

<a id="describe\_cluster"></a>

### describe_cluster

Provides cluster-level details including status, hardware and software
configuration, VPC settings, and so on.

Type annotations for `session.create_client("emr").describe_cluster` method.

Boto3 documentation:
[EMR.Client.describe_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_cluster)

Asynchronous method. Use `await describe_cluster(...)` for a synchronous call.

Arguments mapping described in
[DescribeClusterInputRequestTypeDef](./type_defs.md#describeclusterinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeClusterOutputTypeDef](./type_defs.md#describeclusteroutputtypedef).

<a id="describe\_job\_flows"></a>

### describe_job_flows

This API is no longer supported and will eventually be removed.

Type annotations for `session.create_client("emr").describe_job_flows` method.

Boto3 documentation:
[EMR.Client.describe_job_flows](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_job_flows)

Asynchronous method. Use `await describe_job_flows(...)` for a synchronous
call.

Arguments mapping described in
[DescribeJobFlowsInputRequestTypeDef](./type_defs.md#describejobflowsinputrequesttypedef).

Keyword-only arguments:

- `CreatedAfter`: `Union`\[`datetime`, `str`\]
- `CreatedBefore`: `Union`\[`datetime`, `str`\]
- `JobFlowIds`: `Sequence`\[`str`\]
- `JobFlowStates`:
  `Sequence`\[[JobFlowExecutionStateType](./literals.md#jobflowexecutionstatetype)\]

Returns a `Coroutine` for
[DescribeJobFlowsOutputTypeDef](./type_defs.md#describejobflowsoutputtypedef).

<a id="describe\_notebook\_execution"></a>

### describe_notebook_execution

Provides details of a notebook execution.

Type annotations for `session.create_client("emr").describe_notebook_execution`
method.

Boto3 documentation:
[EMR.Client.describe_notebook_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_notebook_execution)

Asynchronous method. Use `await describe_notebook_execution(...)` for a
synchronous call.

Arguments mapping described in
[DescribeNotebookExecutionInputRequestTypeDef](./type_defs.md#describenotebookexecutioninputrequesttypedef).

Keyword-only arguments:

- `NotebookExecutionId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeNotebookExecutionOutputTypeDef](./type_defs.md#describenotebookexecutionoutputtypedef).

<a id="describe\_release\_label"></a>

### describe_release_label

Provides EMR release label details, such as releases available the region where
the API request is run, and the available applications for a specific EMR
release label.

Type annotations for `session.create_client("emr").describe_release_label`
method.

Boto3 documentation:
[EMR.Client.describe_release_label](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_release_label)

Asynchronous method. Use `await describe_release_label(...)` for a synchronous
call.

Arguments mapping described in
[DescribeReleaseLabelInputRequestTypeDef](./type_defs.md#describereleaselabelinputrequesttypedef).

Keyword-only arguments:

- `ReleaseLabel`: `str`
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[DescribeReleaseLabelOutputTypeDef](./type_defs.md#describereleaselabeloutputtypedef).

<a id="describe\_security\_configuration"></a>

### describe_security_configuration

Provides the details of a security configuration by returning the configuration
JSON.

Type annotations for
`session.create_client("emr").describe_security_configuration` method.

Boto3 documentation:
[EMR.Client.describe_security_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_security_configuration)

Asynchronous method. Use `await describe_security_configuration(...)` for a
synchronous call.

Arguments mapping described in
[DescribeSecurityConfigurationInputRequestTypeDef](./type_defs.md#describesecurityconfigurationinputrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[DescribeSecurityConfigurationOutputTypeDef](./type_defs.md#describesecurityconfigurationoutputtypedef).

<a id="describe\_step"></a>

### describe_step

Provides more detail about the cluster step.

Type annotations for `session.create_client("emr").describe_step` method.

Boto3 documentation:
[EMR.Client.describe_step](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_step)

Asynchronous method. Use `await describe_step(...)` for a synchronous call.

Arguments mapping described in
[DescribeStepInputRequestTypeDef](./type_defs.md#describestepinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `StepId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeStepOutputTypeDef](./type_defs.md#describestepoutputtypedef).

<a id="describe\_studio"></a>

### describe_studio

Returns details for the specified Amazon EMR Studio including ID, Name, VPC,
Studio access URL, and so on.

Type annotations for `session.create_client("emr").describe_studio` method.

Boto3 documentation:
[EMR.Client.describe_studio](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_studio)

Asynchronous method. Use `await describe_studio(...)` for a synchronous call.

Arguments mapping described in
[DescribeStudioInputRequestTypeDef](./type_defs.md#describestudioinputrequesttypedef).

Keyword-only arguments:

- `StudioId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeStudioOutputTypeDef](./type_defs.md#describestudiooutputtypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("emr").generate_presigned_url`
method.

Boto3 documentation:
[EMR.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_auto\_termination\_policy"></a>

### get_auto_termination_policy

Returns the auto-termination policy for an Amazon EMR cluster.

Type annotations for `session.create_client("emr").get_auto_termination_policy`
method.

Boto3 documentation:
[EMR.Client.get_auto_termination_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.get_auto_termination_policy)

Asynchronous method. Use `await get_auto_termination_policy(...)` for a
synchronous call.

Arguments mapping described in
[GetAutoTerminationPolicyInputRequestTypeDef](./type_defs.md#getautoterminationpolicyinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*

Returns a `Coroutine` for
[GetAutoTerminationPolicyOutputTypeDef](./type_defs.md#getautoterminationpolicyoutputtypedef).

<a id="get\_block\_public\_access\_configuration"></a>

### get_block_public_access_configuration

Returns the Amazon EMR block public access configuration for your Amazon Web
Services account in the current Region.

Type annotations for
`session.create_client("emr").get_block_public_access_configuration` method.

Boto3 documentation:
[EMR.Client.get_block_public_access_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.get_block_public_access_configuration)

Asynchronous method. Use `await get_block_public_access_configuration(...)` for
a synchronous call.

Returns a `Coroutine` for
[GetBlockPublicAccessConfigurationOutputTypeDef](./type_defs.md#getblockpublicaccessconfigurationoutputtypedef).

<a id="get\_managed\_scaling\_policy"></a>

### get_managed_scaling_policy

Fetches the attached managed scaling policy for an Amazon EMR cluster.

Type annotations for `session.create_client("emr").get_managed_scaling_policy`
method.

Boto3 documentation:
[EMR.Client.get_managed_scaling_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.get_managed_scaling_policy)

Asynchronous method. Use `await get_managed_scaling_policy(...)` for a
synchronous call.

Arguments mapping described in
[GetManagedScalingPolicyInputRequestTypeDef](./type_defs.md#getmanagedscalingpolicyinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*

Returns a `Coroutine` for
[GetManagedScalingPolicyOutputTypeDef](./type_defs.md#getmanagedscalingpolicyoutputtypedef).

<a id="get\_studio\_session\_mapping"></a>

### get_studio_session_mapping

Fetches mapping details for the specified Amazon EMR Studio and identity (user
or group).

Type annotations for `session.create_client("emr").get_studio_session_mapping`
method.

Boto3 documentation:
[EMR.Client.get_studio_session_mapping](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.get_studio_session_mapping)

Asynchronous method. Use `await get_studio_session_mapping(...)` for a
synchronous call.

Arguments mapping described in
[GetStudioSessionMappingInputRequestTypeDef](./type_defs.md#getstudiosessionmappinginputrequesttypedef).

Keyword-only arguments:

- `StudioId`: `str` *(required)*
- `IdentityType`: [IdentityTypeType](./literals.md#identitytypetype)
  *(required)*
- `IdentityId`: `str`
- `IdentityName`: `str`

Returns a `Coroutine` for
[GetStudioSessionMappingOutputTypeDef](./type_defs.md#getstudiosessionmappingoutputtypedef).

<a id="list\_bootstrap\_actions"></a>

### list_bootstrap_actions

Provides information about the bootstrap actions associated with a cluster.

Type annotations for `session.create_client("emr").list_bootstrap_actions`
method.

Boto3 documentation:
[EMR.Client.list_bootstrap_actions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_bootstrap_actions)

Asynchronous method. Use `await list_bootstrap_actions(...)` for a synchronous
call.

Arguments mapping described in
[ListBootstrapActionsInputRequestTypeDef](./type_defs.md#listbootstrapactionsinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `Marker`: `str`

Returns a `Coroutine` for
[ListBootstrapActionsOutputTypeDef](./type_defs.md#listbootstrapactionsoutputtypedef).

<a id="list\_clusters"></a>

### list_clusters

Provides the status of all clusters visible to this Amazon Web Services
account.

Type annotations for `session.create_client("emr").list_clusters` method.

Boto3 documentation:
[EMR.Client.list_clusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_clusters)

Asynchronous method. Use `await list_clusters(...)` for a synchronous call.

Arguments mapping described in
[ListClustersInputRequestTypeDef](./type_defs.md#listclustersinputrequesttypedef).

Keyword-only arguments:

- `CreatedAfter`: `Union`\[`datetime`, `str`\]
- `CreatedBefore`: `Union`\[`datetime`, `str`\]
- `ClusterStates`:
  `Sequence`\[[ClusterStateType](./literals.md#clusterstatetype)\]
- `Marker`: `str`

Returns a `Coroutine` for
[ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef).

<a id="list\_instance\_fleets"></a>

### list_instance_fleets

Lists all available details about the instance fleets in a cluster.

Type annotations for `session.create_client("emr").list_instance_fleets`
method.

Boto3 documentation:
[EMR.Client.list_instance_fleets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_instance_fleets)

Asynchronous method. Use `await list_instance_fleets(...)` for a synchronous
call.

Arguments mapping described in
[ListInstanceFleetsInputRequestTypeDef](./type_defs.md#listinstancefleetsinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `Marker`: `str`

Returns a `Coroutine` for
[ListInstanceFleetsOutputTypeDef](./type_defs.md#listinstancefleetsoutputtypedef).

<a id="list\_instance\_groups"></a>

### list_instance_groups

Provides all available details about the instance groups in a cluster.

Type annotations for `session.create_client("emr").list_instance_groups`
method.

Boto3 documentation:
[EMR.Client.list_instance_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_instance_groups)

Asynchronous method. Use `await list_instance_groups(...)` for a synchronous
call.

Arguments mapping described in
[ListInstanceGroupsInputRequestTypeDef](./type_defs.md#listinstancegroupsinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `Marker`: `str`

Returns a `Coroutine` for
[ListInstanceGroupsOutputTypeDef](./type_defs.md#listinstancegroupsoutputtypedef).

<a id="list\_instances"></a>

### list_instances

Provides information for all active EC2 instances and EC2 instances terminated
in the last 30 days, up to a maximum of 2,000.

Type annotations for `session.create_client("emr").list_instances` method.

Boto3 documentation:
[EMR.Client.list_instances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_instances)

Asynchronous method. Use `await list_instances(...)` for a synchronous call.

Arguments mapping described in
[ListInstancesInputRequestTypeDef](./type_defs.md#listinstancesinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `InstanceGroupId`: `str`
- `InstanceGroupTypes`:
  `Sequence`\[[InstanceGroupTypeType](./literals.md#instancegrouptypetype)\]
- `InstanceFleetId`: `str`
- `InstanceFleetType`:
  [InstanceFleetTypeType](./literals.md#instancefleettypetype)
- `InstanceStates`:
  `Sequence`\[[InstanceStateType](./literals.md#instancestatetype)\]
- `Marker`: `str`

Returns a `Coroutine` for
[ListInstancesOutputTypeDef](./type_defs.md#listinstancesoutputtypedef).

<a id="list\_notebook\_executions"></a>

### list_notebook_executions

Provides summaries of all notebook executions.

Type annotations for `session.create_client("emr").list_notebook_executions`
method.

Boto3 documentation:
[EMR.Client.list_notebook_executions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_notebook_executions)

Asynchronous method. Use `await list_notebook_executions(...)` for a
synchronous call.

Arguments mapping described in
[ListNotebookExecutionsInputRequestTypeDef](./type_defs.md#listnotebookexecutionsinputrequesttypedef).

Keyword-only arguments:

- `EditorId`: `str`
- `Status`:
  [NotebookExecutionStatusType](./literals.md#notebookexecutionstatustype)
- `From`: `Union`\[`datetime`, `str`\]
- `To`: `Union`\[`datetime`, `str`\]
- `Marker`: `str`

Returns a `Coroutine` for
[ListNotebookExecutionsOutputTypeDef](./type_defs.md#listnotebookexecutionsoutputtypedef).

<a id="list\_release\_labels"></a>

### list_release_labels

Retrieves release labels of EMR services in the region where the API is called.

Type annotations for `session.create_client("emr").list_release_labels` method.

Boto3 documentation:
[EMR.Client.list_release_labels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_release_labels)

Asynchronous method. Use `await list_release_labels(...)` for a synchronous
call.

Arguments mapping described in
[ListReleaseLabelsInputRequestTypeDef](./type_defs.md#listreleaselabelsinputrequesttypedef).

Keyword-only arguments:

- `Filters`:
  [ReleaseLabelFilterTypeDef](./type_defs.md#releaselabelfiltertypedef)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListReleaseLabelsOutputTypeDef](./type_defs.md#listreleaselabelsoutputtypedef).

<a id="list\_security\_configurations"></a>

### list_security_configurations

Lists all the security configurations visible to this account, providing their
creation dates and times, and their names.

Type annotations for
`session.create_client("emr").list_security_configurations` method.

Boto3 documentation:
[EMR.Client.list_security_configurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_security_configurations)

Asynchronous method. Use `await list_security_configurations(...)` for a
synchronous call.

Arguments mapping described in
[ListSecurityConfigurationsInputRequestTypeDef](./type_defs.md#listsecurityconfigurationsinputrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`

Returns a `Coroutine` for
[ListSecurityConfigurationsOutputTypeDef](./type_defs.md#listsecurityconfigurationsoutputtypedef).

<a id="list\_steps"></a>

### list_steps

Provides a list of steps for the cluster in reverse order unless you specify
`stepIds` with the request or filter by `StepStates`.

Type annotations for `session.create_client("emr").list_steps` method.

Boto3 documentation:
[EMR.Client.list_steps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_steps)

Asynchronous method. Use `await list_steps(...)` for a synchronous call.

Arguments mapping described in
[ListStepsInputRequestTypeDef](./type_defs.md#liststepsinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `StepStates`: `Sequence`\[[StepStateType](./literals.md#stepstatetype)\]
- `StepIds`: `Sequence`\[`str`\]
- `Marker`: `str`

Returns a `Coroutine` for
[ListStepsOutputTypeDef](./type_defs.md#liststepsoutputtypedef).

<a id="list\_studio\_session\_mappings"></a>

### list_studio_session_mappings

Returns a list of all user or group session mappings for the Amazon EMR Studio
specified by `StudioId` .

Type annotations for
`session.create_client("emr").list_studio_session_mappings` method.

Boto3 documentation:
[EMR.Client.list_studio_session_mappings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_studio_session_mappings)

Asynchronous method. Use `await list_studio_session_mappings(...)` for a
synchronous call.

Arguments mapping described in
[ListStudioSessionMappingsInputRequestTypeDef](./type_defs.md#liststudiosessionmappingsinputrequesttypedef).

Keyword-only arguments:

- `StudioId`: `str`
- `IdentityType`: [IdentityTypeType](./literals.md#identitytypetype)
- `Marker`: `str`

Returns a `Coroutine` for
[ListStudioSessionMappingsOutputTypeDef](./type_defs.md#liststudiosessionmappingsoutputtypedef).

<a id="list\_studios"></a>

### list_studios

Returns a list of all Amazon EMR Studios associated with the Amazon Web
Services account.

Type annotations for `session.create_client("emr").list_studios` method.

Boto3 documentation:
[EMR.Client.list_studios](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_studios)

Asynchronous method. Use `await list_studios(...)` for a synchronous call.

Arguments mapping described in
[ListStudiosInputRequestTypeDef](./type_defs.md#liststudiosinputrequesttypedef).

Keyword-only arguments:

- `Marker`: `str`

Returns a `Coroutine` for
[ListStudiosOutputTypeDef](./type_defs.md#liststudiosoutputtypedef).

<a id="modify\_cluster"></a>

### modify_cluster

Modifies the number of steps that can be executed concurrently for the cluster
specified using ClusterID.

Type annotations for `session.create_client("emr").modify_cluster` method.

Boto3 documentation:
[EMR.Client.modify_cluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.modify_cluster)

Asynchronous method. Use `await modify_cluster(...)` for a synchronous call.

Arguments mapping described in
[ModifyClusterInputRequestTypeDef](./type_defs.md#modifyclusterinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `StepConcurrencyLevel`: `int`

Returns a `Coroutine` for
[ModifyClusterOutputTypeDef](./type_defs.md#modifyclusteroutputtypedef).

<a id="modify\_instance\_fleet"></a>

### modify_instance_fleet

Modifies the target On-Demand and target Spot capacities for the instance fleet
with the specified InstanceFleetID within the cluster specified using
ClusterID.

Type annotations for `session.create_client("emr").modify_instance_fleet`
method.

Boto3 documentation:
[EMR.Client.modify_instance_fleet](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.modify_instance_fleet)

Asynchronous method. Use `await modify_instance_fleet(...)` for a synchronous
call.

Arguments mapping described in
[ModifyInstanceFleetInputRequestTypeDef](./type_defs.md#modifyinstancefleetinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `InstanceFleet`:
  [InstanceFleetModifyConfigTypeDef](./type_defs.md#instancefleetmodifyconfigtypedef)
  *(required)*

<a id="modify\_instance\_groups"></a>

### modify_instance_groups

ModifyInstanceGroups modifies the number of nodes and configuration settings of
an instance group.

Type annotations for `session.create_client("emr").modify_instance_groups`
method.

Boto3 documentation:
[EMR.Client.modify_instance_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.modify_instance_groups)

Asynchronous method. Use `await modify_instance_groups(...)` for a synchronous
call.

Arguments mapping described in
[ModifyInstanceGroupsInputRequestTypeDef](./type_defs.md#modifyinstancegroupsinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str`
- `InstanceGroups`:
  `Sequence`\[[InstanceGroupModifyConfigTypeDef](./type_defs.md#instancegroupmodifyconfigtypedef)\]

<a id="put\_auto\_scaling\_policy"></a>

### put_auto_scaling_policy

Creates or updates an automatic scaling policy for a core instance group or
task instance group in an Amazon EMR cluster.

Type annotations for `session.create_client("emr").put_auto_scaling_policy`
method.

Boto3 documentation:
[EMR.Client.put_auto_scaling_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_auto_scaling_policy)

Asynchronous method. Use `await put_auto_scaling_policy(...)` for a synchronous
call.

Arguments mapping described in
[PutAutoScalingPolicyInputRequestTypeDef](./type_defs.md#putautoscalingpolicyinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `InstanceGroupId`: `str` *(required)*
- `AutoScalingPolicy`:
  [AutoScalingPolicyTypeDef](./type_defs.md#autoscalingpolicytypedef)
  *(required)*

Returns a `Coroutine` for
[PutAutoScalingPolicyOutputTypeDef](./type_defs.md#putautoscalingpolicyoutputtypedef).

<a id="put\_auto\_termination\_policy"></a>

### put_auto_termination_policy

.

Type annotations for `session.create_client("emr").put_auto_termination_policy`
method.

Boto3 documentation:
[EMR.Client.put_auto_termination_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_auto_termination_policy)

Asynchronous method. Use `await put_auto_termination_policy(...)` for a
synchronous call.

Arguments mapping described in
[PutAutoTerminationPolicyInputRequestTypeDef](./type_defs.md#putautoterminationpolicyinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `AutoTerminationPolicy`:
  [AutoTerminationPolicyTypeDef](./type_defs.md#autoterminationpolicytypedef)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="put\_block\_public\_access\_configuration"></a>

### put_block_public_access_configuration

Creates or updates an Amazon EMR block public access configuration for your
Amazon Web Services account in the current Region.

Type annotations for
`session.create_client("emr").put_block_public_access_configuration` method.

Boto3 documentation:
[EMR.Client.put_block_public_access_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_block_public_access_configuration)

Asynchronous method. Use `await put_block_public_access_configuration(...)` for
a synchronous call.

Arguments mapping described in
[PutBlockPublicAccessConfigurationInputRequestTypeDef](./type_defs.md#putblockpublicaccessconfigurationinputrequesttypedef).

Keyword-only arguments:

- `BlockPublicAccessConfiguration`:
  [BlockPublicAccessConfigurationTypeDef](./type_defs.md#blockpublicaccessconfigurationtypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="put\_managed\_scaling\_policy"></a>

### put_managed_scaling_policy

Creates or updates a managed scaling policy for an Amazon EMR cluster.

Type annotations for `session.create_client("emr").put_managed_scaling_policy`
method.

Boto3 documentation:
[EMR.Client.put_managed_scaling_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_managed_scaling_policy)

Asynchronous method. Use `await put_managed_scaling_policy(...)` for a
synchronous call.

Arguments mapping described in
[PutManagedScalingPolicyInputRequestTypeDef](./type_defs.md#putmanagedscalingpolicyinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `ManagedScalingPolicy`:
  [ManagedScalingPolicyTypeDef](./type_defs.md#managedscalingpolicytypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="remove\_auto\_scaling\_policy"></a>

### remove_auto_scaling_policy

Removes an automatic scaling policy from a specified instance group within an
EMR cluster.

Type annotations for `session.create_client("emr").remove_auto_scaling_policy`
method.

Boto3 documentation:
[EMR.Client.remove_auto_scaling_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.remove_auto_scaling_policy)

Asynchronous method. Use `await remove_auto_scaling_policy(...)` for a
synchronous call.

Arguments mapping described in
[RemoveAutoScalingPolicyInputRequestTypeDef](./type_defs.md#removeautoscalingpolicyinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*
- `InstanceGroupId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="remove\_auto\_termination\_policy"></a>

### remove_auto_termination_policy

Removes an auto-termination policy from an Amazon EMR cluster.

Type annotations for
`session.create_client("emr").remove_auto_termination_policy` method.

Boto3 documentation:
[EMR.Client.remove_auto_termination_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.remove_auto_termination_policy)

Asynchronous method. Use `await remove_auto_termination_policy(...)` for a
synchronous call.

Arguments mapping described in
[RemoveAutoTerminationPolicyInputRequestTypeDef](./type_defs.md#removeautoterminationpolicyinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="remove\_managed\_scaling\_policy"></a>

### remove_managed_scaling_policy

Removes a managed scaling policy from a specified EMR cluster.

Type annotations for
`session.create_client("emr").remove_managed_scaling_policy` method.

Boto3 documentation:
[EMR.Client.remove_managed_scaling_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.remove_managed_scaling_policy)

Asynchronous method. Use `await remove_managed_scaling_policy(...)` for a
synchronous call.

Arguments mapping described in
[RemoveManagedScalingPolicyInputRequestTypeDef](./type_defs.md#removemanagedscalingpolicyinputrequesttypedef).

Keyword-only arguments:

- `ClusterId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="remove\_tags"></a>

### remove_tags

Removes tags from an Amazon EMR resource, such as a cluster or Amazon EMR
Studio.

Type annotations for `session.create_client("emr").remove_tags` method.

Boto3 documentation:
[EMR.Client.remove_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.remove_tags)

Asynchronous method. Use `await remove_tags(...)` for a synchronous call.

Arguments mapping described in
[RemoveTagsInputRequestTypeDef](./type_defs.md#removetagsinputrequesttypedef).

Keyword-only arguments:

- `ResourceId`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="run\_job\_flow"></a>

### run_job_flow

RunJobFlow creates and starts running a new cluster (job flow).

Type annotations for `session.create_client("emr").run_job_flow` method.

Boto3 documentation:
[EMR.Client.run_job_flow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.run_job_flow)

Asynchronous method. Use `await run_job_flow(...)` for a synchronous call.

Arguments mapping described in
[RunJobFlowInputRequestTypeDef](./type_defs.md#runjobflowinputrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Instances`:
  [JobFlowInstancesConfigTypeDef](./type_defs.md#jobflowinstancesconfigtypedef)
  *(required)*
- `LogUri`: `str`
- `LogEncryptionKmsKeyId`: `str`
- `AdditionalInfo`: `str`
- `AmiVersion`: `str`
- `ReleaseLabel`: `str`
- `Steps`: `Sequence`\[[StepConfigTypeDef](./type_defs.md#stepconfigtypedef)\]
- `BootstrapActions`:
  `Sequence`\[[BootstrapActionConfigTypeDef](./type_defs.md#bootstrapactionconfigtypedef)\]
- `SupportedProducts`: `Sequence`\[`str`\]
- `NewSupportedProducts`:
  `Sequence`\[[SupportedProductConfigTypeDef](./type_defs.md#supportedproductconfigtypedef)\]
- `Applications`:
  `Sequence`\[[ApplicationTypeDef](./type_defs.md#applicationtypedef)\]
- `Configurations`:
  `Sequence`\[[ConfigurationTypeDef](./type_defs.md#configurationtypedef)\]
- `VisibleToAllUsers`: `bool`
- `JobFlowRole`: `str`
- `ServiceRole`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `SecurityConfiguration`: `str`
- `AutoScalingRole`: `str`
- `ScaleDownBehavior`:
  [ScaleDownBehaviorType](./literals.md#scaledownbehaviortype)
- `CustomAmiId`: `str`
- `EbsRootVolumeSize`: `int`
- `RepoUpgradeOnBoot`:
  [RepoUpgradeOnBootType](./literals.md#repoupgradeonboottype)
- `KerberosAttributes`:
  [KerberosAttributesTypeDef](./type_defs.md#kerberosattributestypedef)
- `StepConcurrencyLevel`: `int`
- `ManagedScalingPolicy`:
  [ManagedScalingPolicyTypeDef](./type_defs.md#managedscalingpolicytypedef)
- `PlacementGroupConfigs`:
  `Sequence`\[[PlacementGroupConfigTypeDef](./type_defs.md#placementgroupconfigtypedef)\]
- `AutoTerminationPolicy`:
  [AutoTerminationPolicyTypeDef](./type_defs.md#autoterminationpolicytypedef)

Returns a `Coroutine` for
[RunJobFlowOutputTypeDef](./type_defs.md#runjobflowoutputtypedef).

<a id="set\_termination\_protection"></a>

### set_termination_protection

SetTerminationProtection locks a cluster (job flow) so the EC2 instances in the
cluster cannot be terminated by user intervention, an API call, or in the event
of a job-flow error.

Type annotations for `session.create_client("emr").set_termination_protection`
method.

Boto3 documentation:
[EMR.Client.set_termination_protection](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.set_termination_protection)

Asynchronous method. Use `await set_termination_protection(...)` for a
synchronous call.

Arguments mapping described in
[SetTerminationProtectionInputRequestTypeDef](./type_defs.md#setterminationprotectioninputrequesttypedef).

Keyword-only arguments:

- `JobFlowIds`: `Sequence`\[`str`\] *(required)*
- `TerminationProtected`: `bool` *(required)*

<a id="set\_visible\_to\_all\_users"></a>

### set_visible_to_all_users

.

Type annotations for `session.create_client("emr").set_visible_to_all_users`
method.

Boto3 documentation:
[EMR.Client.set_visible_to_all_users](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.set_visible_to_all_users)

Asynchronous method. Use `await set_visible_to_all_users(...)` for a
synchronous call.

Arguments mapping described in
[SetVisibleToAllUsersInputRequestTypeDef](./type_defs.md#setvisibletoallusersinputrequesttypedef).

Keyword-only arguments:

- `JobFlowIds`: `Sequence`\[`str`\] *(required)*
- `VisibleToAllUsers`: `bool` *(required)*

<a id="start\_notebook\_execution"></a>

### start_notebook_execution

Starts a notebook execution.

Type annotations for `session.create_client("emr").start_notebook_execution`
method.

Boto3 documentation:
[EMR.Client.start_notebook_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.start_notebook_execution)

Asynchronous method. Use `await start_notebook_execution(...)` for a
synchronous call.

Arguments mapping described in
[StartNotebookExecutionInputRequestTypeDef](./type_defs.md#startnotebookexecutioninputrequesttypedef).

Keyword-only arguments:

- `EditorId`: `str` *(required)*
- `RelativePath`: `str` *(required)*
- `ExecutionEngine`:
  [ExecutionEngineConfigTypeDef](./type_defs.md#executionengineconfigtypedef)
  *(required)*
- `ServiceRole`: `str` *(required)*
- `NotebookExecutionName`: `str`
- `NotebookParams`: `str`
- `NotebookInstanceSecurityGroupId`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[StartNotebookExecutionOutputTypeDef](./type_defs.md#startnotebookexecutionoutputtypedef).

<a id="stop\_notebook\_execution"></a>

### stop_notebook_execution

Stops a notebook execution.

Type annotations for `session.create_client("emr").stop_notebook_execution`
method.

Boto3 documentation:
[EMR.Client.stop_notebook_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.stop_notebook_execution)

Asynchronous method. Use `await stop_notebook_execution(...)` for a synchronous
call.

Arguments mapping described in
[StopNotebookExecutionInputRequestTypeDef](./type_defs.md#stopnotebookexecutioninputrequesttypedef).

Keyword-only arguments:

- `NotebookExecutionId`: `str` *(required)*

<a id="terminate\_job\_flows"></a>

### terminate_job_flows

TerminateJobFlows shuts a list of clusters (job flows) down.

Type annotations for `session.create_client("emr").terminate_job_flows` method.

Boto3 documentation:
[EMR.Client.terminate_job_flows](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.terminate_job_flows)

Asynchronous method. Use `await terminate_job_flows(...)` for a synchronous
call.

Arguments mapping described in
[TerminateJobFlowsInputRequestTypeDef](./type_defs.md#terminatejobflowsinputrequesttypedef).

Keyword-only arguments:

- `JobFlowIds`: `Sequence`\[`str`\] *(required)*

<a id="update\_studio"></a>

### update_studio

Updates an Amazon EMR Studio configuration, including attributes such as name,
description, and subnets.

Type annotations for `session.create_client("emr").update_studio` method.

Boto3 documentation:
[EMR.Client.update_studio](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.update_studio)

Asynchronous method. Use `await update_studio(...)` for a synchronous call.

Arguments mapping described in
[UpdateStudioInputRequestTypeDef](./type_defs.md#updatestudioinputrequesttypedef).

Keyword-only arguments:

- `StudioId`: `str` *(required)*
- `Name`: `str`
- `Description`: `str`
- `SubnetIds`: `Sequence`\[`str`\]
- `DefaultS3Location`: `str`

<a id="update\_studio\_session\_mapping"></a>

### update_studio_session_mapping

Updates the session policy attached to the user or group for the specified
Amazon EMR Studio.

Type annotations for
`session.create_client("emr").update_studio_session_mapping` method.

Boto3 documentation:
[EMR.Client.update_studio_session_mapping](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.update_studio_session_mapping)

Asynchronous method. Use `await update_studio_session_mapping(...)` for a
synchronous call.

Arguments mapping described in
[UpdateStudioSessionMappingInputRequestTypeDef](./type_defs.md#updatestudiosessionmappinginputrequesttypedef).

Keyword-only arguments:

- `StudioId`: `str` *(required)*
- `IdentityType`: [IdentityTypeType](./literals.md#identitytypetype)
  *(required)*
- `SessionPolicyArn`: `str` *(required)*
- `IdentityId`: `str`
- `IdentityName`: `str`

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("emr").__aenter__` method.

Boto3 documentation:
[EMR.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [EMRClient](#emrclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("emr").__aexit__` method.

Boto3 documentation:
[EMR.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("emr").get_paginator` method with
overloads.

- `client.get_paginator("list_bootstrap_actions")` ->
  [ListBootstrapActionsPaginator](./paginators.md#listbootstrapactionspaginator)
- `client.get_paginator("list_clusters")` ->
  [ListClustersPaginator](./paginators.md#listclusterspaginator)
- `client.get_paginator("list_instance_fleets")` ->
  [ListInstanceFleetsPaginator](./paginators.md#listinstancefleetspaginator)
- `client.get_paginator("list_instance_groups")` ->
  [ListInstanceGroupsPaginator](./paginators.md#listinstancegroupspaginator)
- `client.get_paginator("list_instances")` ->
  [ListInstancesPaginator](./paginators.md#listinstancespaginator)
- `client.get_paginator("list_notebook_executions")` ->
  [ListNotebookExecutionsPaginator](./paginators.md#listnotebookexecutionspaginator)
- `client.get_paginator("list_security_configurations")` ->
  [ListSecurityConfigurationsPaginator](./paginators.md#listsecurityconfigurationspaginator)
- `client.get_paginator("list_steps")` ->
  [ListStepsPaginator](./paginators.md#liststepspaginator)
- `client.get_paginator("list_studio_session_mappings")` ->
  [ListStudioSessionMappingsPaginator](./paginators.md#liststudiosessionmappingspaginator)
- `client.get_paginator("list_studios")` ->
  [ListStudiosPaginator](./paginators.md#liststudiospaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("emr").get_waiter` method with
overloads.

- `client.get_waiter("cluster_running")` ->
  [ClusterRunningWaiter](./waiters.md#clusterrunningwaiter)
- `client.get_waiter("cluster_terminated")` ->
  [ClusterTerminatedWaiter](./waiters.md#clusterterminatedwaiter)
- `client.get_waiter("step_complete")` ->
  [StepCompleteWaiter](./waiters.md#stepcompletewaiter)
