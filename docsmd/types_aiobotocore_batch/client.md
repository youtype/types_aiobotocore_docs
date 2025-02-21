# BatchClient

> [Index](../README.md) > [Batch](./README.md) > BatchClient

!!! note ""

    Auto-generated documentation for [Batch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#batch)
    type annotations stubs module [types-aiobotocore-batch](https://pypi.org/project/types-aiobotocore-batch/).

## BatchClient

Type annotations and code completion for `#!python session.create_client("batch")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client)

```python
# BatchClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_batch.client import BatchClient

session = get_session()
async with session.create_client("batch") as client:
    client: BatchClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("batch").exceptions` structure.

```python
# BatchClient.exceptions usage example

async with session.create_client("batch") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ClientException,
        client.ServerException,
    ) as e:
        print(e)
```

```python
# BatchClient usage type checking example

from types_aiobotocore_batch.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("batch").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("batch").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/generate_presigned_url.html)

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


### cancel\_job

Cancels a job in an Batch job queue.

Type annotations and code completion for `#!python session.create_client("batch").cancel_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/cancel_job.html)

```python
# cancel_job method definition

await def cancel_job(
    self,
    *,
    jobId: str,
    reason: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_job method usage example with argument unpacking

kwargs: CancelJobRequestTypeDef = {  # (1)
    "jobId": ...,
    "reason": ...,
}

parent.cancel_job(**kwargs)
```

1. See [:material-code-braces: CancelJobRequestTypeDef](./type_defs.md#canceljobrequesttypedef) 

### create\_compute\_environment

Creates an Batch compute environment.

Type annotations and code completion for `#!python session.create_client("batch").create_compute_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/create_compute_environment.html)

```python
# create_compute_environment method definition

await def create_compute_environment(
    self,
    *,
    computeEnvironmentName: str,
    type: CETypeType,  # (1)
    state: CEStateType = ...,  # (2)
    unmanagedvCpus: int = ...,
    computeResources: ComputeResourceUnionTypeDef = ...,  # (3)
    serviceRole: str = ...,
    tags: Mapping[str, str] = ...,
    eksConfiguration: EksConfigurationTypeDef = ...,  # (4)
    context: str = ...,
) -> CreateComputeEnvironmentResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: CETypeType](./literals.md#cetypetype) 
2. See [:material-code-brackets: CEStateType](./literals.md#cestatetype) 
3. See [:material-code-braces: ComputeResourceTypeDef](./type_defs.md#computeresourcetypedef) [:material-code-braces: ComputeResourceOutputTypeDef](./type_defs.md#computeresourceoutputtypedef) 
4. See [:material-code-braces: EksConfigurationTypeDef](./type_defs.md#eksconfigurationtypedef) 
5. See [:material-code-braces: CreateComputeEnvironmentResponseTypeDef](./type_defs.md#createcomputeenvironmentresponsetypedef) 


```python
# create_compute_environment method usage example with argument unpacking

kwargs: CreateComputeEnvironmentRequestTypeDef = {  # (1)
    "computeEnvironmentName": ...,
    "type": ...,
}

parent.create_compute_environment(**kwargs)
```

1. See [:material-code-braces: CreateComputeEnvironmentRequestTypeDef](./type_defs.md#createcomputeenvironmentrequesttypedef) 

### create\_job\_queue

Creates an Batch job queue.

Type annotations and code completion for `#!python session.create_client("batch").create_job_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/create_job_queue.html)

```python
# create_job_queue method definition

await def create_job_queue(
    self,
    *,
    jobQueueName: str,
    priority: int,
    computeEnvironmentOrder: Sequence[ComputeEnvironmentOrderTypeDef],  # (1)
    state: JQStateType = ...,  # (2)
    schedulingPolicyArn: str = ...,
    tags: Mapping[str, str] = ...,
    jobStateTimeLimitActions: Sequence[JobStateTimeLimitActionTypeDef] = ...,  # (3)
) -> CreateJobQueueResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ComputeEnvironmentOrderTypeDef](./type_defs.md#computeenvironmentordertypedef) 
2. See [:material-code-brackets: JQStateType](./literals.md#jqstatetype) 
3. See [:material-code-braces: JobStateTimeLimitActionTypeDef](./type_defs.md#jobstatetimelimitactiontypedef) 
4. See [:material-code-braces: CreateJobQueueResponseTypeDef](./type_defs.md#createjobqueueresponsetypedef) 


```python
# create_job_queue method usage example with argument unpacking

kwargs: CreateJobQueueRequestTypeDef = {  # (1)
    "jobQueueName": ...,
    "priority": ...,
    "computeEnvironmentOrder": ...,
}

parent.create_job_queue(**kwargs)
```

1. See [:material-code-braces: CreateJobQueueRequestTypeDef](./type_defs.md#createjobqueuerequesttypedef) 

### create\_scheduling\_policy

Creates an Batch scheduling policy.

Type annotations and code completion for `#!python session.create_client("batch").create_scheduling_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/create_scheduling_policy.html)

```python
# create_scheduling_policy method definition

await def create_scheduling_policy(
    self,
    *,
    name: str,
    fairsharePolicy: FairsharePolicyUnionTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateSchedulingPolicyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FairsharePolicyTypeDef](./type_defs.md#fairsharepolicytypedef) [:material-code-braces: FairsharePolicyOutputTypeDef](./type_defs.md#fairsharepolicyoutputtypedef) 
2. See [:material-code-braces: CreateSchedulingPolicyResponseTypeDef](./type_defs.md#createschedulingpolicyresponsetypedef) 


```python
# create_scheduling_policy method usage example with argument unpacking

kwargs: CreateSchedulingPolicyRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_scheduling_policy(**kwargs)
```

1. See [:material-code-braces: CreateSchedulingPolicyRequestTypeDef](./type_defs.md#createschedulingpolicyrequesttypedef) 

### delete\_compute\_environment

Deletes an Batch compute environment.

Type annotations and code completion for `#!python session.create_client("batch").delete_compute_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/delete_compute_environment.html)

```python
# delete_compute_environment method definition

await def delete_compute_environment(
    self,
    *,
    computeEnvironment: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_compute_environment method usage example with argument unpacking

kwargs: DeleteComputeEnvironmentRequestTypeDef = {  # (1)
    "computeEnvironment": ...,
}

parent.delete_compute_environment(**kwargs)
```

1. See [:material-code-braces: DeleteComputeEnvironmentRequestTypeDef](./type_defs.md#deletecomputeenvironmentrequesttypedef) 

### delete\_job\_queue

Deletes the specified job queue.

Type annotations and code completion for `#!python session.create_client("batch").delete_job_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/delete_job_queue.html)

```python
# delete_job_queue method definition

await def delete_job_queue(
    self,
    *,
    jobQueue: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_job_queue method usage example with argument unpacking

kwargs: DeleteJobQueueRequestTypeDef = {  # (1)
    "jobQueue": ...,
}

parent.delete_job_queue(**kwargs)
```

1. See [:material-code-braces: DeleteJobQueueRequestTypeDef](./type_defs.md#deletejobqueuerequesttypedef) 

### delete\_scheduling\_policy

Deletes the specified scheduling policy.

Type annotations and code completion for `#!python session.create_client("batch").delete_scheduling_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/delete_scheduling_policy.html)

```python
# delete_scheduling_policy method definition

await def delete_scheduling_policy(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_scheduling_policy method usage example with argument unpacking

kwargs: DeleteSchedulingPolicyRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_scheduling_policy(**kwargs)
```

1. See [:material-code-braces: DeleteSchedulingPolicyRequestTypeDef](./type_defs.md#deleteschedulingpolicyrequesttypedef) 

### deregister\_job\_definition

Deregisters an Batch job definition.

Type annotations and code completion for `#!python session.create_client("batch").deregister_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/deregister_job_definition.html)

```python
# deregister_job_definition method definition

await def deregister_job_definition(
    self,
    *,
    jobDefinition: str,
) -> Dict[str, Any]:
    ...
```



```python
# deregister_job_definition method usage example with argument unpacking

kwargs: DeregisterJobDefinitionRequestTypeDef = {  # (1)
    "jobDefinition": ...,
}

parent.deregister_job_definition(**kwargs)
```

1. See [:material-code-braces: DeregisterJobDefinitionRequestTypeDef](./type_defs.md#deregisterjobdefinitionrequesttypedef) 

### describe\_compute\_environments

Describes one or more of your compute environments.

Type annotations and code completion for `#!python session.create_client("batch").describe_compute_environments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/describe_compute_environments.html)

```python
# describe_compute_environments method definition

await def describe_compute_environments(
    self,
    *,
    computeEnvironments: Sequence[str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeComputeEnvironmentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeComputeEnvironmentsResponseTypeDef](./type_defs.md#describecomputeenvironmentsresponsetypedef) 


```python
# describe_compute_environments method usage example with argument unpacking

kwargs: DescribeComputeEnvironmentsRequestTypeDef = {  # (1)
    "computeEnvironments": ...,
}

parent.describe_compute_environments(**kwargs)
```

1. See [:material-code-braces: DescribeComputeEnvironmentsRequestTypeDef](./type_defs.md#describecomputeenvironmentsrequesttypedef) 

### describe\_job\_definitions

Describes a list of job definitions.

Type annotations and code completion for `#!python session.create_client("batch").describe_job_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/describe_job_definitions.html)

```python
# describe_job_definitions method definition

await def describe_job_definitions(
    self,
    *,
    jobDefinitions: Sequence[str] = ...,
    maxResults: int = ...,
    jobDefinitionName: str = ...,
    status: str = ...,
    nextToken: str = ...,
) -> DescribeJobDefinitionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeJobDefinitionsResponseTypeDef](./type_defs.md#describejobdefinitionsresponsetypedef) 


```python
# describe_job_definitions method usage example with argument unpacking

kwargs: DescribeJobDefinitionsRequestTypeDef = {  # (1)
    "jobDefinitions": ...,
}

parent.describe_job_definitions(**kwargs)
```

1. See [:material-code-braces: DescribeJobDefinitionsRequestTypeDef](./type_defs.md#describejobdefinitionsrequesttypedef) 

### describe\_job\_queues

Describes one or more of your job queues.

Type annotations and code completion for `#!python session.create_client("batch").describe_job_queues` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/describe_job_queues.html)

```python
# describe_job_queues method definition

await def describe_job_queues(
    self,
    *,
    jobQueues: Sequence[str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeJobQueuesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeJobQueuesResponseTypeDef](./type_defs.md#describejobqueuesresponsetypedef) 


```python
# describe_job_queues method usage example with argument unpacking

kwargs: DescribeJobQueuesRequestTypeDef = {  # (1)
    "jobQueues": ...,
}

parent.describe_job_queues(**kwargs)
```

1. See [:material-code-braces: DescribeJobQueuesRequestTypeDef](./type_defs.md#describejobqueuesrequesttypedef) 

### describe\_jobs

Describes a list of Batch jobs.

Type annotations and code completion for `#!python session.create_client("batch").describe_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/describe_jobs.html)

```python
# describe_jobs method definition

await def describe_jobs(
    self,
    *,
    jobs: Sequence[str],
) -> DescribeJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef) 


```python
# describe_jobs method usage example with argument unpacking

kwargs: DescribeJobsRequestTypeDef = {  # (1)
    "jobs": ...,
}

parent.describe_jobs(**kwargs)
```

1. See [:material-code-braces: DescribeJobsRequestTypeDef](./type_defs.md#describejobsrequesttypedef) 

### describe\_scheduling\_policies

Describes one or more of your scheduling policies.

Type annotations and code completion for `#!python session.create_client("batch").describe_scheduling_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/describe_scheduling_policies.html)

```python
# describe_scheduling_policies method definition

await def describe_scheduling_policies(
    self,
    *,
    arns: Sequence[str],
) -> DescribeSchedulingPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSchedulingPoliciesResponseTypeDef](./type_defs.md#describeschedulingpoliciesresponsetypedef) 


```python
# describe_scheduling_policies method usage example with argument unpacking

kwargs: DescribeSchedulingPoliciesRequestTypeDef = {  # (1)
    "arns": ...,
}

parent.describe_scheduling_policies(**kwargs)
```

1. See [:material-code-braces: DescribeSchedulingPoliciesRequestTypeDef](./type_defs.md#describeschedulingpoliciesrequesttypedef) 

### get\_job\_queue\_snapshot

Provides a list of the first 100 <code>RUNNABLE</code> jobs associated to a
single job queue.

Type annotations and code completion for `#!python session.create_client("batch").get_job_queue_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/get_job_queue_snapshot.html)

```python
# get_job_queue_snapshot method definition

await def get_job_queue_snapshot(
    self,
    *,
    jobQueue: str,
) -> GetJobQueueSnapshotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobQueueSnapshotResponseTypeDef](./type_defs.md#getjobqueuesnapshotresponsetypedef) 


```python
# get_job_queue_snapshot method usage example with argument unpacking

kwargs: GetJobQueueSnapshotRequestTypeDef = {  # (1)
    "jobQueue": ...,
}

parent.get_job_queue_snapshot(**kwargs)
```

1. See [:material-code-braces: GetJobQueueSnapshotRequestTypeDef](./type_defs.md#getjobqueuesnapshotrequesttypedef) 

### list\_jobs

Returns a list of Batch jobs.

Type annotations and code completion for `#!python session.create_client("batch").list_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/list_jobs.html)

```python
# list_jobs method definition

await def list_jobs(
    self,
    *,
    jobQueue: str = ...,
    arrayJobId: str = ...,
    multiNodeJobId: str = ...,
    jobStatus: JobStatusType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    filters: Sequence[KeyValuesPairTypeDef] = ...,  # (2)
) -> ListJobsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: KeyValuesPairTypeDef](./type_defs.md#keyvaluespairtypedef) 
3. See [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


```python
# list_jobs method usage example with argument unpacking

kwargs: ListJobsRequestTypeDef = {  # (1)
    "jobQueue": ...,
}

parent.list_jobs(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestTypeDef](./type_defs.md#listjobsrequesttypedef) 

### list\_scheduling\_policies

Returns a list of Batch scheduling policies.

Type annotations and code completion for `#!python session.create_client("batch").list_scheduling_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/list_scheduling_policies.html)

```python
# list_scheduling_policies method definition

await def list_scheduling_policies(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSchedulingPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSchedulingPoliciesResponseTypeDef](./type_defs.md#listschedulingpoliciesresponsetypedef) 


```python
# list_scheduling_policies method usage example with argument unpacking

kwargs: ListSchedulingPoliciesRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_scheduling_policies(**kwargs)
```

1. See [:material-code-braces: ListSchedulingPoliciesRequestTypeDef](./type_defs.md#listschedulingpoliciesrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for an Batch resource.

Type annotations and code completion for `#!python session.create_client("batch").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/list_tags_for_resource.html)

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

### register\_job\_definition

Registers an Batch job definition.

Type annotations and code completion for `#!python session.create_client("batch").register_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/register_job_definition.html)

```python
# register_job_definition method definition

await def register_job_definition(
    self,
    *,
    jobDefinitionName: str,
    type: JobDefinitionTypeType,  # (1)
    parameters: Mapping[str, str] = ...,
    schedulingPriority: int = ...,
    containerProperties: ContainerPropertiesUnionTypeDef = ...,  # (2)
    nodeProperties: NodePropertiesUnionTypeDef = ...,  # (3)
    retryStrategy: RetryStrategyUnionTypeDef = ...,  # (4)
    propagateTags: bool = ...,
    timeout: JobTimeoutTypeDef = ...,  # (5)
    tags: Mapping[str, str] = ...,
    platformCapabilities: Sequence[PlatformCapabilityType] = ...,  # (6)
    eksProperties: EksPropertiesUnionTypeDef = ...,  # (7)
    ecsProperties: EcsPropertiesUnionTypeDef = ...,  # (8)
) -> RegisterJobDefinitionResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-brackets: JobDefinitionTypeType](./literals.md#jobdefinitiontypetype) 
2. See [:material-code-braces: ContainerPropertiesTypeDef](./type_defs.md#containerpropertiestypedef) [:material-code-braces: ContainerPropertiesOutputTypeDef](./type_defs.md#containerpropertiesoutputtypedef) 
3. See [:material-code-braces: NodePropertiesTypeDef](./type_defs.md#nodepropertiestypedef) [:material-code-braces: NodePropertiesOutputTypeDef](./type_defs.md#nodepropertiesoutputtypedef) 
4. See [:material-code-braces: RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef) [:material-code-braces: RetryStrategyOutputTypeDef](./type_defs.md#retrystrategyoutputtypedef) 
5. See [:material-code-braces: JobTimeoutTypeDef](./type_defs.md#jobtimeouttypedef) 
6. See [:material-code-brackets: PlatformCapabilityType](./literals.md#platformcapabilitytype) 
7. See [:material-code-braces: EksPropertiesTypeDef](./type_defs.md#ekspropertiestypedef) [:material-code-braces: EksPropertiesOutputTypeDef](./type_defs.md#ekspropertiesoutputtypedef) 
8. See [:material-code-braces: EcsPropertiesTypeDef](./type_defs.md#ecspropertiestypedef) [:material-code-braces: EcsPropertiesOutputTypeDef](./type_defs.md#ecspropertiesoutputtypedef) 
9. See [:material-code-braces: RegisterJobDefinitionResponseTypeDef](./type_defs.md#registerjobdefinitionresponsetypedef) 


```python
# register_job_definition method usage example with argument unpacking

kwargs: RegisterJobDefinitionRequestTypeDef = {  # (1)
    "jobDefinitionName": ...,
    "type": ...,
}

parent.register_job_definition(**kwargs)
```

1. See [:material-code-braces: RegisterJobDefinitionRequestTypeDef](./type_defs.md#registerjobdefinitionrequesttypedef) 

### submit\_job

Submits an Batch job from a job definition.

Type annotations and code completion for `#!python session.create_client("batch").submit_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/submit_job.html)

```python
# submit_job method definition

await def submit_job(
    self,
    *,
    jobName: str,
    jobQueue: str,
    jobDefinition: str,
    shareIdentifier: str = ...,
    schedulingPriorityOverride: int = ...,
    arrayProperties: ArrayPropertiesTypeDef = ...,  # (1)
    dependsOn: Sequence[JobDependencyTypeDef] = ...,  # (2)
    parameters: Mapping[str, str] = ...,
    containerOverrides: ContainerOverridesTypeDef = ...,  # (3)
    nodeOverrides: NodeOverridesTypeDef = ...,  # (4)
    retryStrategy: RetryStrategyUnionTypeDef = ...,  # (5)
    propagateTags: bool = ...,
    timeout: JobTimeoutTypeDef = ...,  # (6)
    tags: Mapping[str, str] = ...,
    eksPropertiesOverride: EksPropertiesOverrideTypeDef = ...,  # (7)
    ecsPropertiesOverride: EcsPropertiesOverrideTypeDef = ...,  # (8)
) -> SubmitJobResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: ArrayPropertiesTypeDef](./type_defs.md#arraypropertiestypedef) 
2. See [:material-code-braces: JobDependencyTypeDef](./type_defs.md#jobdependencytypedef) 
3. See [:material-code-braces: ContainerOverridesTypeDef](./type_defs.md#containeroverridestypedef) 
4. See [:material-code-braces: NodeOverridesTypeDef](./type_defs.md#nodeoverridestypedef) 
5. See [:material-code-braces: RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef) [:material-code-braces: RetryStrategyOutputTypeDef](./type_defs.md#retrystrategyoutputtypedef) 
6. See [:material-code-braces: JobTimeoutTypeDef](./type_defs.md#jobtimeouttypedef) 
7. See [:material-code-braces: EksPropertiesOverrideTypeDef](./type_defs.md#ekspropertiesoverridetypedef) 
8. See [:material-code-braces: EcsPropertiesOverrideTypeDef](./type_defs.md#ecspropertiesoverridetypedef) 
9. See [:material-code-braces: SubmitJobResponseTypeDef](./type_defs.md#submitjobresponsetypedef) 


```python
# submit_job method usage example with argument unpacking

kwargs: SubmitJobRequestTypeDef = {  # (1)
    "jobName": ...,
    "jobQueue": ...,
    "jobDefinition": ...,
}

parent.submit_job(**kwargs)
```

1. See [:material-code-braces: SubmitJobRequestTypeDef](./type_defs.md#submitjobrequesttypedef) 

### tag\_resource

Associates the specified tags to a resource with the specified
<code>resourceArn</code>.

Type annotations and code completion for `#!python session.create_client("batch").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/tag_resource.html)

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

### terminate\_job

Terminates a job in a job queue.

Type annotations and code completion for `#!python session.create_client("batch").terminate_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/terminate_job.html)

```python
# terminate_job method definition

await def terminate_job(
    self,
    *,
    jobId: str,
    reason: str,
) -> Dict[str, Any]:
    ...
```



```python
# terminate_job method usage example with argument unpacking

kwargs: TerminateJobRequestTypeDef = {  # (1)
    "jobId": ...,
    "reason": ...,
}

parent.terminate_job(**kwargs)
```

1. See [:material-code-braces: TerminateJobRequestTypeDef](./type_defs.md#terminatejobrequesttypedef) 

### untag\_resource

Deletes specified tags from an Batch resource.

Type annotations and code completion for `#!python session.create_client("batch").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/untag_resource.html)

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

### update\_compute\_environment

Updates an Batch compute environment.

Type annotations and code completion for `#!python session.create_client("batch").update_compute_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/update_compute_environment.html)

```python
# update_compute_environment method definition

await def update_compute_environment(
    self,
    *,
    computeEnvironment: str,
    state: CEStateType = ...,  # (1)
    unmanagedvCpus: int = ...,
    computeResources: ComputeResourceUpdateTypeDef = ...,  # (2)
    serviceRole: str = ...,
    updatePolicy: UpdatePolicyTypeDef = ...,  # (3)
    context: str = ...,
) -> UpdateComputeEnvironmentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: CEStateType](./literals.md#cestatetype) 
2. See [:material-code-braces: ComputeResourceUpdateTypeDef](./type_defs.md#computeresourceupdatetypedef) 
3. See [:material-code-braces: UpdatePolicyTypeDef](./type_defs.md#updatepolicytypedef) 
4. See [:material-code-braces: UpdateComputeEnvironmentResponseTypeDef](./type_defs.md#updatecomputeenvironmentresponsetypedef) 


```python
# update_compute_environment method usage example with argument unpacking

kwargs: UpdateComputeEnvironmentRequestTypeDef = {  # (1)
    "computeEnvironment": ...,
}

parent.update_compute_environment(**kwargs)
```

1. See [:material-code-braces: UpdateComputeEnvironmentRequestTypeDef](./type_defs.md#updatecomputeenvironmentrequesttypedef) 

### update\_job\_queue

Updates a job queue.

Type annotations and code completion for `#!python session.create_client("batch").update_job_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/update_job_queue.html)

```python
# update_job_queue method definition

await def update_job_queue(
    self,
    *,
    jobQueue: str,
    state: JQStateType = ...,  # (1)
    schedulingPolicyArn: str = ...,
    priority: int = ...,
    computeEnvironmentOrder: Sequence[ComputeEnvironmentOrderTypeDef] = ...,  # (2)
    jobStateTimeLimitActions: Sequence[JobStateTimeLimitActionTypeDef] = ...,  # (3)
) -> UpdateJobQueueResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: JQStateType](./literals.md#jqstatetype) 
2. See [:material-code-braces: ComputeEnvironmentOrderTypeDef](./type_defs.md#computeenvironmentordertypedef) 
3. See [:material-code-braces: JobStateTimeLimitActionTypeDef](./type_defs.md#jobstatetimelimitactiontypedef) 
4. See [:material-code-braces: UpdateJobQueueResponseTypeDef](./type_defs.md#updatejobqueueresponsetypedef) 


```python
# update_job_queue method usage example with argument unpacking

kwargs: UpdateJobQueueRequestTypeDef = {  # (1)
    "jobQueue": ...,
}

parent.update_job_queue(**kwargs)
```

1. See [:material-code-braces: UpdateJobQueueRequestTypeDef](./type_defs.md#updatejobqueuerequesttypedef) 

### update\_scheduling\_policy

Updates a scheduling policy.

Type annotations and code completion for `#!python session.create_client("batch").update_scheduling_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/client/update_scheduling_policy.html)

```python
# update_scheduling_policy method definition

await def update_scheduling_policy(
    self,
    *,
    arn: str,
    fairsharePolicy: FairsharePolicyUnionTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: FairsharePolicyTypeDef](./type_defs.md#fairsharepolicytypedef) [:material-code-braces: FairsharePolicyOutputTypeDef](./type_defs.md#fairsharepolicyoutputtypedef) 


```python
# update_scheduling_policy method usage example with argument unpacking

kwargs: UpdateSchedulingPolicyRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_scheduling_policy(**kwargs)
```

1. See [:material-code-braces: UpdateSchedulingPolicyRequestTypeDef](./type_defs.md#updateschedulingpolicyrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("batch").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("batch").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client)

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

Type annotations and code completion for `#!python session.create_client("batch").get_paginator` method with overloads.

- `client.get_paginator("describe_compute_environments")` -> [DescribeComputeEnvironmentsPaginator](./paginators.md#describecomputeenvironmentspaginator)
- `client.get_paginator("describe_job_definitions")` -> [DescribeJobDefinitionsPaginator](./paginators.md#describejobdefinitionspaginator)
- `client.get_paginator("describe_job_queues")` -> [DescribeJobQueuesPaginator](./paginators.md#describejobqueuespaginator)
- `client.get_paginator("list_jobs")` -> [ListJobsPaginator](./paginators.md#listjobspaginator)
- `client.get_paginator("list_scheduling_policies")` -> [ListSchedulingPoliciesPaginator](./paginators.md#listschedulingpoliciespaginator)



