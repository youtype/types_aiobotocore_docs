# AppConfigClient

> [Index](../README.md) > [AppConfig](./README.md) > AppConfigClient

!!! note ""

    Auto-generated documentation for [AppConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#appconfig)
    type annotations stubs module [types-aiobotocore-appconfig](https://pypi.org/project/types-aiobotocore-appconfig/).

## AppConfigClient

Type annotations and code completion for `#!python session.create_client("appconfig")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client)

```python
# AppConfigClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_appconfig.client import AppConfigClient

session = get_session()
async with session.create_client("appconfig") as client:
    client: AppConfigClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("appconfig").exceptions` structure.

```python
# AppConfigClient.exceptions usage example

async with session.create_client("appconfig") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.PayloadTooLargeException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
    ) as e:
        print(e)
```

```python
# AppConfigClient usage type checking example

from types_aiobotocore_appconfig.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("appconfig").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("appconfig").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/generate_presigned_url.html)

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


### create\_application

Creates an application.

Type annotations and code completion for `#!python session.create_client("appconfig").create_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/create_application.html)

```python
# create_application method definition

await def create_application(
    self,
    *,
    Name: str,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> ApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef) 


```python
# create_application method usage example with argument unpacking

kwargs: CreateApplicationRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_application(**kwargs)
```

1. See [:material-code-braces: CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef) 

### create\_configuration\_profile

Creates a configuration profile, which is information that enables AppConfig to
access the configuration source.

Type annotations and code completion for `#!python session.create_client("appconfig").create_configuration_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/create_configuration_profile.html)

```python
# create_configuration_profile method definition

await def create_configuration_profile(
    self,
    *,
    ApplicationId: str,
    Name: str,
    LocationUri: str,
    Description: str = ...,
    RetrievalRoleArn: str = ...,
    Validators: Sequence[ValidatorTypeDef] = ...,  # (1)
    Tags: Mapping[str, str] = ...,
    Type: str = ...,
    KmsKeyIdentifier: str = ...,
) -> ConfigurationProfileTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ValidatorTypeDef](./type_defs.md#validatortypedef) 
2. See [:material-code-braces: ConfigurationProfileTypeDef](./type_defs.md#configurationprofiletypedef) 


```python
# create_configuration_profile method usage example with argument unpacking

kwargs: CreateConfigurationProfileRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "Name": ...,
    "LocationUri": ...,
}

parent.create_configuration_profile(**kwargs)
```

1. See [:material-code-braces: CreateConfigurationProfileRequestTypeDef](./type_defs.md#createconfigurationprofilerequesttypedef) 

### create\_deployment\_strategy

Creates a deployment strategy that defines important criteria for rolling out
your configuration to the designated targets.

Type annotations and code completion for `#!python session.create_client("appconfig").create_deployment_strategy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/create_deployment_strategy.html)

```python
# create_deployment_strategy method definition

await def create_deployment_strategy(
    self,
    *,
    Name: str,
    DeploymentDurationInMinutes: int,
    GrowthFactor: float,
    Description: str = ...,
    FinalBakeTimeInMinutes: int = ...,
    GrowthType: GrowthTypeType = ...,  # (1)
    ReplicateTo: ReplicateToType = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> DeploymentStrategyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: GrowthTypeType](./literals.md#growthtypetype) 
2. See [:material-code-brackets: ReplicateToType](./literals.md#replicatetotype) 
3. See [:material-code-braces: DeploymentStrategyResponseTypeDef](./type_defs.md#deploymentstrategyresponsetypedef) 


```python
# create_deployment_strategy method usage example with argument unpacking

kwargs: CreateDeploymentStrategyRequestTypeDef = {  # (1)
    "Name": ...,
    "DeploymentDurationInMinutes": ...,
    "GrowthFactor": ...,
}

parent.create_deployment_strategy(**kwargs)
```

1. See [:material-code-braces: CreateDeploymentStrategyRequestTypeDef](./type_defs.md#createdeploymentstrategyrequesttypedef) 

### create\_environment

Creates an environment.

Type annotations and code completion for `#!python session.create_client("appconfig").create_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/create_environment.html)

```python
# create_environment method definition

await def create_environment(
    self,
    *,
    ApplicationId: str,
    Name: str,
    Description: str = ...,
    Monitors: Sequence[MonitorTypeDef] = ...,  # (1)
    Tags: Mapping[str, str] = ...,
) -> EnvironmentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MonitorTypeDef](./type_defs.md#monitortypedef) 
2. See [:material-code-braces: EnvironmentResponseTypeDef](./type_defs.md#environmentresponsetypedef) 


```python
# create_environment method usage example with argument unpacking

kwargs: CreateEnvironmentRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "Name": ...,
}

parent.create_environment(**kwargs)
```

1. See [:material-code-braces: CreateEnvironmentRequestTypeDef](./type_defs.md#createenvironmentrequesttypedef) 

### create\_extension

Creates an AppConfig extension.

Type annotations and code completion for `#!python session.create_client("appconfig").create_extension` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/create_extension.html)

```python
# create_extension method definition

await def create_extension(
    self,
    *,
    Name: str,
    Actions: Mapping[ActionPointType, Sequence[ActionTypeDef]],  # (1)
    Description: str = ...,
    Parameters: Mapping[str, ParameterTypeDef] = ...,  # (2)
    Tags: Mapping[str, str] = ...,
    LatestVersionNumber: int = ...,
) -> ExtensionTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ActionPointType](./literals.md#actionpointtype) [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
3. See [:material-code-braces: ExtensionTypeDef](./type_defs.md#extensiontypedef) 


```python
# create_extension method usage example with argument unpacking

kwargs: CreateExtensionRequestTypeDef = {  # (1)
    "Name": ...,
    "Actions": ...,
}

parent.create_extension(**kwargs)
```

1. See [:material-code-braces: CreateExtensionRequestTypeDef](./type_defs.md#createextensionrequesttypedef) 

### create\_extension\_association

When you create an extension or configure an Amazon Web Services authored
extension, you associate the extension with an AppConfig application,
environment, or configuration profile.

Type annotations and code completion for `#!python session.create_client("appconfig").create_extension_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/create_extension_association.html)

```python
# create_extension_association method definition

await def create_extension_association(
    self,
    *,
    ExtensionIdentifier: str,
    ResourceIdentifier: str,
    ExtensionVersionNumber: int = ...,
    Parameters: Mapping[str, str] = ...,
    Tags: Mapping[str, str] = ...,
) -> ExtensionAssociationTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExtensionAssociationTypeDef](./type_defs.md#extensionassociationtypedef) 


```python
# create_extension_association method usage example with argument unpacking

kwargs: CreateExtensionAssociationRequestTypeDef = {  # (1)
    "ExtensionIdentifier": ...,
    "ResourceIdentifier": ...,
}

parent.create_extension_association(**kwargs)
```

1. See [:material-code-braces: CreateExtensionAssociationRequestTypeDef](./type_defs.md#createextensionassociationrequesttypedef) 

### create\_hosted\_configuration\_version

Creates a new configuration in the AppConfig hosted configuration store.

Type annotations and code completion for `#!python session.create_client("appconfig").create_hosted_configuration_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/create_hosted_configuration_version.html)

```python
# create_hosted_configuration_version method definition

await def create_hosted_configuration_version(
    self,
    *,
    ApplicationId: str,
    ConfigurationProfileId: str,
    Content: BlobTypeDef,
    ContentType: str,
    Description: str = ...,
    LatestVersionNumber: int = ...,
    VersionLabel: str = ...,
) -> HostedConfigurationVersionTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: HostedConfigurationVersionTypeDef](./type_defs.md#hostedconfigurationversiontypedef) 


```python
# create_hosted_configuration_version method usage example with argument unpacking

kwargs: CreateHostedConfigurationVersionRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "ConfigurationProfileId": ...,
    "Content": ...,
    "ContentType": ...,
}

parent.create_hosted_configuration_version(**kwargs)
```

1. See [:material-code-braces: CreateHostedConfigurationVersionRequestTypeDef](./type_defs.md#createhostedconfigurationversionrequesttypedef) 

### delete\_application

Deletes an application.

Type annotations and code completion for `#!python session.create_client("appconfig").delete_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/delete_application.html)

```python
# delete_application method definition

await def delete_application(
    self,
    *,
    ApplicationId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_application method usage example with argument unpacking

kwargs: DeleteApplicationRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.delete_application(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationRequestTypeDef](./type_defs.md#deleteapplicationrequesttypedef) 

### delete\_configuration\_profile

Deletes a configuration profile.

Type annotations and code completion for `#!python session.create_client("appconfig").delete_configuration_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/delete_configuration_profile.html)

```python
# delete_configuration_profile method definition

await def delete_configuration_profile(
    self,
    *,
    ApplicationId: str,
    ConfigurationProfileId: str,
    DeletionProtectionCheck: DeletionProtectionCheckType = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DeletionProtectionCheckType](./literals.md#deletionprotectionchecktype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_configuration_profile method usage example with argument unpacking

kwargs: DeleteConfigurationProfileRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "ConfigurationProfileId": ...,
}

parent.delete_configuration_profile(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationProfileRequestTypeDef](./type_defs.md#deleteconfigurationprofilerequesttypedef) 

### delete\_deployment\_strategy

Deletes a deployment strategy.

Type annotations and code completion for `#!python session.create_client("appconfig").delete_deployment_strategy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/delete_deployment_strategy.html)

```python
# delete_deployment_strategy method definition

await def delete_deployment_strategy(
    self,
    *,
    DeploymentStrategyId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_deployment_strategy method usage example with argument unpacking

kwargs: DeleteDeploymentStrategyRequestTypeDef = {  # (1)
    "DeploymentStrategyId": ...,
}

parent.delete_deployment_strategy(**kwargs)
```

1. See [:material-code-braces: DeleteDeploymentStrategyRequestTypeDef](./type_defs.md#deletedeploymentstrategyrequesttypedef) 

### delete\_environment

Deletes an environment.

Type annotations and code completion for `#!python session.create_client("appconfig").delete_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/delete_environment.html)

```python
# delete_environment method definition

await def delete_environment(
    self,
    *,
    EnvironmentId: str,
    ApplicationId: str,
    DeletionProtectionCheck: DeletionProtectionCheckType = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DeletionProtectionCheckType](./literals.md#deletionprotectionchecktype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_environment method usage example with argument unpacking

kwargs: DeleteEnvironmentRequestTypeDef = {  # (1)
    "EnvironmentId": ...,
    "ApplicationId": ...,
}

parent.delete_environment(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentRequestTypeDef](./type_defs.md#deleteenvironmentrequesttypedef) 

### delete\_extension

Deletes an AppConfig extension.

Type annotations and code completion for `#!python session.create_client("appconfig").delete_extension` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/delete_extension.html)

```python
# delete_extension method definition

await def delete_extension(
    self,
    *,
    ExtensionIdentifier: str,
    VersionNumber: int = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_extension method usage example with argument unpacking

kwargs: DeleteExtensionRequestTypeDef = {  # (1)
    "ExtensionIdentifier": ...,
}

parent.delete_extension(**kwargs)
```

1. See [:material-code-braces: DeleteExtensionRequestTypeDef](./type_defs.md#deleteextensionrequesttypedef) 

### delete\_extension\_association

Deletes an extension association.

Type annotations and code completion for `#!python session.create_client("appconfig").delete_extension_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/delete_extension_association.html)

```python
# delete_extension_association method definition

await def delete_extension_association(
    self,
    *,
    ExtensionAssociationId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_extension_association method usage example with argument unpacking

kwargs: DeleteExtensionAssociationRequestTypeDef = {  # (1)
    "ExtensionAssociationId": ...,
}

parent.delete_extension_association(**kwargs)
```

1. See [:material-code-braces: DeleteExtensionAssociationRequestTypeDef](./type_defs.md#deleteextensionassociationrequesttypedef) 

### delete\_hosted\_configuration\_version

Deletes a version of a configuration from the AppConfig hosted configuration
store.

Type annotations and code completion for `#!python session.create_client("appconfig").delete_hosted_configuration_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/delete_hosted_configuration_version.html)

```python
# delete_hosted_configuration_version method definition

await def delete_hosted_configuration_version(
    self,
    *,
    ApplicationId: str,
    ConfigurationProfileId: str,
    VersionNumber: int,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_hosted_configuration_version method usage example with argument unpacking

kwargs: DeleteHostedConfigurationVersionRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "ConfigurationProfileId": ...,
    "VersionNumber": ...,
}

parent.delete_hosted_configuration_version(**kwargs)
```

1. See [:material-code-braces: DeleteHostedConfigurationVersionRequestTypeDef](./type_defs.md#deletehostedconfigurationversionrequesttypedef) 

### get\_account\_settings

Returns information about the status of the <code>DeletionProtection</code>
parameter.

Type annotations and code completion for `#!python session.create_client("appconfig").get_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/get_account_settings.html)

```python
# get_account_settings method definition

await def get_account_settings(
    self,
) -> AccountSettingsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 

### get\_application

Retrieves information about an application.

Type annotations and code completion for `#!python session.create_client("appconfig").get_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/get_application.html)

```python
# get_application method definition

await def get_application(
    self,
    *,
    ApplicationId: str,
) -> ApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef) 


```python
# get_application method usage example with argument unpacking

kwargs: GetApplicationRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.get_application(**kwargs)
```

1. See [:material-code-braces: GetApplicationRequestTypeDef](./type_defs.md#getapplicationrequesttypedef) 

### get\_configuration

(Deprecated) Retrieves the latest deployed configuration.

Type annotations and code completion for `#!python session.create_client("appconfig").get_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/get_configuration.html)

```python
# get_configuration method definition

await def get_configuration(
    self,
    *,
    Application: str,
    Environment: str,
    Configuration: str,
    ClientId: str,
    ClientConfigurationVersion: str = ...,
) -> ConfigurationTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 


```python
# get_configuration method usage example with argument unpacking

kwargs: GetConfigurationRequestTypeDef = {  # (1)
    "Application": ...,
    "Environment": ...,
    "Configuration": ...,
    "ClientId": ...,
}

parent.get_configuration(**kwargs)
```

1. See [:material-code-braces: GetConfigurationRequestTypeDef](./type_defs.md#getconfigurationrequesttypedef) 

### get\_configuration\_profile

Retrieves information about a configuration profile.

Type annotations and code completion for `#!python session.create_client("appconfig").get_configuration_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/get_configuration_profile.html)

```python
# get_configuration_profile method definition

await def get_configuration_profile(
    self,
    *,
    ApplicationId: str,
    ConfigurationProfileId: str,
) -> ConfigurationProfileTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ConfigurationProfileTypeDef](./type_defs.md#configurationprofiletypedef) 


```python
# get_configuration_profile method usage example with argument unpacking

kwargs: GetConfigurationProfileRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "ConfigurationProfileId": ...,
}

parent.get_configuration_profile(**kwargs)
```

1. See [:material-code-braces: GetConfigurationProfileRequestTypeDef](./type_defs.md#getconfigurationprofilerequesttypedef) 

### get\_deployment

Retrieves information about a configuration deployment.

Type annotations and code completion for `#!python session.create_client("appconfig").get_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/get_deployment.html)

```python
# get_deployment method definition

await def get_deployment(
    self,
    *,
    ApplicationId: str,
    EnvironmentId: str,
    DeploymentNumber: int,
) -> DeploymentTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 


```python
# get_deployment method usage example with argument unpacking

kwargs: GetDeploymentRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "EnvironmentId": ...,
    "DeploymentNumber": ...,
}

parent.get_deployment(**kwargs)
```

1. See [:material-code-braces: GetDeploymentRequestTypeDef](./type_defs.md#getdeploymentrequesttypedef) 

### get\_deployment\_strategy

Retrieves information about a deployment strategy.

Type annotations and code completion for `#!python session.create_client("appconfig").get_deployment_strategy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/get_deployment_strategy.html)

```python
# get_deployment_strategy method definition

await def get_deployment_strategy(
    self,
    *,
    DeploymentStrategyId: str,
) -> DeploymentStrategyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeploymentStrategyResponseTypeDef](./type_defs.md#deploymentstrategyresponsetypedef) 


```python
# get_deployment_strategy method usage example with argument unpacking

kwargs: GetDeploymentStrategyRequestTypeDef = {  # (1)
    "DeploymentStrategyId": ...,
}

parent.get_deployment_strategy(**kwargs)
```

1. See [:material-code-braces: GetDeploymentStrategyRequestTypeDef](./type_defs.md#getdeploymentstrategyrequesttypedef) 

### get\_environment

Retrieves information about an environment.

Type annotations and code completion for `#!python session.create_client("appconfig").get_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/get_environment.html)

```python
# get_environment method definition

await def get_environment(
    self,
    *,
    ApplicationId: str,
    EnvironmentId: str,
) -> EnvironmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EnvironmentResponseTypeDef](./type_defs.md#environmentresponsetypedef) 


```python
# get_environment method usage example with argument unpacking

kwargs: GetEnvironmentRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "EnvironmentId": ...,
}

parent.get_environment(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentRequestTypeDef](./type_defs.md#getenvironmentrequesttypedef) 

### get\_extension

Returns information about an AppConfig extension.

Type annotations and code completion for `#!python session.create_client("appconfig").get_extension` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/get_extension.html)

```python
# get_extension method definition

await def get_extension(
    self,
    *,
    ExtensionIdentifier: str,
    VersionNumber: int = ...,
) -> ExtensionTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExtensionTypeDef](./type_defs.md#extensiontypedef) 


```python
# get_extension method usage example with argument unpacking

kwargs: GetExtensionRequestTypeDef = {  # (1)
    "ExtensionIdentifier": ...,
}

parent.get_extension(**kwargs)
```

1. See [:material-code-braces: GetExtensionRequestTypeDef](./type_defs.md#getextensionrequesttypedef) 

### get\_extension\_association

Returns information about an AppConfig extension association.

Type annotations and code completion for `#!python session.create_client("appconfig").get_extension_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/get_extension_association.html)

```python
# get_extension_association method definition

await def get_extension_association(
    self,
    *,
    ExtensionAssociationId: str,
) -> ExtensionAssociationTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExtensionAssociationTypeDef](./type_defs.md#extensionassociationtypedef) 


```python
# get_extension_association method usage example with argument unpacking

kwargs: GetExtensionAssociationRequestTypeDef = {  # (1)
    "ExtensionAssociationId": ...,
}

parent.get_extension_association(**kwargs)
```

1. See [:material-code-braces: GetExtensionAssociationRequestTypeDef](./type_defs.md#getextensionassociationrequesttypedef) 

### get\_hosted\_configuration\_version

Retrieves information about a specific configuration version.

Type annotations and code completion for `#!python session.create_client("appconfig").get_hosted_configuration_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/get_hosted_configuration_version.html)

```python
# get_hosted_configuration_version method definition

await def get_hosted_configuration_version(
    self,
    *,
    ApplicationId: str,
    ConfigurationProfileId: str,
    VersionNumber: int,
) -> HostedConfigurationVersionTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: HostedConfigurationVersionTypeDef](./type_defs.md#hostedconfigurationversiontypedef) 


```python
# get_hosted_configuration_version method usage example with argument unpacking

kwargs: GetHostedConfigurationVersionRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "ConfigurationProfileId": ...,
    "VersionNumber": ...,
}

parent.get_hosted_configuration_version(**kwargs)
```

1. See [:material-code-braces: GetHostedConfigurationVersionRequestTypeDef](./type_defs.md#gethostedconfigurationversionrequesttypedef) 

### list\_applications

Lists all applications in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("appconfig").list_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/list_applications.html)

```python
# list_applications method definition

await def list_applications(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ApplicationsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ApplicationsTypeDef](./type_defs.md#applicationstypedef) 


```python
# list_applications method usage example with argument unpacking

kwargs: ListApplicationsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_applications(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestTypeDef](./type_defs.md#listapplicationsrequesttypedef) 

### list\_configuration\_profiles

Lists the configuration profiles for an application.

Type annotations and code completion for `#!python session.create_client("appconfig").list_configuration_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/list_configuration_profiles.html)

```python
# list_configuration_profiles method definition

await def list_configuration_profiles(
    self,
    *,
    ApplicationId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    Type: str = ...,
) -> ConfigurationProfilesTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ConfigurationProfilesTypeDef](./type_defs.md#configurationprofilestypedef) 


```python
# list_configuration_profiles method usage example with argument unpacking

kwargs: ListConfigurationProfilesRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.list_configuration_profiles(**kwargs)
```

1. See [:material-code-braces: ListConfigurationProfilesRequestTypeDef](./type_defs.md#listconfigurationprofilesrequesttypedef) 

### list\_deployment\_strategies

Lists deployment strategies.

Type annotations and code completion for `#!python session.create_client("appconfig").list_deployment_strategies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/list_deployment_strategies.html)

```python
# list_deployment_strategies method definition

await def list_deployment_strategies(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DeploymentStrategiesTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeploymentStrategiesTypeDef](./type_defs.md#deploymentstrategiestypedef) 


```python
# list_deployment_strategies method usage example with argument unpacking

kwargs: ListDeploymentStrategiesRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_deployment_strategies(**kwargs)
```

1. See [:material-code-braces: ListDeploymentStrategiesRequestTypeDef](./type_defs.md#listdeploymentstrategiesrequesttypedef) 

### list\_deployments

Lists the deployments for an environment in descending deployment number order.

Type annotations and code completion for `#!python session.create_client("appconfig").list_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/list_deployments.html)

```python
# list_deployments method definition

await def list_deployments(
    self,
    *,
    ApplicationId: str,
    EnvironmentId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DeploymentsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeploymentsTypeDef](./type_defs.md#deploymentstypedef) 


```python
# list_deployments method usage example with argument unpacking

kwargs: ListDeploymentsRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "EnvironmentId": ...,
}

parent.list_deployments(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsRequestTypeDef](./type_defs.md#listdeploymentsrequesttypedef) 

### list\_environments

Lists the environments for an application.

Type annotations and code completion for `#!python session.create_client("appconfig").list_environments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/list_environments.html)

```python
# list_environments method definition

await def list_environments(
    self,
    *,
    ApplicationId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> EnvironmentsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EnvironmentsTypeDef](./type_defs.md#environmentstypedef) 


```python
# list_environments method usage example with argument unpacking

kwargs: ListEnvironmentsRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.list_environments(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsRequestTypeDef](./type_defs.md#listenvironmentsrequesttypedef) 

### list\_extension\_associations

Lists all AppConfig extension associations in the account.

Type annotations and code completion for `#!python session.create_client("appconfig").list_extension_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/list_extension_associations.html)

```python
# list_extension_associations method definition

await def list_extension_associations(
    self,
    *,
    ResourceIdentifier: str = ...,
    ExtensionIdentifier: str = ...,
    ExtensionVersionNumber: int = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ExtensionAssociationsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExtensionAssociationsTypeDef](./type_defs.md#extensionassociationstypedef) 


```python
# list_extension_associations method usage example with argument unpacking

kwargs: ListExtensionAssociationsRequestTypeDef = {  # (1)
    "ResourceIdentifier": ...,
}

parent.list_extension_associations(**kwargs)
```

1. See [:material-code-braces: ListExtensionAssociationsRequestTypeDef](./type_defs.md#listextensionassociationsrequesttypedef) 

### list\_extensions

Lists all custom and Amazon Web Services authored AppConfig extensions in the
account.

Type annotations and code completion for `#!python session.create_client("appconfig").list_extensions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/list_extensions.html)

```python
# list_extensions method definition

await def list_extensions(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Name: str = ...,
) -> ExtensionsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExtensionsTypeDef](./type_defs.md#extensionstypedef) 


```python
# list_extensions method usage example with argument unpacking

kwargs: ListExtensionsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_extensions(**kwargs)
```

1. See [:material-code-braces: ListExtensionsRequestTypeDef](./type_defs.md#listextensionsrequesttypedef) 

### list\_hosted\_configuration\_versions

Lists configurations stored in the AppConfig hosted configuration store by
version.

Type annotations and code completion for `#!python session.create_client("appconfig").list_hosted_configuration_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/list_hosted_configuration_versions.html)

```python
# list_hosted_configuration_versions method definition

await def list_hosted_configuration_versions(
    self,
    *,
    ApplicationId: str,
    ConfigurationProfileId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    VersionLabel: str = ...,
) -> HostedConfigurationVersionsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: HostedConfigurationVersionsTypeDef](./type_defs.md#hostedconfigurationversionstypedef) 


```python
# list_hosted_configuration_versions method usage example with argument unpacking

kwargs: ListHostedConfigurationVersionsRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "ConfigurationProfileId": ...,
}

parent.list_hosted_configuration_versions(**kwargs)
```

1. See [:material-code-braces: ListHostedConfigurationVersionsRequestTypeDef](./type_defs.md#listhostedconfigurationversionsrequesttypedef) 

### list\_tags\_for\_resource

Retrieves the list of key-value tags assigned to the resource.

Type annotations and code completion for `#!python session.create_client("appconfig").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ResourceTagsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResourceTagsTypeDef](./type_defs.md#resourcetagstypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### start\_deployment

Starts a deployment.

Type annotations and code completion for `#!python session.create_client("appconfig").start_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/start_deployment.html)

```python
# start_deployment method definition

await def start_deployment(
    self,
    *,
    ApplicationId: str,
    EnvironmentId: str,
    DeploymentStrategyId: str,
    ConfigurationProfileId: str,
    ConfigurationVersion: str,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
    KmsKeyIdentifier: str = ...,
    DynamicExtensionParameters: Mapping[str, str] = ...,
) -> DeploymentTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 


```python
# start_deployment method usage example with argument unpacking

kwargs: StartDeploymentRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "EnvironmentId": ...,
    "DeploymentStrategyId": ...,
    "ConfigurationProfileId": ...,
    "ConfigurationVersion": ...,
}

parent.start_deployment(**kwargs)
```

1. See [:material-code-braces: StartDeploymentRequestTypeDef](./type_defs.md#startdeploymentrequesttypedef) 

### stop\_deployment

Stops a deployment.

Type annotations and code completion for `#!python session.create_client("appconfig").stop_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/stop_deployment.html)

```python
# stop_deployment method definition

await def stop_deployment(
    self,
    *,
    ApplicationId: str,
    EnvironmentId: str,
    DeploymentNumber: int,
    AllowRevert: bool = ...,
) -> DeploymentTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 


```python
# stop_deployment method usage example with argument unpacking

kwargs: StopDeploymentRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "EnvironmentId": ...,
    "DeploymentNumber": ...,
}

parent.stop_deployment(**kwargs)
```

1. See [:material-code-braces: StopDeploymentRequestTypeDef](./type_defs.md#stopdeploymentrequesttypedef) 

### tag\_resource

Assigns metadata to an AppConfig resource.

Type annotations and code completion for `#!python session.create_client("appconfig").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/tag_resource.html)

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

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Deletes a tag key and value from an AppConfig resource.

Type annotations and code completion for `#!python session.create_client("appconfig").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/untag_resource.html)

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

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_account\_settings

Updates the value of the <code>DeletionProtection</code> parameter.

Type annotations and code completion for `#!python session.create_client("appconfig").update_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/update_account_settings.html)

```python
# update_account_settings method definition

await def update_account_settings(
    self,
    *,
    DeletionProtection: DeletionProtectionSettingsTypeDef = ...,  # (1)
) -> AccountSettingsTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeletionProtectionSettingsTypeDef](./type_defs.md#deletionprotectionsettingstypedef) 
2. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 


```python
# update_account_settings method usage example with argument unpacking

kwargs: UpdateAccountSettingsRequestTypeDef = {  # (1)
    "DeletionProtection": ...,
}

parent.update_account_settings(**kwargs)
```

1. See [:material-code-braces: UpdateAccountSettingsRequestTypeDef](./type_defs.md#updateaccountsettingsrequesttypedef) 

### update\_application

Updates an application.

Type annotations and code completion for `#!python session.create_client("appconfig").update_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/update_application.html)

```python
# update_application method definition

await def update_application(
    self,
    *,
    ApplicationId: str,
    Name: str = ...,
    Description: str = ...,
) -> ApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef) 


```python
# update_application method usage example with argument unpacking

kwargs: UpdateApplicationRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.update_application(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationRequestTypeDef](./type_defs.md#updateapplicationrequesttypedef) 

### update\_configuration\_profile

Updates a configuration profile.

Type annotations and code completion for `#!python session.create_client("appconfig").update_configuration_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/update_configuration_profile.html)

```python
# update_configuration_profile method definition

await def update_configuration_profile(
    self,
    *,
    ApplicationId: str,
    ConfigurationProfileId: str,
    Name: str = ...,
    Description: str = ...,
    RetrievalRoleArn: str = ...,
    Validators: Sequence[ValidatorTypeDef] = ...,  # (1)
    KmsKeyIdentifier: str = ...,
) -> ConfigurationProfileTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ValidatorTypeDef](./type_defs.md#validatortypedef) 
2. See [:material-code-braces: ConfigurationProfileTypeDef](./type_defs.md#configurationprofiletypedef) 


```python
# update_configuration_profile method usage example with argument unpacking

kwargs: UpdateConfigurationProfileRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "ConfigurationProfileId": ...,
}

parent.update_configuration_profile(**kwargs)
```

1. See [:material-code-braces: UpdateConfigurationProfileRequestTypeDef](./type_defs.md#updateconfigurationprofilerequesttypedef) 

### update\_deployment\_strategy

Updates a deployment strategy.

Type annotations and code completion for `#!python session.create_client("appconfig").update_deployment_strategy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/update_deployment_strategy.html)

```python
# update_deployment_strategy method definition

await def update_deployment_strategy(
    self,
    *,
    DeploymentStrategyId: str,
    Description: str = ...,
    DeploymentDurationInMinutes: int = ...,
    FinalBakeTimeInMinutes: int = ...,
    GrowthFactor: float = ...,
    GrowthType: GrowthTypeType = ...,  # (1)
) -> DeploymentStrategyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GrowthTypeType](./literals.md#growthtypetype) 
2. See [:material-code-braces: DeploymentStrategyResponseTypeDef](./type_defs.md#deploymentstrategyresponsetypedef) 


```python
# update_deployment_strategy method usage example with argument unpacking

kwargs: UpdateDeploymentStrategyRequestTypeDef = {  # (1)
    "DeploymentStrategyId": ...,
}

parent.update_deployment_strategy(**kwargs)
```

1. See [:material-code-braces: UpdateDeploymentStrategyRequestTypeDef](./type_defs.md#updatedeploymentstrategyrequesttypedef) 

### update\_environment

Updates an environment.

Type annotations and code completion for `#!python session.create_client("appconfig").update_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/update_environment.html)

```python
# update_environment method definition

await def update_environment(
    self,
    *,
    ApplicationId: str,
    EnvironmentId: str,
    Name: str = ...,
    Description: str = ...,
    Monitors: Sequence[MonitorTypeDef] = ...,  # (1)
) -> EnvironmentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MonitorTypeDef](./type_defs.md#monitortypedef) 
2. See [:material-code-braces: EnvironmentResponseTypeDef](./type_defs.md#environmentresponsetypedef) 


```python
# update_environment method usage example with argument unpacking

kwargs: UpdateEnvironmentRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "EnvironmentId": ...,
}

parent.update_environment(**kwargs)
```

1. See [:material-code-braces: UpdateEnvironmentRequestTypeDef](./type_defs.md#updateenvironmentrequesttypedef) 

### update\_extension

Updates an AppConfig extension.

Type annotations and code completion for `#!python session.create_client("appconfig").update_extension` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/update_extension.html)

```python
# update_extension method definition

await def update_extension(
    self,
    *,
    ExtensionIdentifier: str,
    Description: str = ...,
    Actions: Mapping[ActionPointType, Sequence[ActionTypeDef]] = ...,  # (1)
    Parameters: Mapping[str, ParameterTypeDef] = ...,  # (2)
    VersionNumber: int = ...,
) -> ExtensionTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ActionPointType](./literals.md#actionpointtype) [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
3. See [:material-code-braces: ExtensionTypeDef](./type_defs.md#extensiontypedef) 


```python
# update_extension method usage example with argument unpacking

kwargs: UpdateExtensionRequestTypeDef = {  # (1)
    "ExtensionIdentifier": ...,
}

parent.update_extension(**kwargs)
```

1. See [:material-code-braces: UpdateExtensionRequestTypeDef](./type_defs.md#updateextensionrequesttypedef) 

### update\_extension\_association

Updates an association.

Type annotations and code completion for `#!python session.create_client("appconfig").update_extension_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/update_extension_association.html)

```python
# update_extension_association method definition

await def update_extension_association(
    self,
    *,
    ExtensionAssociationId: str,
    Parameters: Mapping[str, str] = ...,
) -> ExtensionAssociationTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExtensionAssociationTypeDef](./type_defs.md#extensionassociationtypedef) 


```python
# update_extension_association method usage example with argument unpacking

kwargs: UpdateExtensionAssociationRequestTypeDef = {  # (1)
    "ExtensionAssociationId": ...,
}

parent.update_extension_association(**kwargs)
```

1. See [:material-code-braces: UpdateExtensionAssociationRequestTypeDef](./type_defs.md#updateextensionassociationrequesttypedef) 

### validate\_configuration

Uses the validators in a configuration profile to validate a configuration.

Type annotations and code completion for `#!python session.create_client("appconfig").validate_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig/client/validate_configuration.html)

```python
# validate_configuration method definition

await def validate_configuration(
    self,
    *,
    ApplicationId: str,
    ConfigurationProfileId: str,
    ConfigurationVersion: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# validate_configuration method usage example with argument unpacking

kwargs: ValidateConfigurationRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "ConfigurationProfileId": ...,
    "ConfigurationVersion": ...,
}

parent.validate_configuration(**kwargs)
```

1. See [:material-code-braces: ValidateConfigurationRequestTypeDef](./type_defs.md#validateconfigurationrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("appconfig").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("appconfig").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client)

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

Type annotations and code completion for `#!python session.create_client("appconfig").get_paginator` method with overloads.

- `client.get_paginator("list_applications")` -> [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- `client.get_paginator("list_configuration_profiles")` -> [ListConfigurationProfilesPaginator](./paginators.md#listconfigurationprofilespaginator)
- `client.get_paginator("list_deployment_strategies")` -> [ListDeploymentStrategiesPaginator](./paginators.md#listdeploymentstrategiespaginator)
- `client.get_paginator("list_deployments")` -> [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
- `client.get_paginator("list_environments")` -> [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
- `client.get_paginator("list_extension_associations")` -> [ListExtensionAssociationsPaginator](./paginators.md#listextensionassociationspaginator)
- `client.get_paginator("list_extensions")` -> [ListExtensionsPaginator](./paginators.md#listextensionspaginator)
- `client.get_paginator("list_hosted_configuration_versions")` -> [ListHostedConfigurationVersionsPaginator](./paginators.md#listhostedconfigurationversionspaginator)



