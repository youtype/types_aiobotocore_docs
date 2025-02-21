# RoboMakerClient

> [Index](../README.md) > [RoboMaker](./README.md) > RoboMakerClient

!!! note ""

    Auto-generated documentation for [RoboMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#robomaker)
    type annotations stubs module [types-aiobotocore-robomaker](https://pypi.org/project/types-aiobotocore-robomaker/).

## RoboMakerClient

Type annotations and code completion for `#!python session.create_client("robomaker")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client)

```python
# RoboMakerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_robomaker.client import RoboMakerClient

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("robomaker").exceptions` structure.

```python
# RoboMakerClient.exceptions usage example

async with session.create_client("robomaker") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConcurrentDeploymentException,
        client.IdempotentParameterMismatchException,
        client.InternalServerException,
        client.InvalidParameterException,
        client.LimitExceededException,
        client.ResourceAlreadyExistsException,
        client.ResourceNotFoundException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python
# RoboMakerClient usage type checking example

from types_aiobotocore_robomaker.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("robomaker").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("robomaker").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/generate_presigned_url.html)

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


### batch\_delete\_worlds

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").batch_delete_worlds` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/batch_delete_worlds.html)

```python
# batch_delete_worlds method definition

await def batch_delete_worlds(
    self,
    *,
    worlds: Sequence[str],
) -> BatchDeleteWorldsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteWorldsResponseTypeDef](./type_defs.md#batchdeleteworldsresponsetypedef) 


```python
# batch_delete_worlds method usage example with argument unpacking

kwargs: BatchDeleteWorldsRequestTypeDef = {  # (1)
    "worlds": ...,
}

parent.batch_delete_worlds(**kwargs)
```

1. See [:material-code-braces: BatchDeleteWorldsRequestTypeDef](./type_defs.md#batchdeleteworldsrequesttypedef) 

### batch\_describe\_simulation\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").batch_describe_simulation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/batch_describe_simulation_job.html)

```python
# batch_describe_simulation_job method definition

await def batch_describe_simulation_job(
    self,
    *,
    jobs: Sequence[str],
) -> BatchDescribeSimulationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDescribeSimulationJobResponseTypeDef](./type_defs.md#batchdescribesimulationjobresponsetypedef) 


```python
# batch_describe_simulation_job method usage example with argument unpacking

kwargs: BatchDescribeSimulationJobRequestTypeDef = {  # (1)
    "jobs": ...,
}

parent.batch_describe_simulation_job(**kwargs)
```

1. See [:material-code-braces: BatchDescribeSimulationJobRequestTypeDef](./type_defs.md#batchdescribesimulationjobrequesttypedef) 

### cancel\_deployment\_job

This API is no longer supported.

Type annotations and code completion for `#!python session.create_client("robomaker").cancel_deployment_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/cancel_deployment_job.html)

```python
# cancel_deployment_job method definition

await def cancel_deployment_job(
    self,
    *,
    job: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_deployment_job method usage example with argument unpacking

kwargs: CancelDeploymentJobRequestTypeDef = {  # (1)
    "job": ...,
}

parent.cancel_deployment_job(**kwargs)
```

1. See [:material-code-braces: CancelDeploymentJobRequestTypeDef](./type_defs.md#canceldeploymentjobrequesttypedef) 

### cancel\_simulation\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").cancel_simulation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/cancel_simulation_job.html)

```python
# cancel_simulation_job method definition

await def cancel_simulation_job(
    self,
    *,
    job: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_simulation_job method usage example with argument unpacking

kwargs: CancelSimulationJobRequestTypeDef = {  # (1)
    "job": ...,
}

parent.cancel_simulation_job(**kwargs)
```

1. See [:material-code-braces: CancelSimulationJobRequestTypeDef](./type_defs.md#cancelsimulationjobrequesttypedef) 

### cancel\_simulation\_job\_batch

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").cancel_simulation_job_batch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/cancel_simulation_job_batch.html)

```python
# cancel_simulation_job_batch method definition

await def cancel_simulation_job_batch(
    self,
    *,
    batch: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_simulation_job_batch method usage example with argument unpacking

kwargs: CancelSimulationJobBatchRequestTypeDef = {  # (1)
    "batch": ...,
}

parent.cancel_simulation_job_batch(**kwargs)
```

1. See [:material-code-braces: CancelSimulationJobBatchRequestTypeDef](./type_defs.md#cancelsimulationjobbatchrequesttypedef) 

### cancel\_world\_export\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").cancel_world_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/cancel_world_export_job.html)

```python
# cancel_world_export_job method definition

await def cancel_world_export_job(
    self,
    *,
    job: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_world_export_job method usage example with argument unpacking

kwargs: CancelWorldExportJobRequestTypeDef = {  # (1)
    "job": ...,
}

parent.cancel_world_export_job(**kwargs)
```

1. See [:material-code-braces: CancelWorldExportJobRequestTypeDef](./type_defs.md#cancelworldexportjobrequesttypedef) 

### cancel\_world\_generation\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").cancel_world_generation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/cancel_world_generation_job.html)

```python
# cancel_world_generation_job method definition

await def cancel_world_generation_job(
    self,
    *,
    job: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_world_generation_job method usage example with argument unpacking

kwargs: CancelWorldGenerationJobRequestTypeDef = {  # (1)
    "job": ...,
}

parent.cancel_world_generation_job(**kwargs)
```

1. See [:material-code-braces: CancelWorldGenerationJobRequestTypeDef](./type_defs.md#cancelworldgenerationjobrequesttypedef) 

### create\_deployment\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").create_deployment_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/create_deployment_job.html)

```python
# create_deployment_job method definition

await def create_deployment_job(
    self,
    *,
    clientRequestToken: str,
    fleet: str,
    deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigUnionTypeDef],  # (1)
    deploymentConfig: DeploymentConfigTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
) -> CreateDeploymentJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DeploymentApplicationConfigTypeDef](./type_defs.md#deploymentapplicationconfigtypedef) [:material-code-braces: DeploymentApplicationConfigOutputTypeDef](./type_defs.md#deploymentapplicationconfigoutputtypedef) 
2. See [:material-code-braces: DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef) 
3. See [:material-code-braces: CreateDeploymentJobResponseTypeDef](./type_defs.md#createdeploymentjobresponsetypedef) 


```python
# create_deployment_job method usage example with argument unpacking

kwargs: CreateDeploymentJobRequestTypeDef = {  # (1)
    "clientRequestToken": ...,
    "fleet": ...,
    "deploymentApplicationConfigs": ...,
}

parent.create_deployment_job(**kwargs)
```

1. See [:material-code-braces: CreateDeploymentJobRequestTypeDef](./type_defs.md#createdeploymentjobrequesttypedef) 

### create\_fleet

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").create_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/create_fleet.html)

```python
# create_fleet method definition

await def create_fleet(
    self,
    *,
    name: str,
    tags: Mapping[str, str] = ...,
) -> CreateFleetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateFleetResponseTypeDef](./type_defs.md#createfleetresponsetypedef) 


```python
# create_fleet method usage example with argument unpacking

kwargs: CreateFleetRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_fleet(**kwargs)
```

1. See [:material-code-braces: CreateFleetRequestTypeDef](./type_defs.md#createfleetrequesttypedef) 

### create\_robot

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").create_robot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/create_robot.html)

```python
# create_robot method definition

await def create_robot(
    self,
    *,
    name: str,
    architecture: ArchitectureType,  # (1)
    greengrassGroupId: str,
    tags: Mapping[str, str] = ...,
) -> CreateRobotResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
2. See [:material-code-braces: CreateRobotResponseTypeDef](./type_defs.md#createrobotresponsetypedef) 


```python
# create_robot method usage example with argument unpacking

kwargs: CreateRobotRequestTypeDef = {  # (1)
    "name": ...,
    "architecture": ...,
    "greengrassGroupId": ...,
}

parent.create_robot(**kwargs)
```

1. See [:material-code-braces: CreateRobotRequestTypeDef](./type_defs.md#createrobotrequesttypedef) 

### create\_robot\_application

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").create_robot_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/create_robot_application.html)

```python
# create_robot_application method definition

await def create_robot_application(
    self,
    *,
    name: str,
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (1)
    sources: Sequence[SourceConfigTypeDef] = ...,  # (2)
    tags: Mapping[str, str] = ...,
    environment: EnvironmentTypeDef = ...,  # (3)
) -> CreateRobotApplicationResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
2. See [:material-code-braces: SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef) 
3. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
4. See [:material-code-braces: CreateRobotApplicationResponseTypeDef](./type_defs.md#createrobotapplicationresponsetypedef) 


```python
# create_robot_application method usage example with argument unpacking

kwargs: CreateRobotApplicationRequestTypeDef = {  # (1)
    "name": ...,
    "robotSoftwareSuite": ...,
}

parent.create_robot_application(**kwargs)
```

1. See [:material-code-braces: CreateRobotApplicationRequestTypeDef](./type_defs.md#createrobotapplicationrequesttypedef) 

### create\_robot\_application\_version

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").create_robot_application_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/create_robot_application_version.html)

```python
# create_robot_application_version method definition

await def create_robot_application_version(
    self,
    *,
    application: str,
    currentRevisionId: str = ...,
    s3Etags: Sequence[str] = ...,
    imageDigest: str = ...,
) -> CreateRobotApplicationVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateRobotApplicationVersionResponseTypeDef](./type_defs.md#createrobotapplicationversionresponsetypedef) 


```python
# create_robot_application_version method usage example with argument unpacking

kwargs: CreateRobotApplicationVersionRequestTypeDef = {  # (1)
    "application": ...,
}

parent.create_robot_application_version(**kwargs)
```

1. See [:material-code-braces: CreateRobotApplicationVersionRequestTypeDef](./type_defs.md#createrobotapplicationversionrequesttypedef) 

### create\_simulation\_application

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").create_simulation_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/create_simulation_application.html)

```python
# create_simulation_application method definition

await def create_simulation_application(
    self,
    *,
    name: str,
    simulationSoftwareSuite: SimulationSoftwareSuiteTypeDef,  # (1)
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (2)
    sources: Sequence[SourceConfigTypeDef] = ...,  # (3)
    renderingEngine: RenderingEngineTypeDef = ...,  # (4)
    tags: Mapping[str, str] = ...,
    environment: EnvironmentTypeDef = ...,  # (5)
) -> CreateSimulationApplicationResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: SimulationSoftwareSuiteTypeDef](./type_defs.md#simulationsoftwaresuitetypedef) 
2. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
3. See [:material-code-braces: SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef) 
4. See [:material-code-braces: RenderingEngineTypeDef](./type_defs.md#renderingenginetypedef) 
5. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
6. See [:material-code-braces: CreateSimulationApplicationResponseTypeDef](./type_defs.md#createsimulationapplicationresponsetypedef) 


```python
# create_simulation_application method usage example with argument unpacking

kwargs: CreateSimulationApplicationRequestTypeDef = {  # (1)
    "name": ...,
    "simulationSoftwareSuite": ...,
    "robotSoftwareSuite": ...,
}

parent.create_simulation_application(**kwargs)
```

1. See [:material-code-braces: CreateSimulationApplicationRequestTypeDef](./type_defs.md#createsimulationapplicationrequesttypedef) 

### create\_simulation\_application\_version

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").create_simulation_application_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/create_simulation_application_version.html)

```python
# create_simulation_application_version method definition

await def create_simulation_application_version(
    self,
    *,
    application: str,
    currentRevisionId: str = ...,
    s3Etags: Sequence[str] = ...,
    imageDigest: str = ...,
) -> CreateSimulationApplicationVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSimulationApplicationVersionResponseTypeDef](./type_defs.md#createsimulationapplicationversionresponsetypedef) 


```python
# create_simulation_application_version method usage example with argument unpacking

kwargs: CreateSimulationApplicationVersionRequestTypeDef = {  # (1)
    "application": ...,
}

parent.create_simulation_application_version(**kwargs)
```

1. See [:material-code-braces: CreateSimulationApplicationVersionRequestTypeDef](./type_defs.md#createsimulationapplicationversionrequesttypedef) 

### create\_simulation\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").create_simulation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/create_simulation_job.html)

```python
# create_simulation_job method definition

await def create_simulation_job(
    self,
    *,
    maxJobDurationInSeconds: int,
    iamRole: str,
    clientRequestToken: str = ...,
    outputLocation: OutputLocationTypeDef = ...,  # (1)
    loggingConfig: LoggingConfigTypeDef = ...,  # (2)
    failureBehavior: FailureBehaviorType = ...,  # (3)
    robotApplications: Sequence[RobotApplicationConfigUnionTypeDef] = ...,  # (4)
    simulationApplications: Sequence[SimulationApplicationConfigUnionTypeDef] = ...,  # (5)
    dataSources: Sequence[DataSourceConfigUnionTypeDef] = ...,  # (6)
    tags: Mapping[str, str] = ...,
    vpcConfig: VPCConfigUnionTypeDef = ...,  # (7)
    compute: ComputeTypeDef = ...,  # (8)
) -> CreateSimulationJobResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
2. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
3. See [:material-code-brackets: FailureBehaviorType](./literals.md#failurebehaviortype) 
4. See [:material-code-braces: RobotApplicationConfigTypeDef](./type_defs.md#robotapplicationconfigtypedef) [:material-code-braces: RobotApplicationConfigOutputTypeDef](./type_defs.md#robotapplicationconfigoutputtypedef) 
5. See [:material-code-braces: SimulationApplicationConfigTypeDef](./type_defs.md#simulationapplicationconfigtypedef) [:material-code-braces: SimulationApplicationConfigOutputTypeDef](./type_defs.md#simulationapplicationconfigoutputtypedef) 
6. See [:material-code-braces: DataSourceConfigTypeDef](./type_defs.md#datasourceconfigtypedef) [:material-code-braces: DataSourceConfigOutputTypeDef](./type_defs.md#datasourceconfigoutputtypedef) 
7. See [:material-code-braces: VPCConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VPCConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
8. See [:material-code-braces: ComputeTypeDef](./type_defs.md#computetypedef) 
9. See [:material-code-braces: CreateSimulationJobResponseTypeDef](./type_defs.md#createsimulationjobresponsetypedef) 


```python
# create_simulation_job method usage example with argument unpacking

kwargs: CreateSimulationJobRequestTypeDef = {  # (1)
    "maxJobDurationInSeconds": ...,
    "iamRole": ...,
}

parent.create_simulation_job(**kwargs)
```

1. See [:material-code-braces: CreateSimulationJobRequestTypeDef](./type_defs.md#createsimulationjobrequesttypedef) 

### create\_world\_export\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").create_world_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/create_world_export_job.html)

```python
# create_world_export_job method definition

await def create_world_export_job(
    self,
    *,
    worlds: Sequence[str],
    outputLocation: OutputLocationTypeDef,  # (1)
    iamRole: str,
    clientRequestToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateWorldExportJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
2. See [:material-code-braces: CreateWorldExportJobResponseTypeDef](./type_defs.md#createworldexportjobresponsetypedef) 


```python
# create_world_export_job method usage example with argument unpacking

kwargs: CreateWorldExportJobRequestTypeDef = {  # (1)
    "worlds": ...,
    "outputLocation": ...,
    "iamRole": ...,
}

parent.create_world_export_job(**kwargs)
```

1. See [:material-code-braces: CreateWorldExportJobRequestTypeDef](./type_defs.md#createworldexportjobrequesttypedef) 

### create\_world\_generation\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").create_world_generation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/create_world_generation_job.html)

```python
# create_world_generation_job method definition

await def create_world_generation_job(
    self,
    *,
    template: str,
    worldCount: WorldCountTypeDef,  # (1)
    clientRequestToken: str = ...,
    tags: Mapping[str, str] = ...,
    worldTags: Mapping[str, str] = ...,
) -> CreateWorldGenerationJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: WorldCountTypeDef](./type_defs.md#worldcounttypedef) 
2. See [:material-code-braces: CreateWorldGenerationJobResponseTypeDef](./type_defs.md#createworldgenerationjobresponsetypedef) 


```python
# create_world_generation_job method usage example with argument unpacking

kwargs: CreateWorldGenerationJobRequestTypeDef = {  # (1)
    "template": ...,
    "worldCount": ...,
}

parent.create_world_generation_job(**kwargs)
```

1. See [:material-code-braces: CreateWorldGenerationJobRequestTypeDef](./type_defs.md#createworldgenerationjobrequesttypedef) 

### create\_world\_template

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").create_world_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/create_world_template.html)

```python
# create_world_template method definition

await def create_world_template(
    self,
    *,
    clientRequestToken: str = ...,
    name: str = ...,
    templateBody: str = ...,
    templateLocation: TemplateLocationTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateWorldTemplateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TemplateLocationTypeDef](./type_defs.md#templatelocationtypedef) 
2. See [:material-code-braces: CreateWorldTemplateResponseTypeDef](./type_defs.md#createworldtemplateresponsetypedef) 


```python
# create_world_template method usage example with argument unpacking

kwargs: CreateWorldTemplateRequestTypeDef = {  # (1)
    "clientRequestToken": ...,
}

parent.create_world_template(**kwargs)
```

1. See [:material-code-braces: CreateWorldTemplateRequestTypeDef](./type_defs.md#createworldtemplaterequesttypedef) 

### delete\_fleet

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").delete_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/delete_fleet.html)

```python
# delete_fleet method definition

await def delete_fleet(
    self,
    *,
    fleet: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_fleet method usage example with argument unpacking

kwargs: DeleteFleetRequestTypeDef = {  # (1)
    "fleet": ...,
}

parent.delete_fleet(**kwargs)
```

1. See [:material-code-braces: DeleteFleetRequestTypeDef](./type_defs.md#deletefleetrequesttypedef) 

### delete\_robot

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").delete_robot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/delete_robot.html)

```python
# delete_robot method definition

await def delete_robot(
    self,
    *,
    robot: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_robot method usage example with argument unpacking

kwargs: DeleteRobotRequestTypeDef = {  # (1)
    "robot": ...,
}

parent.delete_robot(**kwargs)
```

1. See [:material-code-braces: DeleteRobotRequestTypeDef](./type_defs.md#deleterobotrequesttypedef) 

### delete\_robot\_application

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").delete_robot_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/delete_robot_application.html)

```python
# delete_robot_application method definition

await def delete_robot_application(
    self,
    *,
    application: str,
    applicationVersion: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_robot_application method usage example with argument unpacking

kwargs: DeleteRobotApplicationRequestTypeDef = {  # (1)
    "application": ...,
}

parent.delete_robot_application(**kwargs)
```

1. See [:material-code-braces: DeleteRobotApplicationRequestTypeDef](./type_defs.md#deleterobotapplicationrequesttypedef) 

### delete\_simulation\_application

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").delete_simulation_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/delete_simulation_application.html)

```python
# delete_simulation_application method definition

await def delete_simulation_application(
    self,
    *,
    application: str,
    applicationVersion: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_simulation_application method usage example with argument unpacking

kwargs: DeleteSimulationApplicationRequestTypeDef = {  # (1)
    "application": ...,
}

parent.delete_simulation_application(**kwargs)
```

1. See [:material-code-braces: DeleteSimulationApplicationRequestTypeDef](./type_defs.md#deletesimulationapplicationrequesttypedef) 

### delete\_world\_template

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").delete_world_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/delete_world_template.html)

```python
# delete_world_template method definition

await def delete_world_template(
    self,
    *,
    template: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_world_template method usage example with argument unpacking

kwargs: DeleteWorldTemplateRequestTypeDef = {  # (1)
    "template": ...,
}

parent.delete_world_template(**kwargs)
```

1. See [:material-code-braces: DeleteWorldTemplateRequestTypeDef](./type_defs.md#deleteworldtemplaterequesttypedef) 

### deregister\_robot

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").deregister_robot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/deregister_robot.html)

```python
# deregister_robot method definition

await def deregister_robot(
    self,
    *,
    fleet: str,
    robot: str,
) -> DeregisterRobotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeregisterRobotResponseTypeDef](./type_defs.md#deregisterrobotresponsetypedef) 


```python
# deregister_robot method usage example with argument unpacking

kwargs: DeregisterRobotRequestTypeDef = {  # (1)
    "fleet": ...,
    "robot": ...,
}

parent.deregister_robot(**kwargs)
```

1. See [:material-code-braces: DeregisterRobotRequestTypeDef](./type_defs.md#deregisterrobotrequesttypedef) 

### describe\_deployment\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").describe_deployment_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/describe_deployment_job.html)

```python
# describe_deployment_job method definition

await def describe_deployment_job(
    self,
    *,
    job: str,
) -> DescribeDeploymentJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDeploymentJobResponseTypeDef](./type_defs.md#describedeploymentjobresponsetypedef) 


```python
# describe_deployment_job method usage example with argument unpacking

kwargs: DescribeDeploymentJobRequestTypeDef = {  # (1)
    "job": ...,
}

parent.describe_deployment_job(**kwargs)
```

1. See [:material-code-braces: DescribeDeploymentJobRequestTypeDef](./type_defs.md#describedeploymentjobrequesttypedef) 

### describe\_fleet

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").describe_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/describe_fleet.html)

```python
# describe_fleet method definition

await def describe_fleet(
    self,
    *,
    fleet: str,
) -> DescribeFleetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFleetResponseTypeDef](./type_defs.md#describefleetresponsetypedef) 


```python
# describe_fleet method usage example with argument unpacking

kwargs: DescribeFleetRequestTypeDef = {  # (1)
    "fleet": ...,
}

parent.describe_fleet(**kwargs)
```

1. See [:material-code-braces: DescribeFleetRequestTypeDef](./type_defs.md#describefleetrequesttypedef) 

### describe\_robot

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").describe_robot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/describe_robot.html)

```python
# describe_robot method definition

await def describe_robot(
    self,
    *,
    robot: str,
) -> DescribeRobotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRobotResponseTypeDef](./type_defs.md#describerobotresponsetypedef) 


```python
# describe_robot method usage example with argument unpacking

kwargs: DescribeRobotRequestTypeDef = {  # (1)
    "robot": ...,
}

parent.describe_robot(**kwargs)
```

1. See [:material-code-braces: DescribeRobotRequestTypeDef](./type_defs.md#describerobotrequesttypedef) 

### describe\_robot\_application

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").describe_robot_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/describe_robot_application.html)

```python
# describe_robot_application method definition

await def describe_robot_application(
    self,
    *,
    application: str,
    applicationVersion: str = ...,
) -> DescribeRobotApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRobotApplicationResponseTypeDef](./type_defs.md#describerobotapplicationresponsetypedef) 


```python
# describe_robot_application method usage example with argument unpacking

kwargs: DescribeRobotApplicationRequestTypeDef = {  # (1)
    "application": ...,
}

parent.describe_robot_application(**kwargs)
```

1. See [:material-code-braces: DescribeRobotApplicationRequestTypeDef](./type_defs.md#describerobotapplicationrequesttypedef) 

### describe\_simulation\_application

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").describe_simulation_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/describe_simulation_application.html)

```python
# describe_simulation_application method definition

await def describe_simulation_application(
    self,
    *,
    application: str,
    applicationVersion: str = ...,
) -> DescribeSimulationApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSimulationApplicationResponseTypeDef](./type_defs.md#describesimulationapplicationresponsetypedef) 


```python
# describe_simulation_application method usage example with argument unpacking

kwargs: DescribeSimulationApplicationRequestTypeDef = {  # (1)
    "application": ...,
}

parent.describe_simulation_application(**kwargs)
```

1. See [:material-code-braces: DescribeSimulationApplicationRequestTypeDef](./type_defs.md#describesimulationapplicationrequesttypedef) 

### describe\_simulation\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").describe_simulation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/describe_simulation_job.html)

```python
# describe_simulation_job method definition

await def describe_simulation_job(
    self,
    *,
    job: str,
) -> DescribeSimulationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSimulationJobResponseTypeDef](./type_defs.md#describesimulationjobresponsetypedef) 


```python
# describe_simulation_job method usage example with argument unpacking

kwargs: DescribeSimulationJobRequestTypeDef = {  # (1)
    "job": ...,
}

parent.describe_simulation_job(**kwargs)
```

1. See [:material-code-braces: DescribeSimulationJobRequestTypeDef](./type_defs.md#describesimulationjobrequesttypedef) 

### describe\_simulation\_job\_batch

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").describe_simulation_job_batch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/describe_simulation_job_batch.html)

```python
# describe_simulation_job_batch method definition

await def describe_simulation_job_batch(
    self,
    *,
    batch: str,
) -> DescribeSimulationJobBatchResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSimulationJobBatchResponseTypeDef](./type_defs.md#describesimulationjobbatchresponsetypedef) 


```python
# describe_simulation_job_batch method usage example with argument unpacking

kwargs: DescribeSimulationJobBatchRequestTypeDef = {  # (1)
    "batch": ...,
}

parent.describe_simulation_job_batch(**kwargs)
```

1. See [:material-code-braces: DescribeSimulationJobBatchRequestTypeDef](./type_defs.md#describesimulationjobbatchrequesttypedef) 

### describe\_world

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").describe_world` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/describe_world.html)

```python
# describe_world method definition

await def describe_world(
    self,
    *,
    world: str,
) -> DescribeWorldResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorldResponseTypeDef](./type_defs.md#describeworldresponsetypedef) 


```python
# describe_world method usage example with argument unpacking

kwargs: DescribeWorldRequestTypeDef = {  # (1)
    "world": ...,
}

parent.describe_world(**kwargs)
```

1. See [:material-code-braces: DescribeWorldRequestTypeDef](./type_defs.md#describeworldrequesttypedef) 

### describe\_world\_export\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").describe_world_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/describe_world_export_job.html)

```python
# describe_world_export_job method definition

await def describe_world_export_job(
    self,
    *,
    job: str,
) -> DescribeWorldExportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorldExportJobResponseTypeDef](./type_defs.md#describeworldexportjobresponsetypedef) 


```python
# describe_world_export_job method usage example with argument unpacking

kwargs: DescribeWorldExportJobRequestTypeDef = {  # (1)
    "job": ...,
}

parent.describe_world_export_job(**kwargs)
```

1. See [:material-code-braces: DescribeWorldExportJobRequestTypeDef](./type_defs.md#describeworldexportjobrequesttypedef) 

### describe\_world\_generation\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").describe_world_generation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/describe_world_generation_job.html)

```python
# describe_world_generation_job method definition

await def describe_world_generation_job(
    self,
    *,
    job: str,
) -> DescribeWorldGenerationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorldGenerationJobResponseTypeDef](./type_defs.md#describeworldgenerationjobresponsetypedef) 


```python
# describe_world_generation_job method usage example with argument unpacking

kwargs: DescribeWorldGenerationJobRequestTypeDef = {  # (1)
    "job": ...,
}

parent.describe_world_generation_job(**kwargs)
```

1. See [:material-code-braces: DescribeWorldGenerationJobRequestTypeDef](./type_defs.md#describeworldgenerationjobrequesttypedef) 

### describe\_world\_template

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").describe_world_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/describe_world_template.html)

```python
# describe_world_template method definition

await def describe_world_template(
    self,
    *,
    template: str,
) -> DescribeWorldTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorldTemplateResponseTypeDef](./type_defs.md#describeworldtemplateresponsetypedef) 


```python
# describe_world_template method usage example with argument unpacking

kwargs: DescribeWorldTemplateRequestTypeDef = {  # (1)
    "template": ...,
}

parent.describe_world_template(**kwargs)
```

1. See [:material-code-braces: DescribeWorldTemplateRequestTypeDef](./type_defs.md#describeworldtemplaterequesttypedef) 

### get\_world\_template\_body

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").get_world_template_body` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/get_world_template_body.html)

```python
# get_world_template_body method definition

await def get_world_template_body(
    self,
    *,
    template: str = ...,
    generationJob: str = ...,
) -> GetWorldTemplateBodyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorldTemplateBodyResponseTypeDef](./type_defs.md#getworldtemplatebodyresponsetypedef) 


```python
# get_world_template_body method usage example with argument unpacking

kwargs: GetWorldTemplateBodyRequestTypeDef = {  # (1)
    "template": ...,
}

parent.get_world_template_body(**kwargs)
```

1. See [:material-code-braces: GetWorldTemplateBodyRequestTypeDef](./type_defs.md#getworldtemplatebodyrequesttypedef) 

### list\_deployment\_jobs

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").list_deployment_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/list_deployment_jobs.html)

```python
# list_deployment_jobs method definition

await def list_deployment_jobs(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDeploymentJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListDeploymentJobsResponseTypeDef](./type_defs.md#listdeploymentjobsresponsetypedef) 


```python
# list_deployment_jobs method usage example with argument unpacking

kwargs: ListDeploymentJobsRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_deployment_jobs(**kwargs)
```

1. See [:material-code-braces: ListDeploymentJobsRequestTypeDef](./type_defs.md#listdeploymentjobsrequesttypedef) 

### list\_fleets

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").list_fleets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/list_fleets.html)

```python
# list_fleets method definition

await def list_fleets(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListFleetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListFleetsResponseTypeDef](./type_defs.md#listfleetsresponsetypedef) 


```python
# list_fleets method usage example with argument unpacking

kwargs: ListFleetsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_fleets(**kwargs)
```

1. See [:material-code-braces: ListFleetsRequestTypeDef](./type_defs.md#listfleetsrequesttypedef) 

### list\_robot\_applications

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").list_robot_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/list_robot_applications.html)

```python
# list_robot_applications method definition

await def list_robot_applications(
    self,
    *,
    versionQualifier: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListRobotApplicationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListRobotApplicationsResponseTypeDef](./type_defs.md#listrobotapplicationsresponsetypedef) 


```python
# list_robot_applications method usage example with argument unpacking

kwargs: ListRobotApplicationsRequestTypeDef = {  # (1)
    "versionQualifier": ...,
}

parent.list_robot_applications(**kwargs)
```

1. See [:material-code-braces: ListRobotApplicationsRequestTypeDef](./type_defs.md#listrobotapplicationsrequesttypedef) 

### list\_robots

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").list_robots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/list_robots.html)

```python
# list_robots method definition

await def list_robots(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListRobotsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListRobotsResponseTypeDef](./type_defs.md#listrobotsresponsetypedef) 


```python
# list_robots method usage example with argument unpacking

kwargs: ListRobotsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_robots(**kwargs)
```

1. See [:material-code-braces: ListRobotsRequestTypeDef](./type_defs.md#listrobotsrequesttypedef) 

### list\_simulation\_applications

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").list_simulation_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/list_simulation_applications.html)

```python
# list_simulation_applications method definition

await def list_simulation_applications(
    self,
    *,
    versionQualifier: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListSimulationApplicationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListSimulationApplicationsResponseTypeDef](./type_defs.md#listsimulationapplicationsresponsetypedef) 


```python
# list_simulation_applications method usage example with argument unpacking

kwargs: ListSimulationApplicationsRequestTypeDef = {  # (1)
    "versionQualifier": ...,
}

parent.list_simulation_applications(**kwargs)
```

1. See [:material-code-braces: ListSimulationApplicationsRequestTypeDef](./type_defs.md#listsimulationapplicationsrequesttypedef) 

### list\_simulation\_job\_batches

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").list_simulation_job_batches` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/list_simulation_job_batches.html)

```python
# list_simulation_job_batches method definition

await def list_simulation_job_batches(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListSimulationJobBatchesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListSimulationJobBatchesResponseTypeDef](./type_defs.md#listsimulationjobbatchesresponsetypedef) 


```python
# list_simulation_job_batches method usage example with argument unpacking

kwargs: ListSimulationJobBatchesRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_simulation_job_batches(**kwargs)
```

1. See [:material-code-braces: ListSimulationJobBatchesRequestTypeDef](./type_defs.md#listsimulationjobbatchesrequesttypedef) 

### list\_simulation\_jobs

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").list_simulation_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/list_simulation_jobs.html)

```python
# list_simulation_jobs method definition

await def list_simulation_jobs(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListSimulationJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListSimulationJobsResponseTypeDef](./type_defs.md#listsimulationjobsresponsetypedef) 


```python
# list_simulation_jobs method usage example with argument unpacking

kwargs: ListSimulationJobsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_simulation_jobs(**kwargs)
```

1. See [:material-code-braces: ListSimulationJobsRequestTypeDef](./type_defs.md#listsimulationjobsrequesttypedef) 

### list\_tags\_for\_resource

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### list\_world\_export\_jobs

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").list_world_export_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/list_world_export_jobs.html)

```python
# list_world_export_jobs method definition

await def list_world_export_jobs(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListWorldExportJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListWorldExportJobsResponseTypeDef](./type_defs.md#listworldexportjobsresponsetypedef) 


```python
# list_world_export_jobs method usage example with argument unpacking

kwargs: ListWorldExportJobsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_world_export_jobs(**kwargs)
```

1. See [:material-code-braces: ListWorldExportJobsRequestTypeDef](./type_defs.md#listworldexportjobsrequesttypedef) 

### list\_world\_generation\_jobs

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").list_world_generation_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/list_world_generation_jobs.html)

```python
# list_world_generation_jobs method definition

await def list_world_generation_jobs(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListWorldGenerationJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListWorldGenerationJobsResponseTypeDef](./type_defs.md#listworldgenerationjobsresponsetypedef) 


```python
# list_world_generation_jobs method usage example with argument unpacking

kwargs: ListWorldGenerationJobsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_world_generation_jobs(**kwargs)
```

1. See [:material-code-braces: ListWorldGenerationJobsRequestTypeDef](./type_defs.md#listworldgenerationjobsrequesttypedef) 

### list\_world\_templates

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").list_world_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/list_world_templates.html)

```python
# list_world_templates method definition

await def list_world_templates(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListWorldTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorldTemplatesResponseTypeDef](./type_defs.md#listworldtemplatesresponsetypedef) 


```python
# list_world_templates method usage example with argument unpacking

kwargs: ListWorldTemplatesRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_world_templates(**kwargs)
```

1. See [:material-code-braces: ListWorldTemplatesRequestTypeDef](./type_defs.md#listworldtemplatesrequesttypedef) 

### list\_worlds

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").list_worlds` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/list_worlds.html)

```python
# list_worlds method definition

await def list_worlds(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListWorldsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListWorldsResponseTypeDef](./type_defs.md#listworldsresponsetypedef) 


```python
# list_worlds method usage example with argument unpacking

kwargs: ListWorldsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_worlds(**kwargs)
```

1. See [:material-code-braces: ListWorldsRequestTypeDef](./type_defs.md#listworldsrequesttypedef) 

### register\_robot

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").register_robot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/register_robot.html)

```python
# register_robot method definition

await def register_robot(
    self,
    *,
    fleet: str,
    robot: str,
) -> RegisterRobotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterRobotResponseTypeDef](./type_defs.md#registerrobotresponsetypedef) 


```python
# register_robot method usage example with argument unpacking

kwargs: RegisterRobotRequestTypeDef = {  # (1)
    "fleet": ...,
    "robot": ...,
}

parent.register_robot(**kwargs)
```

1. See [:material-code-braces: RegisterRobotRequestTypeDef](./type_defs.md#registerrobotrequesttypedef) 

### restart\_simulation\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").restart_simulation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/restart_simulation_job.html)

```python
# restart_simulation_job method definition

await def restart_simulation_job(
    self,
    *,
    job: str,
) -> Dict[str, Any]:
    ...
```



```python
# restart_simulation_job method usage example with argument unpacking

kwargs: RestartSimulationJobRequestTypeDef = {  # (1)
    "job": ...,
}

parent.restart_simulation_job(**kwargs)
```

1. See [:material-code-braces: RestartSimulationJobRequestTypeDef](./type_defs.md#restartsimulationjobrequesttypedef) 

### start\_simulation\_job\_batch

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").start_simulation_job_batch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/start_simulation_job_batch.html)

```python
# start_simulation_job_batch method definition

await def start_simulation_job_batch(
    self,
    *,
    createSimulationJobRequests: Sequence[SimulationJobRequestUnionTypeDef],  # (1)
    clientRequestToken: str = ...,
    batchPolicy: BatchPolicyTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
) -> StartSimulationJobBatchResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SimulationJobRequestTypeDef](./type_defs.md#simulationjobrequesttypedef) [:material-code-braces: SimulationJobRequestOutputTypeDef](./type_defs.md#simulationjobrequestoutputtypedef) 
2. See [:material-code-braces: BatchPolicyTypeDef](./type_defs.md#batchpolicytypedef) 
3. See [:material-code-braces: StartSimulationJobBatchResponseTypeDef](./type_defs.md#startsimulationjobbatchresponsetypedef) 


```python
# start_simulation_job_batch method usage example with argument unpacking

kwargs: StartSimulationJobBatchRequestTypeDef = {  # (1)
    "createSimulationJobRequests": ...,
}

parent.start_simulation_job_batch(**kwargs)
```

1. See [:material-code-braces: StartSimulationJobBatchRequestTypeDef](./type_defs.md#startsimulationjobbatchrequesttypedef) 

### sync\_deployment\_job

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").sync_deployment_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/sync_deployment_job.html)

```python
# sync_deployment_job method definition

await def sync_deployment_job(
    self,
    *,
    clientRequestToken: str,
    fleet: str,
) -> SyncDeploymentJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SyncDeploymentJobResponseTypeDef](./type_defs.md#syncdeploymentjobresponsetypedef) 


```python
# sync_deployment_job method usage example with argument unpacking

kwargs: SyncDeploymentJobRequestTypeDef = {  # (1)
    "clientRequestToken": ...,
    "fleet": ...,
}

parent.sync_deployment_job(**kwargs)
```

1. See [:material-code-braces: SyncDeploymentJobRequestTypeDef](./type_defs.md#syncdeploymentjobrequesttypedef) 

### tag\_resource

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_robot\_application

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").update_robot_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/update_robot_application.html)

```python
# update_robot_application method definition

await def update_robot_application(
    self,
    *,
    application: str,
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (1)
    sources: Sequence[SourceConfigTypeDef] = ...,  # (2)
    currentRevisionId: str = ...,
    environment: EnvironmentTypeDef = ...,  # (3)
) -> UpdateRobotApplicationResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
2. See [:material-code-braces: SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef) 
3. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
4. See [:material-code-braces: UpdateRobotApplicationResponseTypeDef](./type_defs.md#updaterobotapplicationresponsetypedef) 


```python
# update_robot_application method usage example with argument unpacking

kwargs: UpdateRobotApplicationRequestTypeDef = {  # (1)
    "application": ...,
    "robotSoftwareSuite": ...,
}

parent.update_robot_application(**kwargs)
```

1. See [:material-code-braces: UpdateRobotApplicationRequestTypeDef](./type_defs.md#updaterobotapplicationrequesttypedef) 

### update\_simulation\_application

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").update_simulation_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/update_simulation_application.html)

```python
# update_simulation_application method definition

await def update_simulation_application(
    self,
    *,
    application: str,
    simulationSoftwareSuite: SimulationSoftwareSuiteTypeDef,  # (1)
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (2)
    sources: Sequence[SourceConfigTypeDef] = ...,  # (3)
    renderingEngine: RenderingEngineTypeDef = ...,  # (4)
    currentRevisionId: str = ...,
    environment: EnvironmentTypeDef = ...,  # (5)
) -> UpdateSimulationApplicationResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: SimulationSoftwareSuiteTypeDef](./type_defs.md#simulationsoftwaresuitetypedef) 
2. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
3. See [:material-code-braces: SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef) 
4. See [:material-code-braces: RenderingEngineTypeDef](./type_defs.md#renderingenginetypedef) 
5. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
6. See [:material-code-braces: UpdateSimulationApplicationResponseTypeDef](./type_defs.md#updatesimulationapplicationresponsetypedef) 


```python
# update_simulation_application method usage example with argument unpacking

kwargs: UpdateSimulationApplicationRequestTypeDef = {  # (1)
    "application": ...,
    "simulationSoftwareSuite": ...,
    "robotSoftwareSuite": ...,
}

parent.update_simulation_application(**kwargs)
```

1. See [:material-code-braces: UpdateSimulationApplicationRequestTypeDef](./type_defs.md#updatesimulationapplicationrequesttypedef) 

### update\_world\_template

End of support notice: On September 10, 2025, Amazon Web Services will
discontinue support for Amazon Web Services RoboMaker.

Type annotations and code completion for `#!python session.create_client("robomaker").update_world_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/client/update_world_template.html)

```python
# update_world_template method definition

await def update_world_template(
    self,
    *,
    template: str,
    name: str = ...,
    templateBody: str = ...,
    templateLocation: TemplateLocationTypeDef = ...,  # (1)
) -> UpdateWorldTemplateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TemplateLocationTypeDef](./type_defs.md#templatelocationtypedef) 
2. See [:material-code-braces: UpdateWorldTemplateResponseTypeDef](./type_defs.md#updateworldtemplateresponsetypedef) 


```python
# update_world_template method usage example with argument unpacking

kwargs: UpdateWorldTemplateRequestTypeDef = {  # (1)
    "template": ...,
}

parent.update_world_template(**kwargs)
```

1. See [:material-code-braces: UpdateWorldTemplateRequestTypeDef](./type_defs.md#updateworldtemplaterequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("robomaker").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("robomaker").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client)

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

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator` method with overloads.

- `client.get_paginator("list_deployment_jobs")` -> [ListDeploymentJobsPaginator](./paginators.md#listdeploymentjobspaginator)
- `client.get_paginator("list_fleets")` -> [ListFleetsPaginator](./paginators.md#listfleetspaginator)
- `client.get_paginator("list_robot_applications")` -> [ListRobotApplicationsPaginator](./paginators.md#listrobotapplicationspaginator)
- `client.get_paginator("list_robots")` -> [ListRobotsPaginator](./paginators.md#listrobotspaginator)
- `client.get_paginator("list_simulation_applications")` -> [ListSimulationApplicationsPaginator](./paginators.md#listsimulationapplicationspaginator)
- `client.get_paginator("list_simulation_job_batches")` -> [ListSimulationJobBatchesPaginator](./paginators.md#listsimulationjobbatchespaginator)
- `client.get_paginator("list_simulation_jobs")` -> [ListSimulationJobsPaginator](./paginators.md#listsimulationjobspaginator)
- `client.get_paginator("list_world_export_jobs")` -> [ListWorldExportJobsPaginator](./paginators.md#listworldexportjobspaginator)
- `client.get_paginator("list_world_generation_jobs")` -> [ListWorldGenerationJobsPaginator](./paginators.md#listworldgenerationjobspaginator)
- `client.get_paginator("list_world_templates")` -> [ListWorldTemplatesPaginator](./paginators.md#listworldtemplatespaginator)
- `client.get_paginator("list_worlds")` -> [ListWorldsPaginator](./paginators.md#listworldspaginator)



