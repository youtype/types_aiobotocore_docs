# LaunchWizardClient

> [Index](../README.md) > [LaunchWizard](./README.md) > LaunchWizardClient

!!! note ""

    Auto-generated documentation for [LaunchWizard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#launchwizard)
    type annotations stubs module [types-aiobotocore-launch-wizard](https://pypi.org/project/types-aiobotocore-launch-wizard/).

## LaunchWizardClient

Type annotations and code completion for `#!python session.create_client("launch-wizard")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client)

```python
# LaunchWizardClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_launch_wizard.client import LaunchWizardClient

session = get_session()
async with session.create_client("launch-wizard") as client:
    client: LaunchWizardClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("launch-wizard").exceptions` structure.

```python
# LaunchWizardClient.exceptions usage example

async with session.create_client("launch-wizard") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalServerException,
        client.ResourceLimitException,
        client.ResourceNotFoundException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# LaunchWizardClient usage type checking example

from types_aiobotocore_launch_wizard.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("launch-wizard").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("launch-wizard").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/generate_presigned_url.html)

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


### create\_deployment

Creates a deployment for the given workload.

Type annotations and code completion for `#!python session.create_client("launch-wizard").create_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/create_deployment.html)

```python
# create_deployment method definition

await def create_deployment(
    self,
    *,
    deploymentPatternName: str,
    name: str,
    specifications: Mapping[str, str],
    workloadName: str,
    dryRun: bool = ...,
    tags: Mapping[str, str] = ...,
) -> CreateDeploymentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateDeploymentOutputTypeDef](./type_defs.md#createdeploymentoutputtypedef) 


```python
# create_deployment method usage example with argument unpacking

kwargs: CreateDeploymentInputTypeDef = {  # (1)
    "deploymentPatternName": ...,
    "name": ...,
    "specifications": ...,
    "workloadName": ...,
}

parent.create_deployment(**kwargs)
```

1. See [:material-code-braces: CreateDeploymentInputTypeDef](./type_defs.md#createdeploymentinputtypedef) 

### delete\_deployment

Deletes a deployment.

Type annotations and code completion for `#!python session.create_client("launch-wizard").delete_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/delete_deployment.html)

```python
# delete_deployment method definition

await def delete_deployment(
    self,
    *,
    deploymentId: str,
) -> DeleteDeploymentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDeploymentOutputTypeDef](./type_defs.md#deletedeploymentoutputtypedef) 


```python
# delete_deployment method usage example with argument unpacking

kwargs: DeleteDeploymentInputTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.delete_deployment(**kwargs)
```

1. See [:material-code-braces: DeleteDeploymentInputTypeDef](./type_defs.md#deletedeploymentinputtypedef) 

### get\_deployment

Returns information about the deployment.

Type annotations and code completion for `#!python session.create_client("launch-wizard").get_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/get_deployment.html)

```python
# get_deployment method definition

await def get_deployment(
    self,
    *,
    deploymentId: str,
) -> GetDeploymentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeploymentOutputTypeDef](./type_defs.md#getdeploymentoutputtypedef) 


```python
# get_deployment method usage example with argument unpacking

kwargs: GetDeploymentInputTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.get_deployment(**kwargs)
```

1. See [:material-code-braces: GetDeploymentInputTypeDef](./type_defs.md#getdeploymentinputtypedef) 

### get\_workload

Returns information about a workload.

Type annotations and code completion for `#!python session.create_client("launch-wizard").get_workload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/get_workload.html)

```python
# get_workload method definition

await def get_workload(
    self,
    *,
    workloadName: str,
) -> GetWorkloadOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkloadOutputTypeDef](./type_defs.md#getworkloadoutputtypedef) 


```python
# get_workload method usage example with argument unpacking

kwargs: GetWorkloadInputTypeDef = {  # (1)
    "workloadName": ...,
}

parent.get_workload(**kwargs)
```

1. See [:material-code-braces: GetWorkloadInputTypeDef](./type_defs.md#getworkloadinputtypedef) 

### get\_workload\_deployment\_pattern

Returns details for a given workload and deployment pattern, including the
available specifications.

Type annotations and code completion for `#!python session.create_client("launch-wizard").get_workload_deployment_pattern` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/get_workload_deployment_pattern.html)

```python
# get_workload_deployment_pattern method definition

await def get_workload_deployment_pattern(
    self,
    *,
    deploymentPatternName: str,
    workloadName: str,
) -> GetWorkloadDeploymentPatternOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkloadDeploymentPatternOutputTypeDef](./type_defs.md#getworkloaddeploymentpatternoutputtypedef) 


```python
# get_workload_deployment_pattern method usage example with argument unpacking

kwargs: GetWorkloadDeploymentPatternInputTypeDef = {  # (1)
    "deploymentPatternName": ...,
    "workloadName": ...,
}

parent.get_workload_deployment_pattern(**kwargs)
```

1. See [:material-code-braces: GetWorkloadDeploymentPatternInputTypeDef](./type_defs.md#getworkloaddeploymentpatterninputtypedef) 

### list\_deployment\_events

Lists the events of a deployment.

Type annotations and code completion for `#!python session.create_client("launch-wizard").list_deployment_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/list_deployment_events.html)

```python
# list_deployment_events method definition

await def list_deployment_events(
    self,
    *,
    deploymentId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDeploymentEventsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDeploymentEventsOutputTypeDef](./type_defs.md#listdeploymenteventsoutputtypedef) 


```python
# list_deployment_events method usage example with argument unpacking

kwargs: ListDeploymentEventsInputTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.list_deployment_events(**kwargs)
```

1. See [:material-code-braces: ListDeploymentEventsInputTypeDef](./type_defs.md#listdeploymenteventsinputtypedef) 

### list\_deployments

Lists the deployments that have been created.

Type annotations and code completion for `#!python session.create_client("launch-wizard").list_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/list_deployments.html)

```python
# list_deployments method definition

await def list_deployments(
    self,
    *,
    filters: Sequence[DeploymentFilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDeploymentsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeploymentFilterTypeDef](./type_defs.md#deploymentfiltertypedef) 
2. See [:material-code-braces: ListDeploymentsOutputTypeDef](./type_defs.md#listdeploymentsoutputtypedef) 


```python
# list_deployments method usage example with argument unpacking

kwargs: ListDeploymentsInputTypeDef = {  # (1)
    "filters": ...,
}

parent.list_deployments(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsInputTypeDef](./type_defs.md#listdeploymentsinputtypedef) 

### list\_tags\_for\_resource

Lists the tags associated with a specified resource.

Type annotations and code completion for `#!python session.create_client("launch-wizard").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef) 

### list\_workload\_deployment\_patterns

Lists the workload deployment patterns for a given workload name.

Type annotations and code completion for `#!python session.create_client("launch-wizard").list_workload_deployment_patterns` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/list_workload_deployment_patterns.html)

```python
# list_workload_deployment_patterns method definition

await def list_workload_deployment_patterns(
    self,
    *,
    workloadName: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkloadDeploymentPatternsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkloadDeploymentPatternsOutputTypeDef](./type_defs.md#listworkloaddeploymentpatternsoutputtypedef) 


```python
# list_workload_deployment_patterns method usage example with argument unpacking

kwargs: ListWorkloadDeploymentPatternsInputTypeDef = {  # (1)
    "workloadName": ...,
}

parent.list_workload_deployment_patterns(**kwargs)
```

1. See [:material-code-braces: ListWorkloadDeploymentPatternsInputTypeDef](./type_defs.md#listworkloaddeploymentpatternsinputtypedef) 

### list\_workloads

Lists the available workload names.

Type annotations and code completion for `#!python session.create_client("launch-wizard").list_workloads` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/list_workloads.html)

```python
# list_workloads method definition

await def list_workloads(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkloadsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkloadsOutputTypeDef](./type_defs.md#listworkloadsoutputtypedef) 


```python
# list_workloads method usage example with argument unpacking

kwargs: ListWorkloadsInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_workloads(**kwargs)
```

1. See [:material-code-braces: ListWorkloadsInputTypeDef](./type_defs.md#listworkloadsinputtypedef) 

### tag\_resource

Adds the specified tags to the given resource.

Type annotations and code completion for `#!python session.create_client("launch-wizard").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/tag_resource.html)

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

kwargs: TagResourceInputTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef) 

### untag\_resource

Removes the specified tags from the given resource.

Type annotations and code completion for `#!python session.create_client("launch-wizard").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard/client/untag_resource.html)

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

kwargs: UntagResourceInputTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("launch-wizard").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("launch-wizard").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client)

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

Type annotations and code completion for `#!python session.create_client("launch-wizard").get_paginator` method with overloads.

- `client.get_paginator("list_deployment_events")` -> [ListDeploymentEventsPaginator](./paginators.md#listdeploymenteventspaginator)
- `client.get_paginator("list_deployments")` -> [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
- `client.get_paginator("list_workload_deployment_patterns")` -> [ListWorkloadDeploymentPatternsPaginator](./paginators.md#listworkloaddeploymentpatternspaginator)
- `client.get_paginator("list_workloads")` -> [ListWorkloadsPaginator](./paginators.md#listworkloadspaginator)



