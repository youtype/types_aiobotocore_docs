# SystemsManagerQuickSetupClient

> [Index](../README.md) > [SystemsManagerQuickSetup](./README.md) > SystemsManagerQuickSetupClient

!!! note ""

    Auto-generated documentation for [SystemsManagerQuickSetup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup)
    type annotations stubs module [types-aiobotocore-ssm-quicksetup](https://pypi.org/project/types-aiobotocore-ssm-quicksetup/).

## SystemsManagerQuickSetupClient

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client)

```python
# SystemsManagerQuickSetupClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_ssm_quicksetup.client import SystemsManagerQuickSetupClient

session = get_session()
async with session.create_client("ssm-quicksetup") as client:
    client: SystemsManagerQuickSetupClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("ssm-quicksetup").exceptions` structure.

```python
# SystemsManagerQuickSetupClient.exceptions usage example

async with session.create_client("ssm-quicksetup") as client:
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
# SystemsManagerQuickSetupClient usage type checking example

from types_aiobotocore_ssm_quicksetup.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_configuration\_manager

Creates a Quick Setup configuration manager resource.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").create_configuration_manager` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.create_configuration_manager)

```python
# create_configuration_manager method definition

await def create_configuration_manager(
    self,
    *,
    ConfigurationDefinitions: Sequence[ConfigurationDefinitionInputTypeDef],  # (1)
    Description: str = ...,
    Name: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateConfigurationManagerOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConfigurationDefinitionInputTypeDef](./type_defs.md#configurationdefinitioninputtypedef) 
2. See [:material-code-braces: CreateConfigurationManagerOutputTypeDef](./type_defs.md#createconfigurationmanageroutputtypedef) 


```python
# create_configuration_manager method usage example with argument unpacking

kwargs: CreateConfigurationManagerInputRequestTypeDef = {  # (1)
    "ConfigurationDefinitions": ...,
}

parent.create_configuration_manager(**kwargs)
```

1. See [:material-code-braces: CreateConfigurationManagerInputRequestTypeDef](./type_defs.md#createconfigurationmanagerinputrequesttypedef) 

### delete\_configuration\_manager

Deletes a configuration manager.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").delete_configuration_manager` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.delete_configuration_manager)

```python
# delete_configuration_manager method definition

await def delete_configuration_manager(
    self,
    *,
    ManagerArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_configuration_manager method usage example with argument unpacking

kwargs: DeleteConfigurationManagerInputRequestTypeDef = {  # (1)
    "ManagerArn": ...,
}

parent.delete_configuration_manager(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationManagerInputRequestTypeDef](./type_defs.md#deleteconfigurationmanagerinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.generate_presigned_url)

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


### get\_configuration\_manager

Returns a configuration manager.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").get_configuration_manager` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.get_configuration_manager)

```python
# get_configuration_manager method definition

await def get_configuration_manager(
    self,
    *,
    ManagerArn: str,
) -> GetConfigurationManagerOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfigurationManagerOutputTypeDef](./type_defs.md#getconfigurationmanageroutputtypedef) 


```python
# get_configuration_manager method usage example with argument unpacking

kwargs: GetConfigurationManagerInputRequestTypeDef = {  # (1)
    "ManagerArn": ...,
}

parent.get_configuration_manager(**kwargs)
```

1. See [:material-code-braces: GetConfigurationManagerInputRequestTypeDef](./type_defs.md#getconfigurationmanagerinputrequesttypedef) 

### get\_service\_settings

Returns settings configured for Quick Setup in the requesting Amazon Web
Services account and Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").get_service_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.get_service_settings)

```python
# get_service_settings method definition

await def get_service_settings(
    self,
) -> GetServiceSettingsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceSettingsOutputTypeDef](./type_defs.md#getservicesettingsoutputtypedef) 

### list\_configuration\_managers

Returns Quick Setup configuration managers.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").list_configuration_managers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.list_configuration_managers)

```python
# list_configuration_managers method definition

await def list_configuration_managers(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxItems: int = ...,
    StartingToken: str = ...,
) -> ListConfigurationManagersOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListConfigurationManagersOutputTypeDef](./type_defs.md#listconfigurationmanagersoutputtypedef) 


```python
# list_configuration_managers method usage example with argument unpacking

kwargs: ListConfigurationManagersInputRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_configuration_managers(**kwargs)
```

1. See [:material-code-braces: ListConfigurationManagersInputRequestTypeDef](./type_defs.md#listconfigurationmanagersinputrequesttypedef) 

### list\_quick\_setup\_types

Returns the available Quick Setup types.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").list_quick_setup_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.list_quick_setup_types)

```python
# list_quick_setup_types method definition

await def list_quick_setup_types(
    self,
) -> ListQuickSetupTypesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListQuickSetupTypesOutputTypeDef](./type_defs.md#listquicksetuptypesoutputtypedef) 

### list\_tags\_for\_resource

Returns tags assigned to the resource.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### tag\_resource

Assigns key-value pairs of metadata to Amazon Web Services resources.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Removes tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_configuration\_definition

Updates a Quick Setup configuration definition.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").update_configuration_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.update_configuration_definition)

```python
# update_configuration_definition method definition

await def update_configuration_definition(
    self,
    *,
    Id: str,
    ManagerArn: str,
    LocalDeploymentAdministrationRoleArn: str = ...,
    LocalDeploymentExecutionRoleName: str = ...,
    Parameters: Mapping[str, str] = ...,
    TypeVersion: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_configuration_definition method usage example with argument unpacking

kwargs: UpdateConfigurationDefinitionInputRequestTypeDef = {  # (1)
    "Id": ...,
    "ManagerArn": ...,
}

parent.update_configuration_definition(**kwargs)
```

1. See [:material-code-braces: UpdateConfigurationDefinitionInputRequestTypeDef](./type_defs.md#updateconfigurationdefinitioninputrequesttypedef) 

### update\_configuration\_manager

Updates a Quick Setup configuration manager.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").update_configuration_manager` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.update_configuration_manager)

```python
# update_configuration_manager method definition

await def update_configuration_manager(
    self,
    *,
    ManagerArn: str,
    Description: str = ...,
    Name: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_configuration_manager method usage example with argument unpacking

kwargs: UpdateConfigurationManagerInputRequestTypeDef = {  # (1)
    "ManagerArn": ...,
}

parent.update_configuration_manager(**kwargs)
```

1. See [:material-code-braces: UpdateConfigurationManagerInputRequestTypeDef](./type_defs.md#updateconfigurationmanagerinputrequesttypedef) 

### update\_service\_settings

Updates settings configured for Quick Setup.

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").update_service_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.update_service_settings)

```python
# update_service_settings method definition

await def update_service_settings(
    self,
    *,
    ExplorerEnablingRoleArn: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_service_settings method usage example with argument unpacking

kwargs: UpdateServiceSettingsInputRequestTypeDef = {  # (1)
    "ExplorerEnablingRoleArn": ...,
}

parent.update_service_settings(**kwargs)
```

1. See [:material-code-braces: UpdateServiceSettingsInputRequestTypeDef](./type_defs.md#updateservicesettingsinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "SystemsManagerQuickSetupClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").get_paginator` method with overloads.

- `client.get_paginator("list_configuration_managers")` -> [ListConfigurationManagersPaginator](./paginators.md#listconfigurationmanagerspaginator)



