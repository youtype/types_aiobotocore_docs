<a id="robomakerclient-for-aiobotocore-robomaker-module"></a>

# RoboMakerClient for aiobotocore RoboMaker module

> [Index](../README.md) > [RoboMaker](./README.md) > RoboMakerClient

Auto-generated documentation for
[RoboMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
type annotations stubs module
[types-aiobotocore-robomaker](https://pypi.org/project/types-aiobotocore-robomaker/).

- [RoboMakerClient for aiobotocore RoboMaker module](#robomakerclient-for-aiobotocore-robomaker-module)
  - [RoboMakerClient](#robomakerclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [batch_delete_worlds](#batch_delete_worlds)
    - [batch_describe_simulation_job](#batch_describe_simulation_job)
    - [can_paginate](#can_paginate)
    - [cancel_deployment_job](#cancel_deployment_job)
    - [cancel_simulation_job](#cancel_simulation_job)
    - [cancel_simulation_job_batch](#cancel_simulation_job_batch)
    - [cancel_world_export_job](#cancel_world_export_job)
    - [cancel_world_generation_job](#cancel_world_generation_job)
    - [create_deployment_job](#create_deployment_job)
    - [create_fleet](#create_fleet)
    - [create_robot](#create_robot)
    - [create_robot_application](#create_robot_application)
    - [create_robot_application_version](#create_robot_application_version)
    - [create_simulation_application](#create_simulation_application)
    - [create_simulation_application_version](#create_simulation_application_version)
    - [create_simulation_job](#create_simulation_job)
    - [create_world_export_job](#create_world_export_job)
    - [create_world_generation_job](#create_world_generation_job)
    - [create_world_template](#create_world_template)
    - [delete_fleet](#delete_fleet)
    - [delete_robot](#delete_robot)
    - [delete_robot_application](#delete_robot_application)
    - [delete_simulation_application](#delete_simulation_application)
    - [delete_world_template](#delete_world_template)
    - [deregister_robot](#deregister_robot)
    - [describe_deployment_job](#describe_deployment_job)
    - [describe_fleet](#describe_fleet)
    - [describe_robot](#describe_robot)
    - [describe_robot_application](#describe_robot_application)
    - [describe_simulation_application](#describe_simulation_application)
    - [describe_simulation_job](#describe_simulation_job)
    - [describe_simulation_job_batch](#describe_simulation_job_batch)
    - [describe_world](#describe_world)
    - [describe_world_export_job](#describe_world_export_job)
    - [describe_world_generation_job](#describe_world_generation_job)
    - [describe_world_template](#describe_world_template)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_world_template_body](#get_world_template_body)
    - [list_deployment_jobs](#list_deployment_jobs)
    - [list_fleets](#list_fleets)
    - [list_robot_applications](#list_robot_applications)
    - [list_robots](#list_robots)
    - [list_simulation_applications](#list_simulation_applications)
    - [list_simulation_job_batches](#list_simulation_job_batches)
    - [list_simulation_jobs](#list_simulation_jobs)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_world_export_jobs](#list_world_export_jobs)
    - [list_world_generation_jobs](#list_world_generation_jobs)
    - [list_world_templates](#list_world_templates)
    - [list_worlds](#list_worlds)
    - [register_robot](#register_robot)
    - [restart_simulation_job](#restart_simulation_job)
    - [start_simulation_job_batch](#start_simulation_job_batch)
    - [sync_deployment_job](#sync_deployment_job)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_robot_application](#update_robot_application)
    - [update_simulation_application](#update_simulation_application)
    - [update_world_template](#update_world_template)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="robomakerclient"></a>

## RoboMakerClient

Type annotations for `session.create_client("robomaker")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_robomaker.client import RoboMakerClient

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
```

Boto3 documentation:
[RoboMaker.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_robomaker.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConcurrentDeploymentException`
- `Exceptions.IdempotentParameterMismatchException`
- `Exceptions.InternalServerException`
- `Exceptions.InvalidParameterException`
- `Exceptions.LimitExceededException`
- `Exceptions.ResourceAlreadyExistsException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceUnavailableException`
- `Exceptions.ThrottlingException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

RoboMakerClient exceptions.

Type annotations for `session.create_client("robomaker").exceptions` method.

Boto3 documentation:
[RoboMaker.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="batch\_delete\_worlds"></a>

### batch_delete_worlds

Deletes one or more worlds in a batch operation.

Type annotations for `session.create_client("robomaker").batch_delete_worlds`
method.

Boto3 documentation:
[RoboMaker.Client.batch_delete_worlds](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.batch_delete_worlds)

Asynchronous method. Use `await batch_delete_worlds(...)` for a synchronous
call.

Arguments mapping described in
[BatchDeleteWorldsRequestRequestTypeDef](./type_defs.md#batchdeleteworldsrequestrequesttypedef).

Keyword-only arguments:

- `worlds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[BatchDeleteWorldsResponseTypeDef](./type_defs.md#batchdeleteworldsresponsetypedef).

<a id="batch\_describe\_simulation\_job"></a>

### batch_describe_simulation_job

Describes one or more simulation jobs.

Type annotations for
`session.create_client("robomaker").batch_describe_simulation_job` method.

Boto3 documentation:
[RoboMaker.Client.batch_describe_simulation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.batch_describe_simulation_job)

Asynchronous method. Use `await batch_describe_simulation_job(...)` for a
synchronous call.

Arguments mapping described in
[BatchDescribeSimulationJobRequestRequestTypeDef](./type_defs.md#batchdescribesimulationjobrequestrequesttypedef).

Keyword-only arguments:

- `jobs`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[BatchDescribeSimulationJobResponseTypeDef](./type_defs.md#batchdescribesimulationjobresponsetypedef).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("robomaker").can_paginate` method.

Boto3 documentation:
[RoboMaker.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel\_deployment\_job"></a>

### cancel_deployment_job

Cancels the specified deployment job.

Type annotations for `session.create_client("robomaker").cancel_deployment_job`
method.

Boto3 documentation:
[RoboMaker.Client.cancel_deployment_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.cancel_deployment_job)

Asynchronous method. Use `await cancel_deployment_job(...)` for a synchronous
call.

Arguments mapping described in
[CancelDeploymentJobRequestRequestTypeDef](./type_defs.md#canceldeploymentjobrequestrequesttypedef).

Keyword-only arguments:

- `job`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="cancel\_simulation\_job"></a>

### cancel_simulation_job

Cancels the specified simulation job.

Type annotations for `session.create_client("robomaker").cancel_simulation_job`
method.

Boto3 documentation:
[RoboMaker.Client.cancel_simulation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.cancel_simulation_job)

Asynchronous method. Use `await cancel_simulation_job(...)` for a synchronous
call.

Arguments mapping described in
[CancelSimulationJobRequestRequestTypeDef](./type_defs.md#cancelsimulationjobrequestrequesttypedef).

Keyword-only arguments:

- `job`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="cancel\_simulation\_job\_batch"></a>

### cancel_simulation_job_batch

Cancels a simulation job batch.

Type annotations for
`session.create_client("robomaker").cancel_simulation_job_batch` method.

Boto3 documentation:
[RoboMaker.Client.cancel_simulation_job_batch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.cancel_simulation_job_batch)

Asynchronous method. Use `await cancel_simulation_job_batch(...)` for a
synchronous call.

Arguments mapping described in
[CancelSimulationJobBatchRequestRequestTypeDef](./type_defs.md#cancelsimulationjobbatchrequestrequesttypedef).

Keyword-only arguments:

- `batch`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="cancel\_world\_export\_job"></a>

### cancel_world_export_job

Cancels the specified export job.

Type annotations for
`session.create_client("robomaker").cancel_world_export_job` method.

Boto3 documentation:
[RoboMaker.Client.cancel_world_export_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.cancel_world_export_job)

Asynchronous method. Use `await cancel_world_export_job(...)` for a synchronous
call.

Arguments mapping described in
[CancelWorldExportJobRequestRequestTypeDef](./type_defs.md#cancelworldexportjobrequestrequesttypedef).

Keyword-only arguments:

- `job`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="cancel\_world\_generation\_job"></a>

### cancel_world_generation_job

Cancels the specified world generator job.

Type annotations for
`session.create_client("robomaker").cancel_world_generation_job` method.

Boto3 documentation:
[RoboMaker.Client.cancel_world_generation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.cancel_world_generation_job)

Asynchronous method. Use `await cancel_world_generation_job(...)` for a
synchronous call.

Arguments mapping described in
[CancelWorldGenerationJobRequestRequestTypeDef](./type_defs.md#cancelworldgenerationjobrequestrequesttypedef).

Keyword-only arguments:

- `job`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="create\_deployment\_job"></a>

### create_deployment_job

Deploys a specific version of a robot application to robots in a fleet.

Type annotations for `session.create_client("robomaker").create_deployment_job`
method.

Boto3 documentation:
[RoboMaker.Client.create_deployment_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_deployment_job)

Asynchronous method. Use `await create_deployment_job(...)` for a synchronous
call.

Arguments mapping described in
[CreateDeploymentJobRequestRequestTypeDef](./type_defs.md#createdeploymentjobrequestrequesttypedef).

Keyword-only arguments:

- `clientRequestToken`: `str` *(required)*
- `fleet`: `str` *(required)*
- `deploymentApplicationConfigs`:
  `Sequence`\[[DeploymentApplicationConfigTypeDef](./type_defs.md#deploymentapplicationconfigtypedef)\]
  *(required)*
- `deploymentConfig`:
  [DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef)
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateDeploymentJobResponseTypeDef](./type_defs.md#createdeploymentjobresponsetypedef).

<a id="create\_fleet"></a>

### create_fleet

Creates a fleet, a logical group of robots running the same robot application.

Type annotations for `session.create_client("robomaker").create_fleet` method.

Boto3 documentation:
[RoboMaker.Client.create_fleet](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_fleet)

Asynchronous method. Use `await create_fleet(...)` for a synchronous call.

Arguments mapping described in
[CreateFleetRequestRequestTypeDef](./type_defs.md#createfleetrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateFleetResponseTypeDef](./type_defs.md#createfleetresponsetypedef).

<a id="create\_robot"></a>

### create_robot

Creates a robot.

Type annotations for `session.create_client("robomaker").create_robot` method.

Boto3 documentation:
[RoboMaker.Client.create_robot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_robot)

Asynchronous method. Use `await create_robot(...)` for a synchronous call.

Arguments mapping described in
[CreateRobotRequestRequestTypeDef](./type_defs.md#createrobotrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `architecture`: [ArchitectureType](./literals.md#architecturetype)
  *(required)*
- `greengrassGroupId`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateRobotResponseTypeDef](./type_defs.md#createrobotresponsetypedef).

<a id="create\_robot\_application"></a>

### create_robot_application

Creates a robot application.

Type annotations for
`session.create_client("robomaker").create_robot_application` method.

Boto3 documentation:
[RoboMaker.Client.create_robot_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_robot_application)

Asynchronous method. Use `await create_robot_application(...)` for a
synchronous call.

Arguments mapping described in
[CreateRobotApplicationRequestRequestTypeDef](./type_defs.md#createrobotapplicationrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `robotSoftwareSuite`:
  [RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef)
  *(required)*
- `sources`:
  `Sequence`\[[SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef)\]
- `tags`: `Mapping`\[`str`, `str`\]
- `environment`: [EnvironmentTypeDef](./type_defs.md#environmenttypedef)

Returns a `Coroutine` for
[CreateRobotApplicationResponseTypeDef](./type_defs.md#createrobotapplicationresponsetypedef).

<a id="create\_robot\_application\_version"></a>

### create_robot_application_version

Creates a version of a robot application.

Type annotations for
`session.create_client("robomaker").create_robot_application_version` method.

Boto3 documentation:
[RoboMaker.Client.create_robot_application_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_robot_application_version)

Asynchronous method. Use `await create_robot_application_version(...)` for a
synchronous call.

Arguments mapping described in
[CreateRobotApplicationVersionRequestRequestTypeDef](./type_defs.md#createrobotapplicationversionrequestrequesttypedef).

Keyword-only arguments:

- `application`: `str` *(required)*
- `currentRevisionId`: `str`
- `s3Etags`: `Sequence`\[`str`\]
- `imageDigest`: `str`

Returns a `Coroutine` for
[CreateRobotApplicationVersionResponseTypeDef](./type_defs.md#createrobotapplicationversionresponsetypedef).

<a id="create\_simulation\_application"></a>

### create_simulation_application

Creates a simulation application.

Type annotations for
`session.create_client("robomaker").create_simulation_application` method.

Boto3 documentation:
[RoboMaker.Client.create_simulation_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_application)

Asynchronous method. Use `await create_simulation_application(...)` for a
synchronous call.

Arguments mapping described in
[CreateSimulationApplicationRequestRequestTypeDef](./type_defs.md#createsimulationapplicationrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `simulationSoftwareSuite`:
  [SimulationSoftwareSuiteTypeDef](./type_defs.md#simulationsoftwaresuitetypedef)
  *(required)*
- `robotSoftwareSuite`:
  [RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef)
  *(required)*
- `sources`:
  `Sequence`\[[SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef)\]
- `renderingEngine`:
  [RenderingEngineTypeDef](./type_defs.md#renderingenginetypedef)
- `tags`: `Mapping`\[`str`, `str`\]
- `environment`: [EnvironmentTypeDef](./type_defs.md#environmenttypedef)

Returns a `Coroutine` for
[CreateSimulationApplicationResponseTypeDef](./type_defs.md#createsimulationapplicationresponsetypedef).

<a id="create\_simulation\_application\_version"></a>

### create_simulation_application_version

Creates a simulation application with a specific revision id.

Type annotations for
`session.create_client("robomaker").create_simulation_application_version`
method.

Boto3 documentation:
[RoboMaker.Client.create_simulation_application_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_application_version)

Asynchronous method. Use `await create_simulation_application_version(...)` for
a synchronous call.

Arguments mapping described in
[CreateSimulationApplicationVersionRequestRequestTypeDef](./type_defs.md#createsimulationapplicationversionrequestrequesttypedef).

Keyword-only arguments:

- `application`: `str` *(required)*
- `currentRevisionId`: `str`
- `s3Etags`: `Sequence`\[`str`\]
- `imageDigest`: `str`

Returns a `Coroutine` for
[CreateSimulationApplicationVersionResponseTypeDef](./type_defs.md#createsimulationapplicationversionresponsetypedef).

<a id="create\_simulation\_job"></a>

### create_simulation_job

Creates a simulation job.

Type annotations for `session.create_client("robomaker").create_simulation_job`
method.

Boto3 documentation:
[RoboMaker.Client.create_simulation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_job)

Asynchronous method. Use `await create_simulation_job(...)` for a synchronous
call.

Arguments mapping described in
[CreateSimulationJobRequestRequestTypeDef](./type_defs.md#createsimulationjobrequestrequesttypedef).

Keyword-only arguments:

- `maxJobDurationInSeconds`: `int` *(required)*
- `iamRole`: `str` *(required)*
- `clientRequestToken`: `str`
- `outputLocation`:
  [OutputLocationTypeDef](./type_defs.md#outputlocationtypedef)
- `loggingConfig`: [LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef)
- `failureBehavior`: [FailureBehaviorType](./literals.md#failurebehaviortype)
- `robotApplications`:
  `Sequence`\[[RobotApplicationConfigTypeDef](./type_defs.md#robotapplicationconfigtypedef)\]
- `simulationApplications`:
  `Sequence`\[[SimulationApplicationConfigTypeDef](./type_defs.md#simulationapplicationconfigtypedef)\]
- `dataSources`:
  `Sequence`\[[DataSourceConfigTypeDef](./type_defs.md#datasourceconfigtypedef)\]
- `tags`: `Mapping`\[`str`, `str`\]
- `vpcConfig`: [VPCConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- `compute`: [ComputeTypeDef](./type_defs.md#computetypedef)

Returns a `Coroutine` for
[CreateSimulationJobResponseTypeDef](./type_defs.md#createsimulationjobresponsetypedef).

<a id="create\_world\_export\_job"></a>

### create_world_export_job

Creates a world export job.

Type annotations for
`session.create_client("robomaker").create_world_export_job` method.

Boto3 documentation:
[RoboMaker.Client.create_world_export_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_world_export_job)

Asynchronous method. Use `await create_world_export_job(...)` for a synchronous
call.

Arguments mapping described in
[CreateWorldExportJobRequestRequestTypeDef](./type_defs.md#createworldexportjobrequestrequesttypedef).

Keyword-only arguments:

- `worlds`: `Sequence`\[`str`\] *(required)*
- `outputLocation`:
  [OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) *(required)*
- `iamRole`: `str` *(required)*
- `clientRequestToken`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateWorldExportJobResponseTypeDef](./type_defs.md#createworldexportjobresponsetypedef).

<a id="create\_world\_generation\_job"></a>

### create_world_generation_job

Creates worlds using the specified template.

Type annotations for
`session.create_client("robomaker").create_world_generation_job` method.

Boto3 documentation:
[RoboMaker.Client.create_world_generation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_world_generation_job)

Asynchronous method. Use `await create_world_generation_job(...)` for a
synchronous call.

Arguments mapping described in
[CreateWorldGenerationJobRequestRequestTypeDef](./type_defs.md#createworldgenerationjobrequestrequesttypedef).

Keyword-only arguments:

- `template`: `str` *(required)*
- `worldCount`: [WorldCountTypeDef](./type_defs.md#worldcounttypedef)
  *(required)*
- `clientRequestToken`: `str`
- `tags`: `Mapping`\[`str`, `str`\]
- `worldTags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateWorldGenerationJobResponseTypeDef](./type_defs.md#createworldgenerationjobresponsetypedef).

<a id="create\_world\_template"></a>

### create_world_template

Creates a world template.

Type annotations for `session.create_client("robomaker").create_world_template`
method.

Boto3 documentation:
[RoboMaker.Client.create_world_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_world_template)

Asynchronous method. Use `await create_world_template(...)` for a synchronous
call.

Arguments mapping described in
[CreateWorldTemplateRequestRequestTypeDef](./type_defs.md#createworldtemplaterequestrequesttypedef).

Keyword-only arguments:

- `clientRequestToken`: `str`
- `name`: `str`
- `templateBody`: `str`
- `templateLocation`:
  [TemplateLocationTypeDef](./type_defs.md#templatelocationtypedef)
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateWorldTemplateResponseTypeDef](./type_defs.md#createworldtemplateresponsetypedef).

<a id="delete\_fleet"></a>

### delete_fleet

Deletes a fleet.

Type annotations for `session.create_client("robomaker").delete_fleet` method.

Boto3 documentation:
[RoboMaker.Client.delete_fleet](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.delete_fleet)

Asynchronous method. Use `await delete_fleet(...)` for a synchronous call.

Arguments mapping described in
[DeleteFleetRequestRequestTypeDef](./type_defs.md#deletefleetrequestrequesttypedef).

Keyword-only arguments:

- `fleet`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_robot"></a>

### delete_robot

Deletes a robot.

Type annotations for `session.create_client("robomaker").delete_robot` method.

Boto3 documentation:
[RoboMaker.Client.delete_robot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.delete_robot)

Asynchronous method. Use `await delete_robot(...)` for a synchronous call.

Arguments mapping described in
[DeleteRobotRequestRequestTypeDef](./type_defs.md#deleterobotrequestrequesttypedef).

Keyword-only arguments:

- `robot`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_robot\_application"></a>

### delete_robot_application

Deletes a robot application.

Type annotations for
`session.create_client("robomaker").delete_robot_application` method.

Boto3 documentation:
[RoboMaker.Client.delete_robot_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.delete_robot_application)

Asynchronous method. Use `await delete_robot_application(...)` for a
synchronous call.

Arguments mapping described in
[DeleteRobotApplicationRequestRequestTypeDef](./type_defs.md#deleterobotapplicationrequestrequesttypedef).

Keyword-only arguments:

- `application`: `str` *(required)*
- `applicationVersion`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_simulation\_application"></a>

### delete_simulation_application

Deletes a simulation application.

Type annotations for
`session.create_client("robomaker").delete_simulation_application` method.

Boto3 documentation:
[RoboMaker.Client.delete_simulation_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.delete_simulation_application)

Asynchronous method. Use `await delete_simulation_application(...)` for a
synchronous call.

Arguments mapping described in
[DeleteSimulationApplicationRequestRequestTypeDef](./type_defs.md#deletesimulationapplicationrequestrequesttypedef).

Keyword-only arguments:

- `application`: `str` *(required)*
- `applicationVersion`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_world\_template"></a>

### delete_world_template

Deletes a world template.

Type annotations for `session.create_client("robomaker").delete_world_template`
method.

Boto3 documentation:
[RoboMaker.Client.delete_world_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.delete_world_template)

Asynchronous method. Use `await delete_world_template(...)` for a synchronous
call.

Arguments mapping described in
[DeleteWorldTemplateRequestRequestTypeDef](./type_defs.md#deleteworldtemplaterequestrequesttypedef).

Keyword-only arguments:

- `template`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="deregister\_robot"></a>

### deregister_robot

Deregisters a robot.

Type annotations for `session.create_client("robomaker").deregister_robot`
method.

Boto3 documentation:
[RoboMaker.Client.deregister_robot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.deregister_robot)

Asynchronous method. Use `await deregister_robot(...)` for a synchronous call.

Arguments mapping described in
[DeregisterRobotRequestRequestTypeDef](./type_defs.md#deregisterrobotrequestrequesttypedef).

Keyword-only arguments:

- `fleet`: `str` *(required)*
- `robot`: `str` *(required)*

Returns a `Coroutine` for
[DeregisterRobotResponseTypeDef](./type_defs.md#deregisterrobotresponsetypedef).

<a id="describe\_deployment\_job"></a>

### describe_deployment_job

Describes a deployment job.

Type annotations for
`session.create_client("robomaker").describe_deployment_job` method.

Boto3 documentation:
[RoboMaker.Client.describe_deployment_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.describe_deployment_job)

Asynchronous method. Use `await describe_deployment_job(...)` for a synchronous
call.

Arguments mapping described in
[DescribeDeploymentJobRequestRequestTypeDef](./type_defs.md#describedeploymentjobrequestrequesttypedef).

Keyword-only arguments:

- `job`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDeploymentJobResponseTypeDef](./type_defs.md#describedeploymentjobresponsetypedef).

<a id="describe\_fleet"></a>

### describe_fleet

Describes a fleet.

Type annotations for `session.create_client("robomaker").describe_fleet`
method.

Boto3 documentation:
[RoboMaker.Client.describe_fleet](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.describe_fleet)

Asynchronous method. Use `await describe_fleet(...)` for a synchronous call.

Arguments mapping described in
[DescribeFleetRequestRequestTypeDef](./type_defs.md#describefleetrequestrequesttypedef).

Keyword-only arguments:

- `fleet`: `str` *(required)*

Returns a `Coroutine` for
[DescribeFleetResponseTypeDef](./type_defs.md#describefleetresponsetypedef).

<a id="describe\_robot"></a>

### describe_robot

Describes a robot.

Type annotations for `session.create_client("robomaker").describe_robot`
method.

Boto3 documentation:
[RoboMaker.Client.describe_robot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.describe_robot)

Asynchronous method. Use `await describe_robot(...)` for a synchronous call.

Arguments mapping described in
[DescribeRobotRequestRequestTypeDef](./type_defs.md#describerobotrequestrequesttypedef).

Keyword-only arguments:

- `robot`: `str` *(required)*

Returns a `Coroutine` for
[DescribeRobotResponseTypeDef](./type_defs.md#describerobotresponsetypedef).

<a id="describe\_robot\_application"></a>

### describe_robot_application

Describes a robot application.

Type annotations for
`session.create_client("robomaker").describe_robot_application` method.

Boto3 documentation:
[RoboMaker.Client.describe_robot_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.describe_robot_application)

Asynchronous method. Use `await describe_robot_application(...)` for a
synchronous call.

Arguments mapping described in
[DescribeRobotApplicationRequestRequestTypeDef](./type_defs.md#describerobotapplicationrequestrequesttypedef).

Keyword-only arguments:

- `application`: `str` *(required)*
- `applicationVersion`: `str`

Returns a `Coroutine` for
[DescribeRobotApplicationResponseTypeDef](./type_defs.md#describerobotapplicationresponsetypedef).

<a id="describe\_simulation\_application"></a>

### describe_simulation_application

Describes a simulation application.

Type annotations for
`session.create_client("robomaker").describe_simulation_application` method.

Boto3 documentation:
[RoboMaker.Client.describe_simulation_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.describe_simulation_application)

Asynchronous method. Use `await describe_simulation_application(...)` for a
synchronous call.

Arguments mapping described in
[DescribeSimulationApplicationRequestRequestTypeDef](./type_defs.md#describesimulationapplicationrequestrequesttypedef).

Keyword-only arguments:

- `application`: `str` *(required)*
- `applicationVersion`: `str`

Returns a `Coroutine` for
[DescribeSimulationApplicationResponseTypeDef](./type_defs.md#describesimulationapplicationresponsetypedef).

<a id="describe\_simulation\_job"></a>

### describe_simulation_job

Describes a simulation job.

Type annotations for
`session.create_client("robomaker").describe_simulation_job` method.

Boto3 documentation:
[RoboMaker.Client.describe_simulation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.describe_simulation_job)

Asynchronous method. Use `await describe_simulation_job(...)` for a synchronous
call.

Arguments mapping described in
[DescribeSimulationJobRequestRequestTypeDef](./type_defs.md#describesimulationjobrequestrequesttypedef).

Keyword-only arguments:

- `job`: `str` *(required)*

Returns a `Coroutine` for
[DescribeSimulationJobResponseTypeDef](./type_defs.md#describesimulationjobresponsetypedef).

<a id="describe\_simulation\_job\_batch"></a>

### describe_simulation_job_batch

Describes a simulation job batch.

Type annotations for
`session.create_client("robomaker").describe_simulation_job_batch` method.

Boto3 documentation:
[RoboMaker.Client.describe_simulation_job_batch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.describe_simulation_job_batch)

Asynchronous method. Use `await describe_simulation_job_batch(...)` for a
synchronous call.

Arguments mapping described in
[DescribeSimulationJobBatchRequestRequestTypeDef](./type_defs.md#describesimulationjobbatchrequestrequesttypedef).

Keyword-only arguments:

- `batch`: `str` *(required)*

Returns a `Coroutine` for
[DescribeSimulationJobBatchResponseTypeDef](./type_defs.md#describesimulationjobbatchresponsetypedef).

<a id="describe\_world"></a>

### describe_world

Describes a world.

Type annotations for `session.create_client("robomaker").describe_world`
method.

Boto3 documentation:
[RoboMaker.Client.describe_world](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.describe_world)

Asynchronous method. Use `await describe_world(...)` for a synchronous call.

Arguments mapping described in
[DescribeWorldRequestRequestTypeDef](./type_defs.md#describeworldrequestrequesttypedef).

Keyword-only arguments:

- `world`: `str` *(required)*

Returns a `Coroutine` for
[DescribeWorldResponseTypeDef](./type_defs.md#describeworldresponsetypedef).

<a id="describe\_world\_export\_job"></a>

### describe_world_export_job

Describes a world export job.

Type annotations for
`session.create_client("robomaker").describe_world_export_job` method.

Boto3 documentation:
[RoboMaker.Client.describe_world_export_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.describe_world_export_job)

Asynchronous method. Use `await describe_world_export_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeWorldExportJobRequestRequestTypeDef](./type_defs.md#describeworldexportjobrequestrequesttypedef).

Keyword-only arguments:

- `job`: `str` *(required)*

Returns a `Coroutine` for
[DescribeWorldExportJobResponseTypeDef](./type_defs.md#describeworldexportjobresponsetypedef).

<a id="describe\_world\_generation\_job"></a>

### describe_world_generation_job

Describes a world generation job.

Type annotations for
`session.create_client("robomaker").describe_world_generation_job` method.

Boto3 documentation:
[RoboMaker.Client.describe_world_generation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.describe_world_generation_job)

Asynchronous method. Use `await describe_world_generation_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeWorldGenerationJobRequestRequestTypeDef](./type_defs.md#describeworldgenerationjobrequestrequesttypedef).

Keyword-only arguments:

- `job`: `str` *(required)*

Returns a `Coroutine` for
[DescribeWorldGenerationJobResponseTypeDef](./type_defs.md#describeworldgenerationjobresponsetypedef).

<a id="describe\_world\_template"></a>

### describe_world_template

Describes a world template.

Type annotations for
`session.create_client("robomaker").describe_world_template` method.

Boto3 documentation:
[RoboMaker.Client.describe_world_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.describe_world_template)

Asynchronous method. Use `await describe_world_template(...)` for a synchronous
call.

Arguments mapping described in
[DescribeWorldTemplateRequestRequestTypeDef](./type_defs.md#describeworldtemplaterequestrequesttypedef).

Keyword-only arguments:

- `template`: `str` *(required)*

Returns a `Coroutine` for
[DescribeWorldTemplateResponseTypeDef](./type_defs.md#describeworldtemplateresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("robomaker").generate_presigned_url` method.

Boto3 documentation:
[RoboMaker.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_world\_template\_body"></a>

### get_world_template_body

Gets the world template body.

Type annotations for
`session.create_client("robomaker").get_world_template_body` method.

Boto3 documentation:
[RoboMaker.Client.get_world_template_body](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.get_world_template_body)

Asynchronous method. Use `await get_world_template_body(...)` for a synchronous
call.

Arguments mapping described in
[GetWorldTemplateBodyRequestRequestTypeDef](./type_defs.md#getworldtemplatebodyrequestrequesttypedef).

Keyword-only arguments:

- `template`: `str`
- `generationJob`: `str`

Returns a `Coroutine` for
[GetWorldTemplateBodyResponseTypeDef](./type_defs.md#getworldtemplatebodyresponsetypedef).

<a id="list\_deployment\_jobs"></a>

### list_deployment_jobs

Returns a list of deployment jobs for a fleet.

Type annotations for `session.create_client("robomaker").list_deployment_jobs`
method.

Boto3 documentation:
[RoboMaker.Client.list_deployment_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_deployment_jobs)

Asynchronous method. Use `await list_deployment_jobs(...)` for a synchronous
call.

Arguments mapping described in
[ListDeploymentJobsRequestRequestTypeDef](./type_defs.md#listdeploymentjobsrequestrequesttypedef).

Keyword-only arguments:

- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListDeploymentJobsResponseTypeDef](./type_defs.md#listdeploymentjobsresponsetypedef).

<a id="list\_fleets"></a>

### list_fleets

Returns a list of fleets.

Type annotations for `session.create_client("robomaker").list_fleets` method.

Boto3 documentation:
[RoboMaker.Client.list_fleets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_fleets)

Asynchronous method. Use `await list_fleets(...)` for a synchronous call.

Arguments mapping described in
[ListFleetsRequestRequestTypeDef](./type_defs.md#listfleetsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListFleetsResponseTypeDef](./type_defs.md#listfleetsresponsetypedef).

<a id="list\_robot\_applications"></a>

### list_robot_applications

Returns a list of robot application.

Type annotations for
`session.create_client("robomaker").list_robot_applications` method.

Boto3 documentation:
[RoboMaker.Client.list_robot_applications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_robot_applications)

Asynchronous method. Use `await list_robot_applications(...)` for a synchronous
call.

Arguments mapping described in
[ListRobotApplicationsRequestRequestTypeDef](./type_defs.md#listrobotapplicationsrequestrequesttypedef).

Keyword-only arguments:

- `versionQualifier`: `str`
- `nextToken`: `str`
- `maxResults`: `int`
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListRobotApplicationsResponseTypeDef](./type_defs.md#listrobotapplicationsresponsetypedef).

<a id="list\_robots"></a>

### list_robots

Returns a list of robots.

Type annotations for `session.create_client("robomaker").list_robots` method.

Boto3 documentation:
[RoboMaker.Client.list_robots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_robots)

Asynchronous method. Use `await list_robots(...)` for a synchronous call.

Arguments mapping described in
[ListRobotsRequestRequestTypeDef](./type_defs.md#listrobotsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListRobotsResponseTypeDef](./type_defs.md#listrobotsresponsetypedef).

<a id="list\_simulation\_applications"></a>

### list_simulation_applications

Returns a list of simulation applications.

Type annotations for
`session.create_client("robomaker").list_simulation_applications` method.

Boto3 documentation:
[RoboMaker.Client.list_simulation_applications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_simulation_applications)

Asynchronous method. Use `await list_simulation_applications(...)` for a
synchronous call.

Arguments mapping described in
[ListSimulationApplicationsRequestRequestTypeDef](./type_defs.md#listsimulationapplicationsrequestrequesttypedef).

Keyword-only arguments:

- `versionQualifier`: `str`
- `nextToken`: `str`
- `maxResults`: `int`
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListSimulationApplicationsResponseTypeDef](./type_defs.md#listsimulationapplicationsresponsetypedef).

<a id="list\_simulation\_job\_batches"></a>

### list_simulation_job_batches

Returns a list simulation job batches.

Type annotations for
`session.create_client("robomaker").list_simulation_job_batches` method.

Boto3 documentation:
[RoboMaker.Client.list_simulation_job_batches](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_simulation_job_batches)

Asynchronous method. Use `await list_simulation_job_batches(...)` for a
synchronous call.

Arguments mapping described in
[ListSimulationJobBatchesRequestRequestTypeDef](./type_defs.md#listsimulationjobbatchesrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListSimulationJobBatchesResponseTypeDef](./type_defs.md#listsimulationjobbatchesresponsetypedef).

<a id="list\_simulation\_jobs"></a>

### list_simulation_jobs

Returns a list of simulation jobs.

Type annotations for `session.create_client("robomaker").list_simulation_jobs`
method.

Boto3 documentation:
[RoboMaker.Client.list_simulation_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_simulation_jobs)

Asynchronous method. Use `await list_simulation_jobs(...)` for a synchronous
call.

Arguments mapping described in
[ListSimulationJobsRequestRequestTypeDef](./type_defs.md#listsimulationjobsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListSimulationJobsResponseTypeDef](./type_defs.md#listsimulationjobsresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Lists all tags on a AWS RoboMaker resource.

Type annotations for
`session.create_client("robomaker").list_tags_for_resource` method.

Boto3 documentation:
[RoboMaker.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="list\_world\_export\_jobs"></a>

### list_world_export_jobs

Lists world export jobs.

Type annotations for
`session.create_client("robomaker").list_world_export_jobs` method.

Boto3 documentation:
[RoboMaker.Client.list_world_export_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_world_export_jobs)

Asynchronous method. Use `await list_world_export_jobs(...)` for a synchronous
call.

Arguments mapping described in
[ListWorldExportJobsRequestRequestTypeDef](./type_defs.md#listworldexportjobsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListWorldExportJobsResponseTypeDef](./type_defs.md#listworldexportjobsresponsetypedef).

<a id="list\_world\_generation\_jobs"></a>

### list_world_generation_jobs

Lists world generator jobs.

Type annotations for
`session.create_client("robomaker").list_world_generation_jobs` method.

Boto3 documentation:
[RoboMaker.Client.list_world_generation_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_world_generation_jobs)

Asynchronous method. Use `await list_world_generation_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListWorldGenerationJobsRequestRequestTypeDef](./type_defs.md#listworldgenerationjobsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListWorldGenerationJobsResponseTypeDef](./type_defs.md#listworldgenerationjobsresponsetypedef).

<a id="list\_world\_templates"></a>

### list_world_templates

Lists world templates.

Type annotations for `session.create_client("robomaker").list_world_templates`
method.

Boto3 documentation:
[RoboMaker.Client.list_world_templates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_world_templates)

Asynchronous method. Use `await list_world_templates(...)` for a synchronous
call.

Arguments mapping described in
[ListWorldTemplatesRequestRequestTypeDef](./type_defs.md#listworldtemplatesrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListWorldTemplatesResponseTypeDef](./type_defs.md#listworldtemplatesresponsetypedef).

<a id="list\_worlds"></a>

### list_worlds

Lists worlds.

Type annotations for `session.create_client("robomaker").list_worlds` method.

Boto3 documentation:
[RoboMaker.Client.list_worlds](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.list_worlds)

Asynchronous method. Use `await list_worlds(...)` for a synchronous call.

Arguments mapping described in
[ListWorldsRequestRequestTypeDef](./type_defs.md#listworldsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListWorldsResponseTypeDef](./type_defs.md#listworldsresponsetypedef).

<a id="register\_robot"></a>

### register_robot

Registers a robot with a fleet.

Type annotations for `session.create_client("robomaker").register_robot`
method.

Boto3 documentation:
[RoboMaker.Client.register_robot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.register_robot)

Asynchronous method. Use `await register_robot(...)` for a synchronous call.

Arguments mapping described in
[RegisterRobotRequestRequestTypeDef](./type_defs.md#registerrobotrequestrequesttypedef).

Keyword-only arguments:

- `fleet`: `str` *(required)*
- `robot`: `str` *(required)*

Returns a `Coroutine` for
[RegisterRobotResponseTypeDef](./type_defs.md#registerrobotresponsetypedef).

<a id="restart\_simulation\_job"></a>

### restart_simulation_job

Restarts a running simulation job.

Type annotations for
`session.create_client("robomaker").restart_simulation_job` method.

Boto3 documentation:
[RoboMaker.Client.restart_simulation_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.restart_simulation_job)

Asynchronous method. Use `await restart_simulation_job(...)` for a synchronous
call.

Arguments mapping described in
[RestartSimulationJobRequestRequestTypeDef](./type_defs.md#restartsimulationjobrequestrequesttypedef).

Keyword-only arguments:

- `job`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="start\_simulation\_job\_batch"></a>

### start_simulation_job_batch

Starts a new simulation job batch.

Type annotations for
`session.create_client("robomaker").start_simulation_job_batch` method.

Boto3 documentation:
[RoboMaker.Client.start_simulation_job_batch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.start_simulation_job_batch)

Asynchronous method. Use `await start_simulation_job_batch(...)` for a
synchronous call.

Arguments mapping described in
[StartSimulationJobBatchRequestRequestTypeDef](./type_defs.md#startsimulationjobbatchrequestrequesttypedef).

Keyword-only arguments:

- `createSimulationJobRequests`:
  `Sequence`\[[SimulationJobRequestTypeDef](./type_defs.md#simulationjobrequesttypedef)\]
  *(required)*
- `clientRequestToken`: `str`
- `batchPolicy`: [BatchPolicyTypeDef](./type_defs.md#batchpolicytypedef)
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[StartSimulationJobBatchResponseTypeDef](./type_defs.md#startsimulationjobbatchresponsetypedef).

<a id="sync\_deployment\_job"></a>

### sync_deployment_job

Syncrhonizes robots in a fleet to the latest deployment.

Type annotations for `session.create_client("robomaker").sync_deployment_job`
method.

Boto3 documentation:
[RoboMaker.Client.sync_deployment_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.sync_deployment_job)

Asynchronous method. Use `await sync_deployment_job(...)` for a synchronous
call.

Arguments mapping described in
[SyncDeploymentJobRequestRequestTypeDef](./type_defs.md#syncdeploymentjobrequestrequesttypedef).

Keyword-only arguments:

- `clientRequestToken`: `str` *(required)*
- `fleet`: `str` *(required)*

Returns a `Coroutine` for
[SyncDeploymentJobResponseTypeDef](./type_defs.md#syncdeploymentjobresponsetypedef).

<a id="tag\_resource"></a>

### tag_resource

Adds or edits tags for a AWS RoboMaker resource.

Type annotations for `session.create_client("robomaker").tag_resource` method.

Boto3 documentation:
[RoboMaker.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

.

Type annotations for `session.create_client("robomaker").untag_resource`
method.

Boto3 documentation:
[RoboMaker.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_robot\_application"></a>

### update_robot_application

Updates a robot application.

Type annotations for
`session.create_client("robomaker").update_robot_application` method.

Boto3 documentation:
[RoboMaker.Client.update_robot_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.update_robot_application)

Asynchronous method. Use `await update_robot_application(...)` for a
synchronous call.

Arguments mapping described in
[UpdateRobotApplicationRequestRequestTypeDef](./type_defs.md#updaterobotapplicationrequestrequesttypedef).

Keyword-only arguments:

- `application`: `str` *(required)*
- `robotSoftwareSuite`:
  [RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef)
  *(required)*
- `sources`:
  `Sequence`\[[SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef)\]
- `currentRevisionId`: `str`
- `environment`: [EnvironmentTypeDef](./type_defs.md#environmenttypedef)

Returns a `Coroutine` for
[UpdateRobotApplicationResponseTypeDef](./type_defs.md#updaterobotapplicationresponsetypedef).

<a id="update\_simulation\_application"></a>

### update_simulation_application

Updates a simulation application.

Type annotations for
`session.create_client("robomaker").update_simulation_application` method.

Boto3 documentation:
[RoboMaker.Client.update_simulation_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.update_simulation_application)

Asynchronous method. Use `await update_simulation_application(...)` for a
synchronous call.

Arguments mapping described in
[UpdateSimulationApplicationRequestRequestTypeDef](./type_defs.md#updatesimulationapplicationrequestrequesttypedef).

Keyword-only arguments:

- `application`: `str` *(required)*
- `simulationSoftwareSuite`:
  [SimulationSoftwareSuiteTypeDef](./type_defs.md#simulationsoftwaresuitetypedef)
  *(required)*
- `robotSoftwareSuite`:
  [RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef)
  *(required)*
- `sources`:
  `Sequence`\[[SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef)\]
- `renderingEngine`:
  [RenderingEngineTypeDef](./type_defs.md#renderingenginetypedef)
- `currentRevisionId`: `str`
- `environment`: [EnvironmentTypeDef](./type_defs.md#environmenttypedef)

Returns a `Coroutine` for
[UpdateSimulationApplicationResponseTypeDef](./type_defs.md#updatesimulationapplicationresponsetypedef).

<a id="update\_world\_template"></a>

### update_world_template

Updates a world template.

Type annotations for `session.create_client("robomaker").update_world_template`
method.

Boto3 documentation:
[RoboMaker.Client.update_world_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.update_world_template)

Asynchronous method. Use `await update_world_template(...)` for a synchronous
call.

Arguments mapping described in
[UpdateWorldTemplateRequestRequestTypeDef](./type_defs.md#updateworldtemplaterequestrequesttypedef).

Keyword-only arguments:

- `template`: `str` *(required)*
- `name`: `str`
- `templateBody`: `str`
- `templateLocation`:
  [TemplateLocationTypeDef](./type_defs.md#templatelocationtypedef)

Returns a `Coroutine` for
[UpdateWorldTemplateResponseTypeDef](./type_defs.md#updateworldtemplateresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("robomaker").__aenter__` method.

Boto3 documentation:
[RoboMaker.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [RoboMakerClient](#robomakerclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("robomaker").__aexit__` method.

Boto3 documentation:
[RoboMaker.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("robomaker").get_paginator` method
with overloads.

- `client.get_paginator("list_deployment_jobs")` ->
  [ListDeploymentJobsPaginator](./paginators.md#listdeploymentjobspaginator)
- `client.get_paginator("list_fleets")` ->
  [ListFleetsPaginator](./paginators.md#listfleetspaginator)
- `client.get_paginator("list_robot_applications")` ->
  [ListRobotApplicationsPaginator](./paginators.md#listrobotapplicationspaginator)
- `client.get_paginator("list_robots")` ->
  [ListRobotsPaginator](./paginators.md#listrobotspaginator)
- `client.get_paginator("list_simulation_applications")` ->
  [ListSimulationApplicationsPaginator](./paginators.md#listsimulationapplicationspaginator)
- `client.get_paginator("list_simulation_job_batches")` ->
  [ListSimulationJobBatchesPaginator](./paginators.md#listsimulationjobbatchespaginator)
- `client.get_paginator("list_simulation_jobs")` ->
  [ListSimulationJobsPaginator](./paginators.md#listsimulationjobspaginator)
- `client.get_paginator("list_world_export_jobs")` ->
  [ListWorldExportJobsPaginator](./paginators.md#listworldexportjobspaginator)
- `client.get_paginator("list_world_generation_jobs")` ->
  [ListWorldGenerationJobsPaginator](./paginators.md#listworldgenerationjobspaginator)
- `client.get_paginator("list_world_templates")` ->
  [ListWorldTemplatesPaginator](./paginators.md#listworldtemplatespaginator)
- `client.get_paginator("list_worlds")` ->
  [ListWorldsPaginator](./paginators.md#listworldspaginator)
