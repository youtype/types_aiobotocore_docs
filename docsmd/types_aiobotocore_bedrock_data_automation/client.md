# DataAutomationforBedrockClient

> [Index](../README.md) > [DataAutomationforBedrock](./README.md) > DataAutomationforBedrockClient

!!! note ""

    Auto-generated documentation for [DataAutomationforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation.html#dataautomationforbedrock)
    type annotations stubs module [types-aiobotocore-bedrock-data-automation](https://pypi.org/project/types-aiobotocore-bedrock-data-automation/).

## DataAutomationforBedrockClient

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation.html#DataAutomationforBedrock.Client)

```python
# DataAutomationforBedrockClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_bedrock_data_automation.client import DataAutomationforBedrockClient

session = get_session()
async with session.create_client("bedrock-data-automation") as client:
    client: DataAutomationforBedrockClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("bedrock-data-automation").exceptions` structure.

```python
# DataAutomationforBedrockClient.exceptions usage example

async with session.create_client("bedrock-data-automation") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# DataAutomationforBedrockClient usage type checking example

from types_aiobotocore_bedrock_data_automation.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/generate_presigned_url.html)

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


### copy\_blueprint\_stage

Copies a Blueprint from one stage to another.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").copy_blueprint_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/copy_blueprint_stage.html)

```python
# copy_blueprint_stage method definition

await def copy_blueprint_stage(
    self,
    *,
    blueprintArn: str,
    sourceStage: BlueprintStageType,  # (1)
    targetStage: BlueprintStageType,  # (1)
    clientToken: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: BlueprintStageType](./literals.md#blueprintstagetype)
2. See [:material-code-brackets: BlueprintStageType](./literals.md#blueprintstagetype)


```python
# copy_blueprint_stage method usage example with argument unpacking

kwargs: CopyBlueprintStageRequestTypeDef = {  # (1)
    "blueprintArn": ...,
    "sourceStage": ...,
    "targetStage": ...,
}

parent.copy_blueprint_stage(**kwargs)
```

1. See [:material-code-braces: CopyBlueprintStageRequestTypeDef](./type_defs.md#copyblueprintstagerequesttypedef)

### create\_blueprint

Creates an Amazon Bedrock Data Automation Blueprint.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").create_blueprint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/create_blueprint.html)

```python
# create_blueprint method definition

await def create_blueprint(
    self,
    *,
    blueprintName: str,
    type: TypeType,  # (1)
    schema: str,
    blueprintStage: BlueprintStageType = ...,  # (2)
    clientToken: str = ...,
    encryptionConfiguration: EncryptionConfigurationTypeDef = ...,  # (3)
    tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateBlueprintResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype)
2. See [:material-code-brackets: BlueprintStageType](./literals.md#blueprintstagetype)
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
4. See `Sequence[TagTypeDef]`
5. See [:material-code-braces: CreateBlueprintResponseTypeDef](./type_defs.md#createblueprintresponsetypedef)


```python
# create_blueprint method usage example with argument unpacking

kwargs: CreateBlueprintRequestTypeDef = {  # (1)
    "blueprintName": ...,
    "type": ...,
    "schema": ...,
}

parent.create_blueprint(**kwargs)
```

1. See [:material-code-braces: CreateBlueprintRequestTypeDef](./type_defs.md#createblueprintrequesttypedef)

### create\_blueprint\_version

Creates a new version of an existing Amazon Bedrock Data Automation Blueprint.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").create_blueprint_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/create_blueprint_version.html)

```python
# create_blueprint_version method definition

await def create_blueprint_version(
    self,
    *,
    blueprintArn: str,
    clientToken: str = ...,
) -> CreateBlueprintVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateBlueprintVersionResponseTypeDef](./type_defs.md#createblueprintversionresponsetypedef)


```python
# create_blueprint_version method usage example with argument unpacking

kwargs: CreateBlueprintVersionRequestTypeDef = {  # (1)
    "blueprintArn": ...,
}

parent.create_blueprint_version(**kwargs)
```

1. See [:material-code-braces: CreateBlueprintVersionRequestTypeDef](./type_defs.md#createblueprintversionrequesttypedef)

### create\_data\_automation\_project

Creates an Amazon Bedrock Data Automation Project.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").create_data_automation_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/create_data_automation_project.html)

```python
# create_data_automation_project method definition

await def create_data_automation_project(
    self,
    *,
    projectName: str,
    standardOutputConfiguration: StandardOutputConfigurationUnionTypeDef,  # (1)
    projectDescription: str = ...,
    projectStage: DataAutomationProjectStageType = ...,  # (2)
    projectType: DataAutomationProjectTypeType = ...,  # (3)
    customOutputConfiguration: CustomOutputConfigurationUnionTypeDef = ...,  # (4)
    overrideConfiguration: OverrideConfigurationUnionTypeDef = ...,  # (5)
    clientToken: str = ...,
    encryptionConfiguration: EncryptionConfigurationTypeDef = ...,  # (6)
    tags: Sequence[TagTypeDef] = ...,  # (7)
) -> CreateDataAutomationProjectResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: StandardOutputConfigurationUnionTypeDef](#standardoutputconfigurationuniontypedef)
2. See [:material-code-brackets: DataAutomationProjectStageType](./literals.md#dataautomationprojectstagetype)
3. See [:material-code-brackets: DataAutomationProjectTypeType](./literals.md#dataautomationprojecttypetype)
4. See [:material-code-braces: CustomOutputConfigurationUnionTypeDef](#customoutputconfigurationuniontypedef)
5. See [:material-code-braces: OverrideConfigurationUnionTypeDef](#overrideconfigurationuniontypedef)
6. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
7. See `Sequence[TagTypeDef]`
8. See [:material-code-braces: CreateDataAutomationProjectResponseTypeDef](./type_defs.md#createdataautomationprojectresponsetypedef)


```python
# create_data_automation_project method usage example with argument unpacking

kwargs: CreateDataAutomationProjectRequestTypeDef = {  # (1)
    "projectName": ...,
    "standardOutputConfiguration": ...,
}

parent.create_data_automation_project(**kwargs)
```

1. See [:material-code-braces: CreateDataAutomationProjectRequestTypeDef](./type_defs.md#createdataautomationprojectrequesttypedef)

### delete\_blueprint

Deletes an existing Amazon Bedrock Data Automation Blueprint.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").delete_blueprint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/delete_blueprint.html)

```python
# delete_blueprint method definition

await def delete_blueprint(
    self,
    *,
    blueprintArn: str,
    blueprintVersion: str = ...,
) -> dict[str, Any]:
    ...
```

```python
# delete_blueprint method usage example with argument unpacking

kwargs: DeleteBlueprintRequestTypeDef = {  # (1)
    "blueprintArn": ...,
}

parent.delete_blueprint(**kwargs)
```

1. See [:material-code-braces: DeleteBlueprintRequestTypeDef](./type_defs.md#deleteblueprintrequesttypedef)

### delete\_data\_automation\_project

Deletes an existing Amazon Bedrock Data Automation Project.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").delete_data_automation_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/delete_data_automation_project.html)

```python
# delete_data_automation_project method definition

await def delete_data_automation_project(
    self,
    *,
    projectArn: str,
) -> DeleteDataAutomationProjectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataAutomationProjectResponseTypeDef](./type_defs.md#deletedataautomationprojectresponsetypedef)


```python
# delete_data_automation_project method usage example with argument unpacking

kwargs: DeleteDataAutomationProjectRequestTypeDef = {  # (1)
    "projectArn": ...,
}

parent.delete_data_automation_project(**kwargs)
```

1. See [:material-code-braces: DeleteDataAutomationProjectRequestTypeDef](./type_defs.md#deletedataautomationprojectrequesttypedef)

### get\_blueprint

Gets an existing Amazon Bedrock Data Automation Blueprint.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").get_blueprint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/get_blueprint.html)

```python
# get_blueprint method definition

await def get_blueprint(
    self,
    *,
    blueprintArn: str,
    blueprintVersion: str = ...,
    blueprintStage: BlueprintStageType = ...,  # (1)
) -> GetBlueprintResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: BlueprintStageType](./literals.md#blueprintstagetype)
2. See [:material-code-braces: GetBlueprintResponseTypeDef](./type_defs.md#getblueprintresponsetypedef)


```python
# get_blueprint method usage example with argument unpacking

kwargs: GetBlueprintRequestTypeDef = {  # (1)
    "blueprintArn": ...,
}

parent.get_blueprint(**kwargs)
```

1. See [:material-code-braces: GetBlueprintRequestTypeDef](./type_defs.md#getblueprintrequesttypedef)

### get\_blueprint\_optimization\_status

API used to get blueprint optimization status.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").get_blueprint_optimization_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/get_blueprint_optimization_status.html)

```python
# get_blueprint_optimization_status method definition

await def get_blueprint_optimization_status(
    self,
    *,
    invocationArn: str,
) -> GetBlueprintOptimizationStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBlueprintOptimizationStatusResponseTypeDef](./type_defs.md#getblueprintoptimizationstatusresponsetypedef)


```python
# get_blueprint_optimization_status method usage example with argument unpacking

kwargs: GetBlueprintOptimizationStatusRequestTypeDef = {  # (1)
    "invocationArn": ...,
}

parent.get_blueprint_optimization_status(**kwargs)
```

1. See [:material-code-braces: GetBlueprintOptimizationStatusRequestTypeDef](./type_defs.md#getblueprintoptimizationstatusrequesttypedef)

### get\_data\_automation\_project

Gets an existing Amazon Bedrock Data Automation Project.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").get_data_automation_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/get_data_automation_project.html)

```python
# get_data_automation_project method definition

await def get_data_automation_project(
    self,
    *,
    projectArn: str,
    projectStage: DataAutomationProjectStageType = ...,  # (1)
) -> GetDataAutomationProjectResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataAutomationProjectStageType](./literals.md#dataautomationprojectstagetype)
2. See [:material-code-braces: GetDataAutomationProjectResponseTypeDef](./type_defs.md#getdataautomationprojectresponsetypedef)


```python
# get_data_automation_project method usage example with argument unpacking

kwargs: GetDataAutomationProjectRequestTypeDef = {  # (1)
    "projectArn": ...,
}

parent.get_data_automation_project(**kwargs)
```

1. See [:material-code-braces: GetDataAutomationProjectRequestTypeDef](./type_defs.md#getdataautomationprojectrequesttypedef)

### invoke\_blueprint\_optimization\_async

Invoke an async job to perform Blueprint Optimization.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").invoke_blueprint_optimization_async` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/invoke_blueprint_optimization_async.html)

```python
# invoke_blueprint_optimization_async method definition

await def invoke_blueprint_optimization_async(
    self,
    *,
    blueprint: BlueprintOptimizationObjectTypeDef,  # (1)
    samples: Sequence[BlueprintOptimizationSampleTypeDef],  # (2)
    outputConfiguration: BlueprintOptimizationOutputConfigurationTypeDef,  # (3)
    dataAutomationProfileArn: str,
    encryptionConfiguration: EncryptionConfigurationTypeDef = ...,  # (4)
    tags: Sequence[TagTypeDef] = ...,  # (5)
) -> InvokeBlueprintOptimizationAsyncResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: BlueprintOptimizationObjectTypeDef](./type_defs.md#blueprintoptimizationobjecttypedef)
2. See `Sequence[BlueprintOptimizationSampleTypeDef]`
3. See [:material-code-braces: BlueprintOptimizationOutputConfigurationTypeDef](./type_defs.md#blueprintoptimizationoutputconfigurationtypedef)
4. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
5. See `Sequence[TagTypeDef]`
6. See [:material-code-braces: InvokeBlueprintOptimizationAsyncResponseTypeDef](./type_defs.md#invokeblueprintoptimizationasyncresponsetypedef)


```python
# invoke_blueprint_optimization_async method usage example with argument unpacking

kwargs: InvokeBlueprintOptimizationAsyncRequestTypeDef = {  # (1)
    "blueprint": ...,
    "samples": ...,
    "outputConfiguration": ...,
    "dataAutomationProfileArn": ...,
}

parent.invoke_blueprint_optimization_async(**kwargs)
```

1. See [:material-code-braces: InvokeBlueprintOptimizationAsyncRequestTypeDef](./type_defs.md#invokeblueprintoptimizationasyncrequesttypedef)

### list\_blueprints

Lists all existing Amazon Bedrock Data Automation Blueprints.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").list_blueprints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/list_blueprints.html)

```python
# list_blueprints method definition

await def list_blueprints(
    self,
    *,
    blueprintArn: str = ...,
    resourceOwner: ResourceOwnerType = ...,  # (1)
    blueprintStageFilter: BlueprintStageFilterType = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
    projectFilter: DataAutomationProjectFilterTypeDef = ...,  # (3)
) -> ListBlueprintsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype)
2. See [:material-code-brackets: BlueprintStageFilterType](./literals.md#blueprintstagefiltertype)
3. See [:material-code-braces: DataAutomationProjectFilterTypeDef](./type_defs.md#dataautomationprojectfiltertypedef)
4. See [:material-code-braces: ListBlueprintsResponseTypeDef](./type_defs.md#listblueprintsresponsetypedef)


```python
# list_blueprints method usage example with argument unpacking

kwargs: ListBlueprintsRequestTypeDef = {  # (1)
    "blueprintArn": ...,
}

parent.list_blueprints(**kwargs)
```

1. See [:material-code-braces: ListBlueprintsRequestTypeDef](./type_defs.md#listblueprintsrequesttypedef)

### list\_data\_automation\_projects

Lists all existing Amazon Bedrock Data Automation Projects.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").list_data_automation_projects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/list_data_automation_projects.html)

```python
# list_data_automation_projects method definition

await def list_data_automation_projects(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    projectStageFilter: DataAutomationProjectStageFilterType = ...,  # (1)
    blueprintFilter: BlueprintFilterTypeDef = ...,  # (2)
    resourceOwner: ResourceOwnerType = ...,  # (3)
) -> ListDataAutomationProjectsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: DataAutomationProjectStageFilterType](./literals.md#dataautomationprojectstagefiltertype)
2. See [:material-code-braces: BlueprintFilterTypeDef](./type_defs.md#blueprintfiltertypedef)
3. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype)
4. See [:material-code-braces: ListDataAutomationProjectsResponseTypeDef](./type_defs.md#listdataautomationprojectsresponsetypedef)


```python
# list_data_automation_projects method usage example with argument unpacking

kwargs: ListDataAutomationProjectsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_data_automation_projects(**kwargs)
```

1. See [:material-code-braces: ListDataAutomationProjectsRequestTypeDef](./type_defs.md#listdataautomationprojectsrequesttypedef)

### list\_tags\_for\_resource

List tags for an Amazon Bedrock Data Automation resource.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)

### tag\_resource

Tag an Amazon Bedrock Data Automation resource.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceARN: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See `Sequence[TagTypeDef]`


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### untag\_resource

Untag an Amazon Bedrock Data Automation resource.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceARN: str,
    tagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```

```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### update\_blueprint

Updates an existing Amazon Bedrock Data Automation Blueprint.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").update_blueprint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/update_blueprint.html)

```python
# update_blueprint method definition

await def update_blueprint(
    self,
    *,
    blueprintArn: str,
    schema: str,
    blueprintStage: BlueprintStageType = ...,  # (1)
    encryptionConfiguration: EncryptionConfigurationTypeDef = ...,  # (2)
) -> UpdateBlueprintResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: BlueprintStageType](./literals.md#blueprintstagetype)
2. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
3. See [:material-code-braces: UpdateBlueprintResponseTypeDef](./type_defs.md#updateblueprintresponsetypedef)


```python
# update_blueprint method usage example with argument unpacking

kwargs: UpdateBlueprintRequestTypeDef = {  # (1)
    "blueprintArn": ...,
    "schema": ...,
}

parent.update_blueprint(**kwargs)
```

1. See [:material-code-braces: UpdateBlueprintRequestTypeDef](./type_defs.md#updateblueprintrequesttypedef)

### update\_data\_automation\_project

Updates an existing Amazon Bedrock Data Automation Project.

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").update_data_automation_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation/client/update_data_automation_project.html)

```python
# update_data_automation_project method definition

await def update_data_automation_project(
    self,
    *,
    projectArn: str,
    standardOutputConfiguration: StandardOutputConfigurationUnionTypeDef,  # (1)
    projectStage: DataAutomationProjectStageType = ...,  # (2)
    projectDescription: str = ...,
    customOutputConfiguration: CustomOutputConfigurationUnionTypeDef = ...,  # (3)
    overrideConfiguration: OverrideConfigurationUnionTypeDef = ...,  # (4)
    encryptionConfiguration: EncryptionConfigurationTypeDef = ...,  # (5)
) -> UpdateDataAutomationProjectResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: StandardOutputConfigurationUnionTypeDef](#standardoutputconfigurationuniontypedef)
2. See [:material-code-brackets: DataAutomationProjectStageType](./literals.md#dataautomationprojectstagetype)
3. See [:material-code-braces: CustomOutputConfigurationUnionTypeDef](#customoutputconfigurationuniontypedef)
4. See [:material-code-braces: OverrideConfigurationUnionTypeDef](#overrideconfigurationuniontypedef)
5. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
6. See [:material-code-braces: UpdateDataAutomationProjectResponseTypeDef](./type_defs.md#updatedataautomationprojectresponsetypedef)


```python
# update_data_automation_project method usage example with argument unpacking

kwargs: UpdateDataAutomationProjectRequestTypeDef = {  # (1)
    "projectArn": ...,
    "standardOutputConfiguration": ...,
}

parent.update_data_automation_project(**kwargs)
```

1. See [:material-code-braces: UpdateDataAutomationProjectRequestTypeDef](./type_defs.md#updatedataautomationprojectrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation.html#DataAutomationforBedrock.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation.html#DataAutomationforBedrock.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").get_paginator` method with overloads.

- `client.get_paginator("list_blueprints")` -> [ListBlueprintsPaginator](./paginators.md#listblueprintspaginator)
- `client.get_paginator("list_data_automation_projects")` -> [ListDataAutomationProjectsPaginator](./paginators.md#listdataautomationprojectspaginator)



