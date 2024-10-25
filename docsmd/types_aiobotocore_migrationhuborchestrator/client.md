# MigrationHubOrchestratorClient

> [Index](../README.md) > [MigrationHubOrchestrator](./README.md) > MigrationHubOrchestratorClient

!!! note ""

    Auto-generated documentation for [MigrationHubOrchestrator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
    type annotations stubs module [types-aiobotocore-migrationhuborchestrator](https://pypi.org/project/types-aiobotocore-migrationhuborchestrator/).

## MigrationHubOrchestratorClient

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client)

```python
# MigrationHubOrchestratorClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_migrationhuborchestrator.client import MigrationHubOrchestratorClient

session = get_session()
async with session.create_client("migrationhuborchestrator") as client:
    client: MigrationHubOrchestratorClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("migrationhuborchestrator").exceptions` structure.

```python
# MigrationHubOrchestratorClient.exceptions usage example

async with session.create_client("migrationhuborchestrator") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# MigrationHubOrchestratorClient usage type checking example

from types_aiobotocore_migrationhuborchestrator.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_template

Creates a migration workflow template.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").create_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_template)

```python
# create_template method definition

await def create_template(
    self,
    *,
    templateName: str,
    templateSource: TemplateSourceTypeDef,  # (1)
    templateDescription: str = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateTemplateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TemplateSourceTypeDef](./type_defs.md#templatesourcetypedef) 
2. See [:material-code-braces: CreateTemplateResponseTypeDef](./type_defs.md#createtemplateresponsetypedef) 


```python
# create_template method usage example with argument unpacking

kwargs: CreateTemplateRequestRequestTypeDef = {  # (1)
    "templateName": ...,
    "templateSource": ...,
}

parent.create_template(**kwargs)
```

1. See [:material-code-braces: CreateTemplateRequestRequestTypeDef](./type_defs.md#createtemplaterequestrequesttypedef) 

### create\_workflow

Create a workflow to orchestrate your migrations.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").create_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow)

```python
# create_workflow method definition

await def create_workflow(
    self,
    *,
    name: str,
    templateId: str,
    inputParameters: Mapping[str, StepInputUnionTypeDef],  # (1)
    description: str = ...,
    applicationConfigurationId: str = ...,
    stepTargets: Sequence[str] = ...,
    tags: Mapping[str, str] = ...,
) -> CreateMigrationWorkflowResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StepInputTypeDef](./type_defs.md#stepinputtypedef) [:material-code-braces: StepInputOutputTypeDef](./type_defs.md#stepinputoutputtypedef) 
2. See [:material-code-braces: CreateMigrationWorkflowResponseTypeDef](./type_defs.md#createmigrationworkflowresponsetypedef) 


```python
# create_workflow method usage example with argument unpacking

kwargs: CreateMigrationWorkflowRequestRequestTypeDef = {  # (1)
    "name": ...,
    "templateId": ...,
    "inputParameters": ...,
}

parent.create_workflow(**kwargs)
```

1. See [:material-code-braces: CreateMigrationWorkflowRequestRequestTypeDef](./type_defs.md#createmigrationworkflowrequestrequesttypedef) 

### create\_workflow\_step

Create a step in the migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").create_workflow_step` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow_step)

```python
# create_workflow_step method definition

await def create_workflow_step(
    self,
    *,
    name: str,
    stepGroupId: str,
    workflowId: str,
    stepActionType: StepActionTypeType,  # (1)
    description: str = ...,
    workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,  # (2)
    stepTarget: Sequence[str] = ...,
    outputs: Sequence[WorkflowStepUnionTypeDef] = ...,  # (3)
    previous: Sequence[str] = ...,
    next: Sequence[str] = ...,
) -> CreateWorkflowStepResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: StepActionTypeType](./literals.md#stepactiontypetype) 
2. See [:material-code-braces: WorkflowStepAutomationConfigurationTypeDef](./type_defs.md#workflowstepautomationconfigurationtypedef) 
3. See [:material-code-braces: WorkflowStepOutputTypeDef](./type_defs.md#workflowstepoutputtypedef) [:material-code-braces: WorkflowStepExtraOutputTypeDef](./type_defs.md#workflowstepextraoutputtypedef) 
4. See [:material-code-braces: CreateWorkflowStepResponseTypeDef](./type_defs.md#createworkflowstepresponsetypedef) 


```python
# create_workflow_step method usage example with argument unpacking

kwargs: CreateWorkflowStepRequestRequestTypeDef = {  # (1)
    "name": ...,
    "stepGroupId": ...,
    "workflowId": ...,
    "stepActionType": ...,
}

parent.create_workflow_step(**kwargs)
```

1. See [:material-code-braces: CreateWorkflowStepRequestRequestTypeDef](./type_defs.md#createworkflowsteprequestrequesttypedef) 

### create\_workflow\_step\_group

Create a step group in a migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").create_workflow_step_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow_step_group)

```python
# create_workflow_step_group method definition

await def create_workflow_step_group(
    self,
    *,
    workflowId: str,
    name: str,
    description: str = ...,
    next: Sequence[str] = ...,
    previous: Sequence[str] = ...,
) -> CreateWorkflowStepGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateWorkflowStepGroupResponseTypeDef](./type_defs.md#createworkflowstepgroupresponsetypedef) 


```python
# create_workflow_step_group method usage example with argument unpacking

kwargs: CreateWorkflowStepGroupRequestRequestTypeDef = {  # (1)
    "workflowId": ...,
    "name": ...,
}

parent.create_workflow_step_group(**kwargs)
```

1. See [:material-code-braces: CreateWorkflowStepGroupRequestRequestTypeDef](./type_defs.md#createworkflowstepgrouprequestrequesttypedef) 

### delete\_template

Deletes a migration workflow template.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").delete_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.delete_template)

```python
# delete_template method definition

await def delete_template(
    self,
    *,
    id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_template method usage example with argument unpacking

kwargs: DeleteTemplateRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_template(**kwargs)
```

1. See [:material-code-braces: DeleteTemplateRequestRequestTypeDef](./type_defs.md#deletetemplaterequestrequesttypedef) 

### delete\_workflow

Delete a migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").delete_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.delete_workflow)

```python
# delete_workflow method definition

await def delete_workflow(
    self,
    *,
    id: str,
) -> DeleteMigrationWorkflowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMigrationWorkflowResponseTypeDef](./type_defs.md#deletemigrationworkflowresponsetypedef) 


```python
# delete_workflow method usage example with argument unpacking

kwargs: DeleteMigrationWorkflowRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_workflow(**kwargs)
```

1. See [:material-code-braces: DeleteMigrationWorkflowRequestRequestTypeDef](./type_defs.md#deletemigrationworkflowrequestrequesttypedef) 

### delete\_workflow\_step

Delete a step in a migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").delete_workflow_step` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.delete_workflow_step)

```python
# delete_workflow_step method definition

await def delete_workflow_step(
    self,
    *,
    id: str,
    stepGroupId: str,
    workflowId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_workflow_step method usage example with argument unpacking

kwargs: DeleteWorkflowStepRequestRequestTypeDef = {  # (1)
    "id": ...,
    "stepGroupId": ...,
    "workflowId": ...,
}

parent.delete_workflow_step(**kwargs)
```

1. See [:material-code-braces: DeleteWorkflowStepRequestRequestTypeDef](./type_defs.md#deleteworkflowsteprequestrequesttypedef) 

### delete\_workflow\_step\_group

Delete a step group in a migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").delete_workflow_step_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.delete_workflow_step_group)

```python
# delete_workflow_step_group method definition

await def delete_workflow_step_group(
    self,
    *,
    workflowId: str,
    id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_workflow_step_group method usage example with argument unpacking

kwargs: DeleteWorkflowStepGroupRequestRequestTypeDef = {  # (1)
    "workflowId": ...,
    "id": ...,
}

parent.delete_workflow_step_group(**kwargs)
```

1. See [:material-code-braces: DeleteWorkflowStepGroupRequestRequestTypeDef](./type_defs.md#deleteworkflowstepgrouprequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.generate_presigned_url)

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


### get\_template

Get the template you want to use for creating a migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.get_template)

```python
# get_template method definition

await def get_template(
    self,
    *,
    id: str,
) -> GetMigrationWorkflowTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMigrationWorkflowTemplateResponseTypeDef](./type_defs.md#getmigrationworkflowtemplateresponsetypedef) 


```python
# get_template method usage example with argument unpacking

kwargs: GetMigrationWorkflowTemplateRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_template(**kwargs)
```

1. See [:material-code-braces: GetMigrationWorkflowTemplateRequestRequestTypeDef](./type_defs.md#getmigrationworkflowtemplaterequestrequesttypedef) 

### get\_template\_step

Get a specific step in a template.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_template_step` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.get_template_step)

```python
# get_template_step method definition

await def get_template_step(
    self,
    *,
    id: str,
    templateId: str,
    stepGroupId: str,
) -> GetTemplateStepResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTemplateStepResponseTypeDef](./type_defs.md#gettemplatestepresponsetypedef) 


```python
# get_template_step method usage example with argument unpacking

kwargs: GetTemplateStepRequestRequestTypeDef = {  # (1)
    "id": ...,
    "templateId": ...,
    "stepGroupId": ...,
}

parent.get_template_step(**kwargs)
```

1. See [:material-code-braces: GetTemplateStepRequestRequestTypeDef](./type_defs.md#gettemplatesteprequestrequesttypedef) 

### get\_template\_step\_group

Get a step group in a template.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_template_step_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.get_template_step_group)

```python
# get_template_step_group method definition

await def get_template_step_group(
    self,
    *,
    templateId: str,
    id: str,
) -> GetTemplateStepGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTemplateStepGroupResponseTypeDef](./type_defs.md#gettemplatestepgroupresponsetypedef) 


```python
# get_template_step_group method usage example with argument unpacking

kwargs: GetTemplateStepGroupRequestRequestTypeDef = {  # (1)
    "templateId": ...,
    "id": ...,
}

parent.get_template_step_group(**kwargs)
```

1. See [:material-code-braces: GetTemplateStepGroupRequestRequestTypeDef](./type_defs.md#gettemplatestepgrouprequestrequesttypedef) 

### get\_workflow

Get migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.get_workflow)

```python
# get_workflow method definition

await def get_workflow(
    self,
    *,
    id: str,
) -> GetMigrationWorkflowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMigrationWorkflowResponseTypeDef](./type_defs.md#getmigrationworkflowresponsetypedef) 


```python
# get_workflow method usage example with argument unpacking

kwargs: GetMigrationWorkflowRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_workflow(**kwargs)
```

1. See [:material-code-braces: GetMigrationWorkflowRequestRequestTypeDef](./type_defs.md#getmigrationworkflowrequestrequesttypedef) 

### get\_workflow\_step

Get a step in the migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_workflow_step` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.get_workflow_step)

```python
# get_workflow_step method definition

await def get_workflow_step(
    self,
    *,
    workflowId: str,
    stepGroupId: str,
    id: str,
) -> GetWorkflowStepResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkflowStepResponseTypeDef](./type_defs.md#getworkflowstepresponsetypedef) 


```python
# get_workflow_step method usage example with argument unpacking

kwargs: GetWorkflowStepRequestRequestTypeDef = {  # (1)
    "workflowId": ...,
    "stepGroupId": ...,
    "id": ...,
}

parent.get_workflow_step(**kwargs)
```

1. See [:material-code-braces: GetWorkflowStepRequestRequestTypeDef](./type_defs.md#getworkflowsteprequestrequesttypedef) 

### get\_workflow\_step\_group

Get the step group of a migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_workflow_step_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.get_workflow_step_group)

```python
# get_workflow_step_group method definition

await def get_workflow_step_group(
    self,
    *,
    id: str,
    workflowId: str,
) -> GetWorkflowStepGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkflowStepGroupResponseTypeDef](./type_defs.md#getworkflowstepgroupresponsetypedef) 


```python
# get_workflow_step_group method usage example with argument unpacking

kwargs: GetWorkflowStepGroupRequestRequestTypeDef = {  # (1)
    "id": ...,
    "workflowId": ...,
}

parent.get_workflow_step_group(**kwargs)
```

1. See [:material-code-braces: GetWorkflowStepGroupRequestRequestTypeDef](./type_defs.md#getworkflowstepgrouprequestrequesttypedef) 

### list\_plugins

List AWS Migration Hub Orchestrator plugins.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").list_plugins` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.list_plugins)

```python
# list_plugins method definition

await def list_plugins(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListPluginsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPluginsResponseTypeDef](./type_defs.md#listpluginsresponsetypedef) 


```python
# list_plugins method usage example with argument unpacking

kwargs: ListPluginsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_plugins(**kwargs)
```

1. See [:material-code-braces: ListPluginsRequestRequestTypeDef](./type_defs.md#listpluginsrequestrequesttypedef) 

### list\_tags\_for\_resource

List the tags added to a resource.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.list_tags_for_resource)

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

### list\_template\_step\_groups

List the step groups in a template.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").list_template_step_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.list_template_step_groups)

```python
# list_template_step_groups method definition

await def list_template_step_groups(
    self,
    *,
    templateId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTemplateStepGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTemplateStepGroupsResponseTypeDef](./type_defs.md#listtemplatestepgroupsresponsetypedef) 


```python
# list_template_step_groups method usage example with argument unpacking

kwargs: ListTemplateStepGroupsRequestRequestTypeDef = {  # (1)
    "templateId": ...,
}

parent.list_template_step_groups(**kwargs)
```

1. See [:material-code-braces: ListTemplateStepGroupsRequestRequestTypeDef](./type_defs.md#listtemplatestepgroupsrequestrequesttypedef) 

### list\_template\_steps

List the steps in a template.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").list_template_steps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.list_template_steps)

```python
# list_template_steps method definition

await def list_template_steps(
    self,
    *,
    templateId: str,
    stepGroupId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTemplateStepsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTemplateStepsResponseTypeDef](./type_defs.md#listtemplatestepsresponsetypedef) 


```python
# list_template_steps method usage example with argument unpacking

kwargs: ListTemplateStepsRequestRequestTypeDef = {  # (1)
    "templateId": ...,
    "stepGroupId": ...,
}

parent.list_template_steps(**kwargs)
```

1. See [:material-code-braces: ListTemplateStepsRequestRequestTypeDef](./type_defs.md#listtemplatestepsrequestrequesttypedef) 

### list\_templates

List the templates available in Migration Hub Orchestrator to create a
migration
workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").list_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.list_templates)

```python
# list_templates method definition

await def list_templates(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    name: str = ...,
) -> ListMigrationWorkflowTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMigrationWorkflowTemplatesResponseTypeDef](./type_defs.md#listmigrationworkflowtemplatesresponsetypedef) 


```python
# list_templates method usage example with argument unpacking

kwargs: ListMigrationWorkflowTemplatesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_templates(**kwargs)
```

1. See [:material-code-braces: ListMigrationWorkflowTemplatesRequestRequestTypeDef](./type_defs.md#listmigrationworkflowtemplatesrequestrequesttypedef) 

### list\_workflow\_step\_groups

List the step groups in a migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").list_workflow_step_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.list_workflow_step_groups)

```python
# list_workflow_step_groups method definition

await def list_workflow_step_groups(
    self,
    *,
    workflowId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListWorkflowStepGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkflowStepGroupsResponseTypeDef](./type_defs.md#listworkflowstepgroupsresponsetypedef) 


```python
# list_workflow_step_groups method usage example with argument unpacking

kwargs: ListWorkflowStepGroupsRequestRequestTypeDef = {  # (1)
    "workflowId": ...,
}

parent.list_workflow_step_groups(**kwargs)
```

1. See [:material-code-braces: ListWorkflowStepGroupsRequestRequestTypeDef](./type_defs.md#listworkflowstepgroupsrequestrequesttypedef) 

### list\_workflow\_steps

List the steps in a workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").list_workflow_steps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.list_workflow_steps)

```python
# list_workflow_steps method definition

await def list_workflow_steps(
    self,
    *,
    workflowId: str,
    stepGroupId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListWorkflowStepsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkflowStepsResponseTypeDef](./type_defs.md#listworkflowstepsresponsetypedef) 


```python
# list_workflow_steps method usage example with argument unpacking

kwargs: ListWorkflowStepsRequestRequestTypeDef = {  # (1)
    "workflowId": ...,
    "stepGroupId": ...,
}

parent.list_workflow_steps(**kwargs)
```

1. See [:material-code-braces: ListWorkflowStepsRequestRequestTypeDef](./type_defs.md#listworkflowstepsrequestrequesttypedef) 

### list\_workflows

List the migration workflows.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").list_workflows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.list_workflows)

```python
# list_workflows method definition

await def list_workflows(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    templateId: str = ...,
    adsApplicationConfigurationName: str = ...,
    status: MigrationWorkflowStatusEnumType = ...,  # (1)
    name: str = ...,
) -> ListMigrationWorkflowsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MigrationWorkflowStatusEnumType](./literals.md#migrationworkflowstatusenumtype) 
2. See [:material-code-braces: ListMigrationWorkflowsResponseTypeDef](./type_defs.md#listmigrationworkflowsresponsetypedef) 


```python
# list_workflows method usage example with argument unpacking

kwargs: ListMigrationWorkflowsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_workflows(**kwargs)
```

1. See [:material-code-braces: ListMigrationWorkflowsRequestRequestTypeDef](./type_defs.md#listmigrationworkflowsrequestrequesttypedef) 

### retry\_workflow\_step

Retry a failed step in a migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").retry_workflow_step` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.retry_workflow_step)

```python
# retry_workflow_step method definition

await def retry_workflow_step(
    self,
    *,
    workflowId: str,
    stepGroupId: str,
    id: str,
) -> RetryWorkflowStepResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RetryWorkflowStepResponseTypeDef](./type_defs.md#retryworkflowstepresponsetypedef) 


```python
# retry_workflow_step method usage example with argument unpacking

kwargs: RetryWorkflowStepRequestRequestTypeDef = {  # (1)
    "workflowId": ...,
    "stepGroupId": ...,
    "id": ...,
}

parent.retry_workflow_step(**kwargs)
```

1. See [:material-code-braces: RetryWorkflowStepRequestRequestTypeDef](./type_defs.md#retryworkflowsteprequestrequesttypedef) 

### start\_workflow

Start a migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").start_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.start_workflow)

```python
# start_workflow method definition

await def start_workflow(
    self,
    *,
    id: str,
) -> StartMigrationWorkflowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMigrationWorkflowResponseTypeDef](./type_defs.md#startmigrationworkflowresponsetypedef) 


```python
# start_workflow method usage example with argument unpacking

kwargs: StartMigrationWorkflowRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.start_workflow(**kwargs)
```

1. See [:material-code-braces: StartMigrationWorkflowRequestRequestTypeDef](./type_defs.md#startmigrationworkflowrequestrequesttypedef) 

### stop\_workflow

Stop an ongoing migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").stop_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.stop_workflow)

```python
# stop_workflow method definition

await def stop_workflow(
    self,
    *,
    id: str,
) -> StopMigrationWorkflowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopMigrationWorkflowResponseTypeDef](./type_defs.md#stopmigrationworkflowresponsetypedef) 


```python
# stop_workflow method usage example with argument unpacking

kwargs: StopMigrationWorkflowRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.stop_workflow(**kwargs)
```

1. See [:material-code-braces: StopMigrationWorkflowRequestRequestTypeDef](./type_defs.md#stopmigrationworkflowrequestrequesttypedef) 

### tag\_resource

Tag a resource by specifying its Amazon Resource Name (ARN).

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.tag_resource)

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

### untag\_resource

Deletes the tags for a resource.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.untag_resource)

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

### update\_template

Updates a migration workflow template.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").update_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_template)

```python
# update_template method definition

await def update_template(
    self,
    *,
    id: str,
    templateName: str = ...,
    templateDescription: str = ...,
    clientToken: str = ...,
) -> UpdateTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateTemplateResponseTypeDef](./type_defs.md#updatetemplateresponsetypedef) 


```python
# update_template method usage example with argument unpacking

kwargs: UpdateTemplateRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.update_template(**kwargs)
```

1. See [:material-code-braces: UpdateTemplateRequestRequestTypeDef](./type_defs.md#updatetemplaterequestrequesttypedef) 

### update\_workflow

Update a migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").update_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow)

```python
# update_workflow method definition

await def update_workflow(
    self,
    *,
    id: str,
    name: str = ...,
    description: str = ...,
    inputParameters: Mapping[str, StepInputTypeDef] = ...,  # (1)
    stepTargets: Sequence[str] = ...,
) -> UpdateMigrationWorkflowResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StepInputTypeDef](./type_defs.md#stepinputtypedef) 
2. See [:material-code-braces: UpdateMigrationWorkflowResponseTypeDef](./type_defs.md#updatemigrationworkflowresponsetypedef) 


```python
# update_workflow method usage example with argument unpacking

kwargs: UpdateMigrationWorkflowRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.update_workflow(**kwargs)
```

1. See [:material-code-braces: UpdateMigrationWorkflowRequestRequestTypeDef](./type_defs.md#updatemigrationworkflowrequestrequesttypedef) 

### update\_workflow\_step

Update a step in a migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").update_workflow_step` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow_step)

```python
# update_workflow_step method definition

await def update_workflow_step(
    self,
    *,
    id: str,
    stepGroupId: str,
    workflowId: str,
    name: str = ...,
    description: str = ...,
    stepActionType: StepActionTypeType = ...,  # (1)
    workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,  # (2)
    stepTarget: Sequence[str] = ...,
    outputs: Sequence[WorkflowStepOutputTypeDef] = ...,  # (3)
    previous: Sequence[str] = ...,
    next: Sequence[str] = ...,
    status: StepStatusType = ...,  # (4)
) -> UpdateWorkflowStepResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: StepActionTypeType](./literals.md#stepactiontypetype) 
2. See [:material-code-braces: WorkflowStepAutomationConfigurationTypeDef](./type_defs.md#workflowstepautomationconfigurationtypedef) 
3. See [:material-code-braces: WorkflowStepOutputTypeDef](./type_defs.md#workflowstepoutputtypedef) 
4. See [:material-code-brackets: StepStatusType](./literals.md#stepstatustype) 
5. See [:material-code-braces: UpdateWorkflowStepResponseTypeDef](./type_defs.md#updateworkflowstepresponsetypedef) 


```python
# update_workflow_step method usage example with argument unpacking

kwargs: UpdateWorkflowStepRequestRequestTypeDef = {  # (1)
    "id": ...,
    "stepGroupId": ...,
    "workflowId": ...,
}

parent.update_workflow_step(**kwargs)
```

1. See [:material-code-braces: UpdateWorkflowStepRequestRequestTypeDef](./type_defs.md#updateworkflowsteprequestrequesttypedef) 

### update\_workflow\_step\_group

Update the step group in a migration workflow.

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").update_workflow_step_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow_step_group)

```python
# update_workflow_step_group method definition

await def update_workflow_step_group(
    self,
    *,
    workflowId: str,
    id: str,
    name: str = ...,
    description: str = ...,
    next: Sequence[str] = ...,
    previous: Sequence[str] = ...,
) -> UpdateWorkflowStepGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateWorkflowStepGroupResponseTypeDef](./type_defs.md#updateworkflowstepgroupresponsetypedef) 


```python
# update_workflow_step_group method usage example with argument unpacking

kwargs: UpdateWorkflowStepGroupRequestRequestTypeDef = {  # (1)
    "workflowId": ...,
    "id": ...,
}

parent.update_workflow_step_group(**kwargs)
```

1. See [:material-code-braces: UpdateWorkflowStepGroupRequestRequestTypeDef](./type_defs.md#updateworkflowstepgrouprequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "MigrationHubOrchestratorClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("migrationhuborchestrator").get_paginator` method with overloads.

- `client.get_paginator("list_plugins")` -> [ListPluginsPaginator](./paginators.md#listpluginspaginator)
- `client.get_paginator("list_template_step_groups")` -> [ListTemplateStepGroupsPaginator](./paginators.md#listtemplatestepgroupspaginator)
- `client.get_paginator("list_template_steps")` -> [ListTemplateStepsPaginator](./paginators.md#listtemplatestepspaginator)
- `client.get_paginator("list_templates")` -> [ListTemplatesPaginator](./paginators.md#listtemplatespaginator)
- `client.get_paginator("list_workflow_step_groups")` -> [ListWorkflowStepGroupsPaginator](./paginators.md#listworkflowstepgroupspaginator)
- `client.get_paginator("list_workflow_steps")` -> [ListWorkflowStepsPaginator](./paginators.md#listworkflowstepspaginator)
- `client.get_paginator("list_workflows")` -> [ListWorkflowsPaginator](./paginators.md#listworkflowspaginator)



