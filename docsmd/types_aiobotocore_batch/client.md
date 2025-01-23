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

kwargs: CancelJobRequestRequestTypeDef = {  # (1)
    "jobId": ...,
    "reason": ...,
}

parent.cancel_job(**kwargs)
```

1. See [:material-code-braces: CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef) 

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
    computeResources: ComputeResourceTypeDef = ...,  # (3)
    serviceRole: str = ...,
    tags: Mapping[str, str] = ...,
    eksConfiguration: EksConfigurationTypeDef = ...,  # (4)
    context: str = ...,
) -> CreateComputeEnvironmentResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: CETypeType](./literals.md#cetypetype) 
2. See [:material-code-brackets: CEStateType](./literals.md#cestatetype) 
3. See [:material-code-braces: ComputeResourceTypeDef](./type_defs.md#computeresourcetypedef) 
4. See [:material-code-braces: EksConfigurationTypeDef](./type_defs.md#eksconfigurationtypedef) 
5. See [:material-code-braces: CreateComputeEnvironmentResponseTypeDef](./type_defs.md#createcomputeenvironmentresponsetypedef) 


```python
# create_compute_environment method usage example with argument unpacking

kwargs: CreateComputeEnvironmentRequestRequestTypeDef = {  # (1)
    "computeEnvironmentName": ...,
    "type": ...,
}

parent.create_compute_environment(**kwargs)
```

1. See [:material-code-braces: CreateComputeEnvironmentRequestRequestTypeDef](./type_defs.md#createcomputeenvironmentrequestrequesttypedef) 

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

kwargs: CreateJobQueueRequestRequestTypeDef = {  # (1)
    "jobQueueName": ...,
    "priority": ...,
    "computeEnvironmentOrder": ...,
}

parent.create_job_queue(**kwargs)
```

1. See [:material-code-braces: CreateJobQueueRequestRequestTypeDef](./type_defs.md#createjobqueuerequestrequesttypedef) 

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
    fairsharePolicy: FairsharePolicyTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateSchedulingPolicyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FairsharePolicyTypeDef](./type_defs.md#fairsharepolicytypedef) 
2. See [:material-code-braces: CreateSchedulingPolicyResponseTypeDef](./type_defs.md#createschedulingpolicyresponsetypedef) 


```python
# create_scheduling_policy method usage example with argument unpacking

kwargs: CreateSchedulingPolicyRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_scheduling_policy(**kwargs)
```

1. See [:material-code-braces: CreateSchedulingPolicyRequestRequestTypeDef](./type_defs.md#createschedulingpolicyrequestrequesttypedef) 

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

kwargs: DeleteComputeEnvironmentRequestRequestTypeDef = {  # (1)
    "computeEnvironment": ...,
}

parent.delete_compute_environment(**kwargs)
```

1. See [:material-code-braces: DeleteComputeEnvironmentRequestRequestTypeDef](./type_defs.md#deletecomputeenvironmentrequestrequesttypedef) 

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

kwargs: DeleteJobQueueRequestRequestTypeDef = {  # (1)
    "jobQueue": ...,
}

parent.delete_job_queue(**kwargs)
```

1. See [:material-code-braces: DeleteJobQueueRequestRequestTypeDef](./type_defs.md#deletejobqueuerequestrequesttypedef) 

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

kwargs: DeleteSchedulingPolicyRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_scheduling_policy(**kwargs)
```

1. See [:material-code-braces: DeleteSchedulingPolicyRequestRequestTypeDef](./type_defs.md#deleteschedulingpolicyrequestrequesttypedef) 

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

kwargs: DeregisterJobDefinitionRequestRequestTypeDef = {  # (1)
    "jobDefinition": ...,
}

parent.deregister_job_definition(**kwargs)
```

1. See [:material-code-braces: DeregisterJobDefinitionRequestRequestTypeDef](./type_defs.md#deregisterjobdefinitionrequestrequesttypedef) 

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

kwargs: DescribeComputeEnvironmentsRequestRequestTypeDef = {  # (1)
    "computeEnvironments": ...,
}

parent.describe_compute_environments(**kwargs)
```

1. See [:material-code-braces: DescribeComputeEnvironmentsRequestRequestTypeDef](./type_defs.md#describecomputeenvironmentsrequestrequesttypedef) 

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

kwargs: DescribeJobDefinitionsRequestRequestTypeDef = {  # (1)
    "jobDefinitions": ...,
}

parent.describe_job_definitions(**kwargs)
```

1. See [:material-code-braces: DescribeJobDefinitionsRequestRequestTypeDef](./type_defs.md#describejobdefinitionsrequestrequesttypedef) 

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

kwargs: DescribeJobQueuesRequestRequestTypeDef = {  # (1)
    "jobQueues": ...,
}

parent.describe_job_queues(**kwargs)
```

1. See [:material-code-braces: DescribeJobQueuesRequestRequestTypeDef](./type_defs.md#describejobqueuesrequestrequesttypedef) 

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

kwargs: DescribeJobsRequestRequestTypeDef = {  # (1)
    "jobs": ...,
}

parent.describe_jobs(**kwargs)
```

1. See [:material-code-braces: DescribeJobsRequestRequestTypeDef](./type_defs.md#describejobsrequestrequesttypedef) 

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

kwargs: DescribeSchedulingPoliciesRequestRequestTypeDef = {  # (1)
    "arns": ...,
}

parent.describe_scheduling_policies(**kwargs)
```

1. See [:material-code-braces: DescribeSchedulingPoliciesRequestRequestTypeDef](./type_defs.md#describeschedulingpoliciesrequestrequesttypedef) 

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

kwargs: GetJobQueueSnapshotRequestRequestTypeDef = {  # (1)
    "jobQueue": ...,
}

parent.get_job_queue_snapshot(**kwargs)
```

1. See [:material-code-braces: GetJobQueueSnapshotRequestRequestTypeDef](./type_defs.md#getjobqueuesnapshotrequestrequesttypedef) 

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

kwargs: ListJobsRequestRequestTypeDef = {  # (1)
    "jobQueue": ...,
}

parent.list_jobs(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef) 

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

kwargs: ListSchedulingPoliciesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_scheduling_policies(**kwargs)
```

1. See [:material-code-braces: ListSchedulingPoliciesRequestRequestTypeDef](./type_defs.md#listschedulingpoliciesrequestrequesttypedef) 

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

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

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
    containerProperties: ContainerPropertiesTypeDef = ...,  # (2)
    nodeProperties: NodePropertiesTypeDef = ...,  # (3)
    retryStrategy: RetryStrategyTypeDef = ...,  # (4)
    propagateTags: bool = ...,
    timeout: JobTimeoutTypeDef = ...,  # (5)
    tags: Mapping[str, str] = ...,
    platformCapabilities: Sequence[PlatformCapabilityType] = ...,  # (6)
    eksProperties: EksPropertiesTypeDef = ...,  # (7)
    ecsProperties: EcsPropertiesTypeDef = ...,  # (8)
) -> RegisterJobDefinitionResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-brackets: JobDefinitionTypeType](./literals.md#jobdefinitiontypetype) 
2. See [:material-code-braces: ContainerPropertiesTypeDef](./type_defs.md#containerpropertiestypedef) 
3. See [:material-code-braces: NodePropertiesTypeDef](./type_defs.md#nodepropertiestypedef) 
4. See [:material-code-braces: RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef) 
5. See [:material-code-braces: JobTimeoutTypeDef](./type_defs.md#jobtimeouttypedef) 
6. See [:material-code-brackets: PlatformCapabilityType](./literals.md#platformcapabilitytype) 
7. See [:material-code-braces: EksPropertiesTypeDef](./type_defs.md#ekspropertiestypedef) 
8. See [:material-code-braces: EcsPropertiesTypeDef](./type_defs.md#ecspropertiestypedef) 
9. See [:material-code-braces: RegisterJobDefinitionResponseTypeDef](./type_defs.md#registerjobdefinitionresponsetypedef) 


```python
# register_job_definition method usage example with argument unpacking

kwargs: RegisterJobDefinitionRequestRequestTypeDef = {  # (1)
    "jobDefinitionName": ...,
    "type": ...,
}

parent.register_job_definition(**kwargs)
```

1. See [:material-code-braces: RegisterJobDefinitionRequestRequestTypeDef](./type_defs.md#registerjobdefinitionrequestrequesttypedef) 

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
    retryStrategy: RetryStrategyTypeDef = ...,  # (5)
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
5. See [:material-code-braces: RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef) 
6. See [:material-code-braces: JobTimeoutTypeDef](./type_defs.md#jobtimeouttypedef) 
7. See [:material-code-braces: EksPropertiesOverrideTypeDef](./type_defs.md#ekspropertiesoverridetypedef) 
8. See [:material-code-braces: EcsPropertiesOverrideTypeDef](./type_defs.md#ecspropertiesoverridetypedef) 
9. See [:material-code-braces: SubmitJobResponseTypeDef](./type_defs.md#submitjobresponsetypedef) 


```python
# submit_job method usage example with argument unpacking

kwargs: SubmitJobRequestRequestTypeDef = {  # (1)
    "jobName": ...,
    "jobQueue": ...,
    "jobDefinition": ...,
}

parent.submit_job(**kwargs)
```

1. See [:material-code-braces: SubmitJobRequestRequestTypeDef](./type_defs.md#submitjobrequestrequesttypedef) 

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

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

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

kwargs: TerminateJobRequestRequestTypeDef = {  # (1)
    "jobId": ...,
    "reason": ...,
}

parent.terminate_job(**kwargs)
```

1. See [:material-code-braces: TerminateJobRequestRequestTypeDef](./type_defs.md#terminatejobrequestrequesttypedef) 

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

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

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

kwargs: UpdateComputeEnvironmentRequestRequestTypeDef = {  # (1)
    "computeEnvironment": ...,
}

parent.update_compute_environment(**kwargs)
```

1. See [:material-code-braces: UpdateComputeEnvironmentRequestRequestTypeDef](./type_defs.md#updatecomputeenvironmentrequestrequesttypedef) 

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

kwargs: UpdateJobQueueRequestRequestTypeDef = {  # (1)
    "jobQueue": ...,
}

parent.update_job_queue(**kwargs)
```

1. See [:material-code-braces: UpdateJobQueueRequestRequestTypeDef](./type_defs.md#updatejobqueuerequestrequesttypedef) 

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
    fairsharePolicy: FairsharePolicyTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: FairsharePolicyTypeDef](./type_defs.md#fairsharepolicytypedef) 


```python
# update_scheduling_policy method usage example with argument unpacking

kwargs: UpdateSchedulingPolicyRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_scheduling_policy(**kwargs)
```

1. See [:material-code-braces: UpdateSchedulingPolicyRequestRequestTypeDef](./type_defs.md#updateschedulingpolicyrequestrequesttypedef) 

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



