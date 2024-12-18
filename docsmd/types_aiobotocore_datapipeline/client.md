# DataPipelineClient

> [Index](../README.md) > [DataPipeline](./README.md) > DataPipelineClient

!!! note ""

    Auto-generated documentation for [DataPipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#datapipeline)
    type annotations stubs module [types-aiobotocore-datapipeline](https://pypi.org/project/types-aiobotocore-datapipeline/).

## DataPipelineClient

Type annotations and code completion for `#!python session.create_client("datapipeline")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client)

```python
# DataPipelineClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_datapipeline.client import DataPipelineClient

session = get_session()
async with session.create_client("datapipeline") as client:
    client: DataPipelineClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("datapipeline").exceptions` structure.

```python
# DataPipelineClient.exceptions usage example

async with session.create_client("datapipeline") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalServiceError,
        client.InvalidRequestException,
        client.PipelineDeletedException,
        client.PipelineNotFoundException,
        client.TaskNotFoundException,
    ) as e:
        print(e)
```

```python
# DataPipelineClient usage type checking example

from types_aiobotocore_datapipeline.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("datapipeline").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("datapipeline").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/generate_presigned_url.html)

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


### close



Type annotations and code completion for `#!python session.create_client("datapipeline").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### activate\_pipeline

Validates the specified pipeline and starts processing pipeline tasks.

Type annotations and code completion for `#!python session.create_client("datapipeline").activate_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/activate_pipeline.html)

```python
# activate_pipeline method definition

await def activate_pipeline(
    self,
    *,
    pipelineId: str,
    parameterValues: Sequence[ParameterValueTypeDef] = ...,  # (1)
    startTimestamp: TimestampTypeDef = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ParameterValueTypeDef](./type_defs.md#parametervaluetypedef) 


```python
# activate_pipeline method usage example with argument unpacking

kwargs: ActivatePipelineInputRequestTypeDef = {  # (1)
    "pipelineId": ...,
}

parent.activate_pipeline(**kwargs)
```

1. See [:material-code-braces: ActivatePipelineInputRequestTypeDef](./type_defs.md#activatepipelineinputrequesttypedef) 

### add\_tags

Adds or modifies tags for the specified pipeline.

Type annotations and code completion for `#!python session.create_client("datapipeline").add_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/add_tags.html)

```python
# add_tags method definition

await def add_tags(
    self,
    *,
    pipelineId: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# add_tags method usage example with argument unpacking

kwargs: AddTagsInputRequestTypeDef = {  # (1)
    "pipelineId": ...,
    "tags": ...,
}

parent.add_tags(**kwargs)
```

1. See [:material-code-braces: AddTagsInputRequestTypeDef](./type_defs.md#addtagsinputrequesttypedef) 

### create\_pipeline

Creates a new, empty pipeline.

Type annotations and code completion for `#!python session.create_client("datapipeline").create_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/create_pipeline.html)

```python
# create_pipeline method definition

await def create_pipeline(
    self,
    *,
    name: str,
    uniqueId: str,
    description: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreatePipelineOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreatePipelineOutputTypeDef](./type_defs.md#createpipelineoutputtypedef) 


```python
# create_pipeline method usage example with argument unpacking

kwargs: CreatePipelineInputRequestTypeDef = {  # (1)
    "name": ...,
    "uniqueId": ...,
}

parent.create_pipeline(**kwargs)
```

1. See [:material-code-braces: CreatePipelineInputRequestTypeDef](./type_defs.md#createpipelineinputrequesttypedef) 

### deactivate\_pipeline

Deactivates the specified running pipeline.

Type annotations and code completion for `#!python session.create_client("datapipeline").deactivate_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/deactivate_pipeline.html)

```python
# deactivate_pipeline method definition

await def deactivate_pipeline(
    self,
    *,
    pipelineId: str,
    cancelActive: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# deactivate_pipeline method usage example with argument unpacking

kwargs: DeactivatePipelineInputRequestTypeDef = {  # (1)
    "pipelineId": ...,
}

parent.deactivate_pipeline(**kwargs)
```

1. See [:material-code-braces: DeactivatePipelineInputRequestTypeDef](./type_defs.md#deactivatepipelineinputrequesttypedef) 

### delete\_pipeline

Deletes a pipeline, its pipeline definition, and its run history.

Type annotations and code completion for `#!python session.create_client("datapipeline").delete_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/delete_pipeline.html)

```python
# delete_pipeline method definition

await def delete_pipeline(
    self,
    *,
    pipelineId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_pipeline method usage example with argument unpacking

kwargs: DeletePipelineInputRequestTypeDef = {  # (1)
    "pipelineId": ...,
}

parent.delete_pipeline(**kwargs)
```

1. See [:material-code-braces: DeletePipelineInputRequestTypeDef](./type_defs.md#deletepipelineinputrequesttypedef) 

### describe\_objects

Gets the object definitions for a set of objects associated with the pipeline.

Type annotations and code completion for `#!python session.create_client("datapipeline").describe_objects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/describe_objects.html)

```python
# describe_objects method definition

await def describe_objects(
    self,
    *,
    pipelineId: str,
    objectIds: Sequence[str],
    evaluateExpressions: bool = ...,
    marker: str = ...,
) -> DescribeObjectsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeObjectsOutputTypeDef](./type_defs.md#describeobjectsoutputtypedef) 


```python
# describe_objects method usage example with argument unpacking

kwargs: DescribeObjectsInputRequestTypeDef = {  # (1)
    "pipelineId": ...,
    "objectIds": ...,
}

parent.describe_objects(**kwargs)
```

1. See [:material-code-braces: DescribeObjectsInputRequestTypeDef](./type_defs.md#describeobjectsinputrequesttypedef) 

### describe\_pipelines

Retrieves metadata about one or more pipelines.

Type annotations and code completion for `#!python session.create_client("datapipeline").describe_pipelines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/describe_pipelines.html)

```python
# describe_pipelines method definition

await def describe_pipelines(
    self,
    *,
    pipelineIds: Sequence[str],
) -> DescribePipelinesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePipelinesOutputTypeDef](./type_defs.md#describepipelinesoutputtypedef) 


```python
# describe_pipelines method usage example with argument unpacking

kwargs: DescribePipelinesInputRequestTypeDef = {  # (1)
    "pipelineIds": ...,
}

parent.describe_pipelines(**kwargs)
```

1. See [:material-code-braces: DescribePipelinesInputRequestTypeDef](./type_defs.md#describepipelinesinputrequesttypedef) 

### evaluate\_expression

Task runners call <code>EvaluateExpression</code> to evaluate a string in the
context of the specified object.

Type annotations and code completion for `#!python session.create_client("datapipeline").evaluate_expression` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/evaluate_expression.html)

```python
# evaluate_expression method definition

await def evaluate_expression(
    self,
    *,
    pipelineId: str,
    objectId: str,
    expression: str,
) -> EvaluateExpressionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EvaluateExpressionOutputTypeDef](./type_defs.md#evaluateexpressionoutputtypedef) 


```python
# evaluate_expression method usage example with argument unpacking

kwargs: EvaluateExpressionInputRequestTypeDef = {  # (1)
    "pipelineId": ...,
    "objectId": ...,
    "expression": ...,
}

parent.evaluate_expression(**kwargs)
```

1. See [:material-code-braces: EvaluateExpressionInputRequestTypeDef](./type_defs.md#evaluateexpressioninputrequesttypedef) 

### get\_pipeline\_definition

Gets the definition of the specified pipeline.

Type annotations and code completion for `#!python session.create_client("datapipeline").get_pipeline_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/get_pipeline_definition.html)

```python
# get_pipeline_definition method definition

await def get_pipeline_definition(
    self,
    *,
    pipelineId: str,
    version: str = ...,
) -> GetPipelineDefinitionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPipelineDefinitionOutputTypeDef](./type_defs.md#getpipelinedefinitionoutputtypedef) 


```python
# get_pipeline_definition method usage example with argument unpacking

kwargs: GetPipelineDefinitionInputRequestTypeDef = {  # (1)
    "pipelineId": ...,
}

parent.get_pipeline_definition(**kwargs)
```

1. See [:material-code-braces: GetPipelineDefinitionInputRequestTypeDef](./type_defs.md#getpipelinedefinitioninputrequesttypedef) 

### list\_pipelines

Lists the pipeline identifiers for all active pipelines that you have
permission to access.

Type annotations and code completion for `#!python session.create_client("datapipeline").list_pipelines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/list_pipelines.html)

```python
# list_pipelines method definition

await def list_pipelines(
    self,
    *,
    marker: str = ...,
) -> ListPipelinesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPipelinesOutputTypeDef](./type_defs.md#listpipelinesoutputtypedef) 


```python
# list_pipelines method usage example with argument unpacking

kwargs: ListPipelinesInputRequestTypeDef = {  # (1)
    "marker": ...,
}

parent.list_pipelines(**kwargs)
```

1. See [:material-code-braces: ListPipelinesInputRequestTypeDef](./type_defs.md#listpipelinesinputrequesttypedef) 

### poll\_for\_task

Task runners call <code>PollForTask</code> to receive a task to perform from
AWS Data Pipeline.

Type annotations and code completion for `#!python session.create_client("datapipeline").poll_for_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/poll_for_task.html)

```python
# poll_for_task method definition

await def poll_for_task(
    self,
    *,
    workerGroup: str,
    hostname: str = ...,
    instanceIdentity: InstanceIdentityTypeDef = ...,  # (1)
) -> PollForTaskOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InstanceIdentityTypeDef](./type_defs.md#instanceidentitytypedef) 
2. See [:material-code-braces: PollForTaskOutputTypeDef](./type_defs.md#pollfortaskoutputtypedef) 


```python
# poll_for_task method usage example with argument unpacking

kwargs: PollForTaskInputRequestTypeDef = {  # (1)
    "workerGroup": ...,
}

parent.poll_for_task(**kwargs)
```

1. See [:material-code-braces: PollForTaskInputRequestTypeDef](./type_defs.md#pollfortaskinputrequesttypedef) 

### put\_pipeline\_definition

Adds tasks, schedules, and preconditions to the specified pipeline.

Type annotations and code completion for `#!python session.create_client("datapipeline").put_pipeline_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/put_pipeline_definition.html)

```python
# put_pipeline_definition method definition

await def put_pipeline_definition(
    self,
    *,
    pipelineId: str,
    pipelineObjects: Sequence[PipelineObjectUnionTypeDef],  # (1)
    parameterObjects: Sequence[ParameterObjectUnionTypeDef] = ...,  # (2)
    parameterValues: Sequence[ParameterValueTypeDef] = ...,  # (3)
) -> PutPipelineDefinitionOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: PipelineObjectTypeDef](./type_defs.md#pipelineobjecttypedef) [:material-code-braces: PipelineObjectOutputTypeDef](./type_defs.md#pipelineobjectoutputtypedef) 
2. See [:material-code-braces: ParameterObjectTypeDef](./type_defs.md#parameterobjecttypedef) [:material-code-braces: ParameterObjectOutputTypeDef](./type_defs.md#parameterobjectoutputtypedef) 
3. See [:material-code-braces: ParameterValueTypeDef](./type_defs.md#parametervaluetypedef) 
4. See [:material-code-braces: PutPipelineDefinitionOutputTypeDef](./type_defs.md#putpipelinedefinitionoutputtypedef) 


```python
# put_pipeline_definition method usage example with argument unpacking

kwargs: PutPipelineDefinitionInputRequestTypeDef = {  # (1)
    "pipelineId": ...,
    "pipelineObjects": ...,
}

parent.put_pipeline_definition(**kwargs)
```

1. See [:material-code-braces: PutPipelineDefinitionInputRequestTypeDef](./type_defs.md#putpipelinedefinitioninputrequesttypedef) 

### query\_objects

Queries the specified pipeline for the names of objects that match the
specified set of conditions.

Type annotations and code completion for `#!python session.create_client("datapipeline").query_objects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/query_objects.html)

```python
# query_objects method definition

await def query_objects(
    self,
    *,
    pipelineId: str,
    sphere: str,
    query: QueryTypeDef = ...,  # (1)
    marker: str = ...,
    limit: int = ...,
) -> QueryObjectsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: QueryTypeDef](./type_defs.md#querytypedef) 
2. See [:material-code-braces: QueryObjectsOutputTypeDef](./type_defs.md#queryobjectsoutputtypedef) 


```python
# query_objects method usage example with argument unpacking

kwargs: QueryObjectsInputRequestTypeDef = {  # (1)
    "pipelineId": ...,
    "sphere": ...,
}

parent.query_objects(**kwargs)
```

1. See [:material-code-braces: QueryObjectsInputRequestTypeDef](./type_defs.md#queryobjectsinputrequesttypedef) 

### remove\_tags

Removes existing tags from the specified pipeline.

Type annotations and code completion for `#!python session.create_client("datapipeline").remove_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/remove_tags.html)

```python
# remove_tags method definition

await def remove_tags(
    self,
    *,
    pipelineId: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# remove_tags method usage example with argument unpacking

kwargs: RemoveTagsInputRequestTypeDef = {  # (1)
    "pipelineId": ...,
    "tagKeys": ...,
}

parent.remove_tags(**kwargs)
```

1. See [:material-code-braces: RemoveTagsInputRequestTypeDef](./type_defs.md#removetagsinputrequesttypedef) 

### report\_task\_progress

Task runners call <code>ReportTaskProgress</code> when assigned a task to
acknowledge that it has the task.

Type annotations and code completion for `#!python session.create_client("datapipeline").report_task_progress` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/report_task_progress.html)

```python
# report_task_progress method definition

await def report_task_progress(
    self,
    *,
    taskId: str,
    fields: Sequence[FieldTypeDef] = ...,  # (1)
) -> ReportTaskProgressOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
2. See [:material-code-braces: ReportTaskProgressOutputTypeDef](./type_defs.md#reporttaskprogressoutputtypedef) 


```python
# report_task_progress method usage example with argument unpacking

kwargs: ReportTaskProgressInputRequestTypeDef = {  # (1)
    "taskId": ...,
}

parent.report_task_progress(**kwargs)
```

1. See [:material-code-braces: ReportTaskProgressInputRequestTypeDef](./type_defs.md#reporttaskprogressinputrequesttypedef) 

### report\_task\_runner\_heartbeat

Task runners call <code>ReportTaskRunnerHeartbeat</code> every 15 minutes to
indicate that they are operational.

Type annotations and code completion for `#!python session.create_client("datapipeline").report_task_runner_heartbeat` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/report_task_runner_heartbeat.html)

```python
# report_task_runner_heartbeat method definition

await def report_task_runner_heartbeat(
    self,
    *,
    taskrunnerId: str,
    workerGroup: str = ...,
    hostname: str = ...,
) -> ReportTaskRunnerHeartbeatOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ReportTaskRunnerHeartbeatOutputTypeDef](./type_defs.md#reporttaskrunnerheartbeatoutputtypedef) 


```python
# report_task_runner_heartbeat method usage example with argument unpacking

kwargs: ReportTaskRunnerHeartbeatInputRequestTypeDef = {  # (1)
    "taskrunnerId": ...,
}

parent.report_task_runner_heartbeat(**kwargs)
```

1. See [:material-code-braces: ReportTaskRunnerHeartbeatInputRequestTypeDef](./type_defs.md#reporttaskrunnerheartbeatinputrequesttypedef) 

### set\_status

Requests that the status of the specified physical or logical pipeline objects
be updated in the specified pipeline.

Type annotations and code completion for `#!python session.create_client("datapipeline").set_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/set_status.html)

```python
# set_status method definition

await def set_status(
    self,
    *,
    pipelineId: str,
    objectIds: Sequence[str],
    status: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_status method usage example with argument unpacking

kwargs: SetStatusInputRequestTypeDef = {  # (1)
    "pipelineId": ...,
    "objectIds": ...,
    "status": ...,
}

parent.set_status(**kwargs)
```

1. See [:material-code-braces: SetStatusInputRequestTypeDef](./type_defs.md#setstatusinputrequesttypedef) 

### set\_task\_status

Task runners call <code>SetTaskStatus</code> to notify AWS Data Pipeline that a
task is completed and provide information about the final status.

Type annotations and code completion for `#!python session.create_client("datapipeline").set_task_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/set_task_status.html)

```python
# set_task_status method definition

await def set_task_status(
    self,
    *,
    taskId: str,
    taskStatus: TaskStatusType,  # (1)
    errorId: str = ...,
    errorMessage: str = ...,
    errorStackTrace: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 


```python
# set_task_status method usage example with argument unpacking

kwargs: SetTaskStatusInputRequestTypeDef = {  # (1)
    "taskId": ...,
    "taskStatus": ...,
}

parent.set_task_status(**kwargs)
```

1. See [:material-code-braces: SetTaskStatusInputRequestTypeDef](./type_defs.md#settaskstatusinputrequesttypedef) 

### validate\_pipeline\_definition

Validates the specified pipeline definition to ensure that it is well formed
and can be run without error.

Type annotations and code completion for `#!python session.create_client("datapipeline").validate_pipeline_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/client/validate_pipeline_definition.html)

```python
# validate_pipeline_definition method definition

await def validate_pipeline_definition(
    self,
    *,
    pipelineId: str,
    pipelineObjects: Sequence[PipelineObjectTypeDef],  # (1)
    parameterObjects: Sequence[ParameterObjectTypeDef] = ...,  # (2)
    parameterValues: Sequence[ParameterValueTypeDef] = ...,  # (3)
) -> ValidatePipelineDefinitionOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: PipelineObjectTypeDef](./type_defs.md#pipelineobjecttypedef) 
2. See [:material-code-braces: ParameterObjectTypeDef](./type_defs.md#parameterobjecttypedef) 
3. See [:material-code-braces: ParameterValueTypeDef](./type_defs.md#parametervaluetypedef) 
4. See [:material-code-braces: ValidatePipelineDefinitionOutputTypeDef](./type_defs.md#validatepipelinedefinitionoutputtypedef) 


```python
# validate_pipeline_definition method usage example with argument unpacking

kwargs: ValidatePipelineDefinitionInputRequestTypeDef = {  # (1)
    "pipelineId": ...,
    "pipelineObjects": ...,
}

parent.validate_pipeline_definition(**kwargs)
```

1. See [:material-code-braces: ValidatePipelineDefinitionInputRequestTypeDef](./type_defs.md#validatepipelinedefinitioninputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("datapipeline").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "DataPipelineClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("datapipeline").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("datapipeline").get_paginator` method with overloads.

- `client.get_paginator("describe_objects")` -> [DescribeObjectsPaginator](./paginators.md#describeobjectspaginator)
- `client.get_paginator("list_pipelines")` -> [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
- `client.get_paginator("query_objects")` -> [QueryObjectsPaginator](./paginators.md#queryobjectspaginator)



