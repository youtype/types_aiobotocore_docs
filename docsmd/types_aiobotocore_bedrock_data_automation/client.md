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
) -> CreateBlueprintResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-brackets: BlueprintStageType](./literals.md#blueprintstagetype) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
4. See [:material-code-braces: CreateBlueprintResponseTypeDef](./type_defs.md#createblueprintresponsetypedef) 


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
    customOutputConfiguration: CustomOutputConfigurationUnionTypeDef = ...,  # (3)
    overrideConfiguration: OverrideConfigurationTypeDef = ...,  # (4)
    clientToken: str = ...,
    encryptionConfiguration: EncryptionConfigurationTypeDef = ...,  # (5)
) -> CreateDataAutomationProjectResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: StandardOutputConfigurationTypeDef](./type_defs.md#standardoutputconfigurationtypedef) [:material-code-braces: StandardOutputConfigurationOutputTypeDef](./type_defs.md#standardoutputconfigurationoutputtypedef) 
2. See [:material-code-brackets: DataAutomationProjectStageType](./literals.md#dataautomationprojectstagetype) 
3. See [:material-code-braces: CustomOutputConfigurationTypeDef](./type_defs.md#customoutputconfigurationtypedef) [:material-code-braces: CustomOutputConfigurationOutputTypeDef](./type_defs.md#customoutputconfigurationoutputtypedef) 
4. See [:material-code-braces: OverrideConfigurationTypeDef](./type_defs.md#overrideconfigurationtypedef) 
5. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
6. See [:material-code-braces: CreateDataAutomationProjectResponseTypeDef](./type_defs.md#createdataautomationprojectresponsetypedef) 


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
) -> Dict[str, Any]:
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
) -> UpdateBlueprintResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: BlueprintStageType](./literals.md#blueprintstagetype) 
2. See [:material-code-braces: UpdateBlueprintResponseTypeDef](./type_defs.md#updateblueprintresponsetypedef) 


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
    overrideConfiguration: OverrideConfigurationTypeDef = ...,  # (4)
) -> UpdateDataAutomationProjectResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: StandardOutputConfigurationTypeDef](./type_defs.md#standardoutputconfigurationtypedef) [:material-code-braces: StandardOutputConfigurationOutputTypeDef](./type_defs.md#standardoutputconfigurationoutputtypedef) 
2. See [:material-code-brackets: DataAutomationProjectStageType](./literals.md#dataautomationprojectstagetype) 
3. See [:material-code-braces: CustomOutputConfigurationTypeDef](./type_defs.md#customoutputconfigurationtypedef) [:material-code-braces: CustomOutputConfigurationOutputTypeDef](./type_defs.md#customoutputconfigurationoutputtypedef) 
4. See [:material-code-braces: OverrideConfigurationTypeDef](./type_defs.md#overrideconfigurationtypedef) 
5. See [:material-code-braces: UpdateDataAutomationProjectResponseTypeDef](./type_defs.md#updatedataautomationprojectresponsetypedef) 


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
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("bedrock-data-automation").get_paginator` method with overloads.

- `client.get_paginator("list_blueprints")` -> [ListBlueprintsPaginator](./paginators.md#listblueprintspaginator)
- `client.get_paginator("list_data_automation_projects")` -> [ListDataAutomationProjectsPaginator](./paginators.md#listdataautomationprojectspaginator)



