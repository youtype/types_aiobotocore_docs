# FISClient

> [Index](../README.md) > [FIS](./README.md) > FISClient

!!! note ""

    Auto-generated documentation for [FIS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
    type annotations stubs module [types-aiobotocore-fis](https://pypi.org/project/types-aiobotocore-fis/).

## FISClient

Type annotations and code completion for `#!python session.create_client("fis")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client)

```python
FISClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_fis.client import FISClient

session = get_session()
async with session.create_client("fis") as client:
    client: FISClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("fis").exceptions` structure.

```python
FISClient.exceptions usage example

async with session.create_client("fis") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConflictException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
FISClient usage type checking example

from types_aiobotocore_fis.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("fis").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("fis").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_experiment\_template

Creates an experiment template.

Type annotations and code completion for `#!python session.create_client("fis").create_experiment_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.create_experiment_template)

```python
# create_experiment_template method definition

await def create_experiment_template(
    self,
    *,
    clientToken: str,
    description: str,
    stopConditions: Sequence[CreateExperimentTemplateStopConditionInputTypeDef],  # (1)
    actions: Mapping[str, CreateExperimentTemplateActionInputTypeDef],  # (2)
    roleArn: str,
    targets: Mapping[str, CreateExperimentTemplateTargetInputTypeDef] = ...,  # (3)
    tags: Mapping[str, str] = ...,
    logConfiguration: CreateExperimentTemplateLogConfigurationInputTypeDef = ...,  # (4)
) -> CreateExperimentTemplateResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: CreateExperimentTemplateStopConditionInputTypeDef](./type_defs.md#createexperimenttemplatestopconditioninputtypedef) 
2. See [:material-code-braces: CreateExperimentTemplateActionInputTypeDef](./type_defs.md#createexperimenttemplateactioninputtypedef) 
3. See [:material-code-braces: CreateExperimentTemplateTargetInputTypeDef](./type_defs.md#createexperimenttemplatetargetinputtypedef) 
4. See [:material-code-braces: CreateExperimentTemplateLogConfigurationInputTypeDef](./type_defs.md#createexperimenttemplatelogconfigurationinputtypedef) 
5. See [:material-code-braces: CreateExperimentTemplateResponseTypeDef](./type_defs.md#createexperimenttemplateresponsetypedef) 


```python
# create_experiment_template method usage example with argument unpacking

kwargs: CreateExperimentTemplateRequestRequestTypeDef = {  # (1)
    "clientToken": ...,
    "description": ...,
    "stopConditions": ...,
    "actions": ...,
    "roleArn": ...,
}

parent.create_experiment_template(**kwargs)
```

1. See [:material-code-braces: CreateExperimentTemplateRequestRequestTypeDef](./type_defs.md#createexperimenttemplaterequestrequesttypedef) 

### delete\_experiment\_template

Deletes the specified experiment template.

Type annotations and code completion for `#!python session.create_client("fis").delete_experiment_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.delete_experiment_template)

```python
# delete_experiment_template method definition

await def delete_experiment_template(
    self,
    *,
    id: str,
) -> DeleteExperimentTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteExperimentTemplateResponseTypeDef](./type_defs.md#deleteexperimenttemplateresponsetypedef) 


```python
# delete_experiment_template method usage example with argument unpacking

kwargs: DeleteExperimentTemplateRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_experiment_template(**kwargs)
```

1. See [:material-code-braces: DeleteExperimentTemplateRequestRequestTypeDef](./type_defs.md#deleteexperimenttemplaterequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("fis").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.generate_presigned_url)

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


### get\_action

Gets information about the specified FIS action.

Type annotations and code completion for `#!python session.create_client("fis").get_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.get_action)

```python
# get_action method definition

await def get_action(
    self,
    *,
    id: str,
) -> GetActionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetActionResponseTypeDef](./type_defs.md#getactionresponsetypedef) 


```python
# get_action method usage example with argument unpacking

kwargs: GetActionRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_action(**kwargs)
```

1. See [:material-code-braces: GetActionRequestRequestTypeDef](./type_defs.md#getactionrequestrequesttypedef) 

### get\_experiment

Gets information about the specified experiment.

Type annotations and code completion for `#!python session.create_client("fis").get_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.get_experiment)

```python
# get_experiment method definition

await def get_experiment(
    self,
    *,
    id: str,
) -> GetExperimentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetExperimentResponseTypeDef](./type_defs.md#getexperimentresponsetypedef) 


```python
# get_experiment method usage example with argument unpacking

kwargs: GetExperimentRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_experiment(**kwargs)
```

1. See [:material-code-braces: GetExperimentRequestRequestTypeDef](./type_defs.md#getexperimentrequestrequesttypedef) 

### get\_experiment\_template

Gets information about the specified experiment template.

Type annotations and code completion for `#!python session.create_client("fis").get_experiment_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.get_experiment_template)

```python
# get_experiment_template method definition

await def get_experiment_template(
    self,
    *,
    id: str,
) -> GetExperimentTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetExperimentTemplateResponseTypeDef](./type_defs.md#getexperimenttemplateresponsetypedef) 


```python
# get_experiment_template method usage example with argument unpacking

kwargs: GetExperimentTemplateRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_experiment_template(**kwargs)
```

1. See [:material-code-braces: GetExperimentTemplateRequestRequestTypeDef](./type_defs.md#getexperimenttemplaterequestrequesttypedef) 

### get\_target\_resource\_type

Gets information about the specified resource type.

Type annotations and code completion for `#!python session.create_client("fis").get_target_resource_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.get_target_resource_type)

```python
# get_target_resource_type method definition

await def get_target_resource_type(
    self,
    *,
    resourceType: str,
) -> GetTargetResourceTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTargetResourceTypeResponseTypeDef](./type_defs.md#gettargetresourcetyperesponsetypedef) 


```python
# get_target_resource_type method usage example with argument unpacking

kwargs: GetTargetResourceTypeRequestRequestTypeDef = {  # (1)
    "resourceType": ...,
}

parent.get_target_resource_type(**kwargs)
```

1. See [:material-code-braces: GetTargetResourceTypeRequestRequestTypeDef](./type_defs.md#gettargetresourcetyperequestrequesttypedef) 

### list\_actions

Lists the available FIS actions.

Type annotations and code completion for `#!python session.create_client("fis").list_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.list_actions)

```python
# list_actions method definition

await def list_actions(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListActionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListActionsResponseTypeDef](./type_defs.md#listactionsresponsetypedef) 


```python
# list_actions method usage example with argument unpacking

kwargs: ListActionsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_actions(**kwargs)
```

1. See [:material-code-braces: ListActionsRequestRequestTypeDef](./type_defs.md#listactionsrequestrequesttypedef) 

### list\_experiment\_templates

Lists your experiment templates.

Type annotations and code completion for `#!python session.create_client("fis").list_experiment_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.list_experiment_templates)

```python
# list_experiment_templates method definition

await def list_experiment_templates(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListExperimentTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListExperimentTemplatesResponseTypeDef](./type_defs.md#listexperimenttemplatesresponsetypedef) 


```python
# list_experiment_templates method usage example with argument unpacking

kwargs: ListExperimentTemplatesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_experiment_templates(**kwargs)
```

1. See [:material-code-braces: ListExperimentTemplatesRequestRequestTypeDef](./type_defs.md#listexperimenttemplatesrequestrequesttypedef) 

### list\_experiments

Lists your experiments.

Type annotations and code completion for `#!python session.create_client("fis").list_experiments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.list_experiments)

```python
# list_experiments method definition

await def list_experiments(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListExperimentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef) 


```python
# list_experiments method usage example with argument unpacking

kwargs: ListExperimentsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_experiments(**kwargs)
```

1. See [:material-code-braces: ListExperimentsRequestRequestTypeDef](./type_defs.md#listexperimentsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("fis").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.list_tags_for_resource)

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

### list\_target\_resource\_types

Lists the target resource types.

Type annotations and code completion for `#!python session.create_client("fis").list_target_resource_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.list_target_resource_types)

```python
# list_target_resource_types method definition

await def list_target_resource_types(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTargetResourceTypesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTargetResourceTypesResponseTypeDef](./type_defs.md#listtargetresourcetypesresponsetypedef) 


```python
# list_target_resource_types method usage example with argument unpacking

kwargs: ListTargetResourceTypesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_target_resource_types(**kwargs)
```

1. See [:material-code-braces: ListTargetResourceTypesRequestRequestTypeDef](./type_defs.md#listtargetresourcetypesrequestrequesttypedef) 

### start\_experiment

Starts running an experiment from the specified experiment template.

Type annotations and code completion for `#!python session.create_client("fis").start_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.start_experiment)

```python
# start_experiment method definition

await def start_experiment(
    self,
    *,
    clientToken: str,
    experimentTemplateId: str,
    tags: Mapping[str, str] = ...,
) -> StartExperimentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartExperimentResponseTypeDef](./type_defs.md#startexperimentresponsetypedef) 


```python
# start_experiment method usage example with argument unpacking

kwargs: StartExperimentRequestRequestTypeDef = {  # (1)
    "clientToken": ...,
    "experimentTemplateId": ...,
}

parent.start_experiment(**kwargs)
```

1. See [:material-code-braces: StartExperimentRequestRequestTypeDef](./type_defs.md#startexperimentrequestrequesttypedef) 

### stop\_experiment

Stops the specified experiment.

Type annotations and code completion for `#!python session.create_client("fis").stop_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.stop_experiment)

```python
# stop_experiment method definition

await def stop_experiment(
    self,
    *,
    id: str,
) -> StopExperimentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopExperimentResponseTypeDef](./type_defs.md#stopexperimentresponsetypedef) 


```python
# stop_experiment method usage example with argument unpacking

kwargs: StopExperimentRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.stop_experiment(**kwargs)
```

1. See [:material-code-braces: StopExperimentRequestRequestTypeDef](./type_defs.md#stopexperimentrequestrequesttypedef) 

### tag\_resource

Applies the specified tags to the specified resource.

Type annotations and code completion for `#!python session.create_client("fis").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.tag_resource)

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

Removes the specified tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("fis").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_experiment\_template

Updates the specified experiment template.

Type annotations and code completion for `#!python session.create_client("fis").update_experiment_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.update_experiment_template)

```python
# update_experiment_template method definition

await def update_experiment_template(
    self,
    *,
    id: str,
    description: str = ...,
    stopConditions: Sequence[UpdateExperimentTemplateStopConditionInputTypeDef] = ...,  # (1)
    targets: Mapping[str, UpdateExperimentTemplateTargetInputTypeDef] = ...,  # (2)
    actions: Mapping[str, UpdateExperimentTemplateActionInputItemTypeDef] = ...,  # (3)
    roleArn: str = ...,
    logConfiguration: UpdateExperimentTemplateLogConfigurationInputTypeDef = ...,  # (4)
) -> UpdateExperimentTemplateResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: UpdateExperimentTemplateStopConditionInputTypeDef](./type_defs.md#updateexperimenttemplatestopconditioninputtypedef) 
2. See [:material-code-braces: UpdateExperimentTemplateTargetInputTypeDef](./type_defs.md#updateexperimenttemplatetargetinputtypedef) 
3. See [:material-code-braces: UpdateExperimentTemplateActionInputItemTypeDef](./type_defs.md#updateexperimenttemplateactioninputitemtypedef) 
4. See [:material-code-braces: UpdateExperimentTemplateLogConfigurationInputTypeDef](./type_defs.md#updateexperimenttemplatelogconfigurationinputtypedef) 
5. See [:material-code-braces: UpdateExperimentTemplateResponseTypeDef](./type_defs.md#updateexperimenttemplateresponsetypedef) 


```python
# update_experiment_template method usage example with argument unpacking

kwargs: UpdateExperimentTemplateRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.update_experiment_template(**kwargs)
```

1. See [:material-code-braces: UpdateExperimentTemplateRequestRequestTypeDef](./type_defs.md#updateexperimenttemplaterequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("fis").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> FISClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("fis").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client.__aexit__)

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





