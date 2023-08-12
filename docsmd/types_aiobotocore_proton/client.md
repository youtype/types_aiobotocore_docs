# ProtonClient

> [Index](../README.md) > [Proton](./README.md) > ProtonClient

!!! note ""

    Auto-generated documentation for [Proton](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
    type annotations stubs module [types-aiobotocore-proton](https://pypi.org/project/types-aiobotocore-proton/).

## ProtonClient

Type annotations and code completion for `#!python session.create_client("proton")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client)

```python
ProtonClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_proton.client import ProtonClient

session = get_session()
async with session.create_client("proton") as client:
    client: ProtonClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("proton").exceptions` structure.

```python
ProtonClient.exceptions usage example

async with session.create_client("proton") as client:
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
ProtonClient usage type checking example

from types_aiobotocore_proton.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### accept\_environment\_account\_connection

In a management account, an environment account connection request is accepted.

Type annotations and code completion for `#!python session.create_client("proton").accept_environment_account_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.accept_environment_account_connection)

```python
# accept_environment_account_connection method definition

await def accept_environment_account_connection(
    self,
    *,
    id: str,
) -> AcceptEnvironmentAccountConnectionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AcceptEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#acceptenvironmentaccountconnectionoutputtypedef) 


```python
# accept_environment_account_connection method usage example with argument unpacking

kwargs: AcceptEnvironmentAccountConnectionInputRequestTypeDef = {  # (1)
    "id": ...,
}

parent.accept_environment_account_connection(**kwargs)
```

1. See [:material-code-braces: AcceptEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#acceptenvironmentaccountconnectioninputrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("proton").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_component\_deployment

Attempts to cancel a component deployment (for a component that is in the
`IN_PROGRESS` deployment status).

Type annotations and code completion for `#!python session.create_client("proton").cancel_component_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_component_deployment)

```python
# cancel_component_deployment method definition

await def cancel_component_deployment(
    self,
    *,
    componentName: str,
) -> CancelComponentDeploymentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelComponentDeploymentOutputTypeDef](./type_defs.md#cancelcomponentdeploymentoutputtypedef) 


```python
# cancel_component_deployment method usage example with argument unpacking

kwargs: CancelComponentDeploymentInputRequestTypeDef = {  # (1)
    "componentName": ...,
}

parent.cancel_component_deployment(**kwargs)
```

1. See [:material-code-braces: CancelComponentDeploymentInputRequestTypeDef](./type_defs.md#cancelcomponentdeploymentinputrequesttypedef) 

### cancel\_environment\_deployment

Attempts to cancel an environment deployment on an  UpdateEnvironment action, if
the deployment is `IN_PROGRESS`.

Type annotations and code completion for `#!python session.create_client("proton").cancel_environment_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_environment_deployment)

```python
# cancel_environment_deployment method definition

await def cancel_environment_deployment(
    self,
    *,
    environmentName: str,
) -> CancelEnvironmentDeploymentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelEnvironmentDeploymentOutputTypeDef](./type_defs.md#cancelenvironmentdeploymentoutputtypedef) 


```python
# cancel_environment_deployment method usage example with argument unpacking

kwargs: CancelEnvironmentDeploymentInputRequestTypeDef = {  # (1)
    "environmentName": ...,
}

parent.cancel_environment_deployment(**kwargs)
```

1. See [:material-code-braces: CancelEnvironmentDeploymentInputRequestTypeDef](./type_defs.md#cancelenvironmentdeploymentinputrequesttypedef) 

### cancel\_service\_instance\_deployment

Attempts to cancel a service instance deployment on an  UpdateServiceInstance
action, if the deployment is `IN_PROGRESS`.

Type annotations and code completion for `#!python session.create_client("proton").cancel_service_instance_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_instance_deployment)

```python
# cancel_service_instance_deployment method definition

await def cancel_service_instance_deployment(
    self,
    *,
    serviceInstanceName: str,
    serviceName: str,
) -> CancelServiceInstanceDeploymentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelServiceInstanceDeploymentOutputTypeDef](./type_defs.md#cancelserviceinstancedeploymentoutputtypedef) 


```python
# cancel_service_instance_deployment method usage example with argument unpacking

kwargs: CancelServiceInstanceDeploymentInputRequestTypeDef = {  # (1)
    "serviceInstanceName": ...,
    "serviceName": ...,
}

parent.cancel_service_instance_deployment(**kwargs)
```

1. See [:material-code-braces: CancelServiceInstanceDeploymentInputRequestTypeDef](./type_defs.md#cancelserviceinstancedeploymentinputrequesttypedef) 

### cancel\_service\_pipeline\_deployment

Attempts to cancel a service pipeline deployment on an  UpdateServicePipeline
action, if the deployment is `IN_PROGRESS`.

Type annotations and code completion for `#!python session.create_client("proton").cancel_service_pipeline_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_pipeline_deployment)

```python
# cancel_service_pipeline_deployment method definition

await def cancel_service_pipeline_deployment(
    self,
    *,
    serviceName: str,
) -> CancelServicePipelineDeploymentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelServicePipelineDeploymentOutputTypeDef](./type_defs.md#cancelservicepipelinedeploymentoutputtypedef) 


```python
# cancel_service_pipeline_deployment method usage example with argument unpacking

kwargs: CancelServicePipelineDeploymentInputRequestTypeDef = {  # (1)
    "serviceName": ...,
}

parent.cancel_service_pipeline_deployment(**kwargs)
```

1. See [:material-code-braces: CancelServicePipelineDeploymentInputRequestTypeDef](./type_defs.md#cancelservicepipelinedeploymentinputrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("proton").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_component

Create an Proton component.

Type annotations and code completion for `#!python session.create_client("proton").create_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_component)

```python
# create_component method definition

await def create_component(
    self,
    *,
    manifest: str,
    name: str,
    templateFile: str,
    clientToken: str = ...,
    description: str = ...,
    environmentName: str = ...,
    serviceInstanceName: str = ...,
    serviceName: str = ...,
    serviceSpec: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateComponentOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateComponentOutputTypeDef](./type_defs.md#createcomponentoutputtypedef) 


```python
# create_component method usage example with argument unpacking

kwargs: CreateComponentInputRequestTypeDef = {  # (1)
    "manifest": ...,
    "name": ...,
    "templateFile": ...,
}

parent.create_component(**kwargs)
```

1. See [:material-code-braces: CreateComponentInputRequestTypeDef](./type_defs.md#createcomponentinputrequesttypedef) 

### create\_environment

Deploy a new environment.

Type annotations and code completion for `#!python session.create_client("proton").create_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment)

```python
# create_environment method definition

await def create_environment(
    self,
    *,
    name: str,
    spec: str,
    templateMajorVersion: str,
    templateName: str,
    codebuildRoleArn: str = ...,
    componentRoleArn: str = ...,
    description: str = ...,
    environmentAccountConnectionId: str = ...,
    protonServiceRoleArn: str = ...,
    provisioningRepository: RepositoryBranchInputTypeDef = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
    templateMinorVersion: str = ...,
) -> CreateEnvironmentOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RepositoryBranchInputTypeDef](./type_defs.md#repositorybranchinputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateEnvironmentOutputTypeDef](./type_defs.md#createenvironmentoutputtypedef) 


```python
# create_environment method usage example with argument unpacking

kwargs: CreateEnvironmentInputRequestTypeDef = {  # (1)
    "name": ...,
    "spec": ...,
    "templateMajorVersion": ...,
    "templateName": ...,
}

parent.create_environment(**kwargs)
```

1. See [:material-code-braces: CreateEnvironmentInputRequestTypeDef](./type_defs.md#createenvironmentinputrequesttypedef) 

### create\_environment\_account\_connection

Create an environment account connection in an environment account so that
environment infrastructure resources can be provisioned in the environment
account from a management account.

Type annotations and code completion for `#!python session.create_client("proton").create_environment_account_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_account_connection)

```python
# create_environment_account_connection method definition

await def create_environment_account_connection(
    self,
    *,
    environmentName: str,
    managementAccountId: str,
    clientToken: str = ...,
    codebuildRoleArn: str = ...,
    componentRoleArn: str = ...,
    roleArn: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateEnvironmentAccountConnectionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#createenvironmentaccountconnectionoutputtypedef) 


```python
# create_environment_account_connection method usage example with argument unpacking

kwargs: CreateEnvironmentAccountConnectionInputRequestTypeDef = {  # (1)
    "environmentName": ...,
    "managementAccountId": ...,
}

parent.create_environment_account_connection(**kwargs)
```

1. See [:material-code-braces: CreateEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#createenvironmentaccountconnectioninputrequesttypedef) 

### create\_environment\_template

Create an environment template for Proton.

Type annotations and code completion for `#!python session.create_client("proton").create_environment_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template)

```python
# create_environment_template method definition

await def create_environment_template(
    self,
    *,
    name: str,
    description: str = ...,
    displayName: str = ...,
    encryptionKey: str = ...,
    provisioning: ProvisioningType = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateEnvironmentTemplateOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ProvisioningType](./literals.md#provisioningtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateEnvironmentTemplateOutputTypeDef](./type_defs.md#createenvironmenttemplateoutputtypedef) 


```python
# create_environment_template method usage example with argument unpacking

kwargs: CreateEnvironmentTemplateInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_environment_template(**kwargs)
```

1. See [:material-code-braces: CreateEnvironmentTemplateInputRequestTypeDef](./type_defs.md#createenvironmenttemplateinputrequesttypedef) 

### create\_environment\_template\_version

Create a new major or minor version of an environment template.

Type annotations and code completion for `#!python session.create_client("proton").create_environment_template_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template_version)

```python
# create_environment_template_version method definition

await def create_environment_template_version(
    self,
    *,
    source: TemplateVersionSourceInputTypeDef,  # (1)
    templateName: str,
    clientToken: str = ...,
    description: str = ...,
    majorVersion: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateEnvironmentTemplateVersionOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TemplateVersionSourceInputTypeDef](./type_defs.md#templateversionsourceinputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateEnvironmentTemplateVersionOutputTypeDef](./type_defs.md#createenvironmenttemplateversionoutputtypedef) 


```python
# create_environment_template_version method usage example with argument unpacking

kwargs: CreateEnvironmentTemplateVersionInputRequestTypeDef = {  # (1)
    "source": ...,
    "templateName": ...,
}

parent.create_environment_template_version(**kwargs)
```

1. See [:material-code-braces: CreateEnvironmentTemplateVersionInputRequestTypeDef](./type_defs.md#createenvironmenttemplateversioninputrequesttypedef) 

### create\_repository

Create and register a link to a repository.

Type annotations and code completion for `#!python session.create_client("proton").create_repository` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_repository)

```python
# create_repository method definition

await def create_repository(
    self,
    *,
    connectionArn: str,
    name: str,
    provider: RepositoryProviderType,  # (1)
    encryptionKey: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateRepositoryOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateRepositoryOutputTypeDef](./type_defs.md#createrepositoryoutputtypedef) 


```python
# create_repository method usage example with argument unpacking

kwargs: CreateRepositoryInputRequestTypeDef = {  # (1)
    "connectionArn": ...,
    "name": ...,
    "provider": ...,
}

parent.create_repository(**kwargs)
```

1. See [:material-code-braces: CreateRepositoryInputRequestTypeDef](./type_defs.md#createrepositoryinputrequesttypedef) 

### create\_service

Create an Proton service.

Type annotations and code completion for `#!python session.create_client("proton").create_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service)

```python
# create_service method definition

await def create_service(
    self,
    *,
    name: str,
    spec: str,
    templateMajorVersion: str,
    templateName: str,
    branchName: str = ...,
    description: str = ...,
    repositoryConnectionArn: str = ...,
    repositoryId: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
    templateMinorVersion: str = ...,
) -> CreateServiceOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateServiceOutputTypeDef](./type_defs.md#createserviceoutputtypedef) 


```python
# create_service method usage example with argument unpacking

kwargs: CreateServiceInputRequestTypeDef = {  # (1)
    "name": ...,
    "spec": ...,
    "templateMajorVersion": ...,
    "templateName": ...,
}

parent.create_service(**kwargs)
```

1. See [:material-code-braces: CreateServiceInputRequestTypeDef](./type_defs.md#createserviceinputrequesttypedef) 

### create\_service\_instance

Create a service instance.

Type annotations and code completion for `#!python session.create_client("proton").create_service_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_instance)

```python
# create_service_instance method definition

await def create_service_instance(
    self,
    *,
    name: str,
    serviceName: str,
    spec: str,
    clientToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
    templateMajorVersion: str = ...,
    templateMinorVersion: str = ...,
) -> CreateServiceInstanceOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateServiceInstanceOutputTypeDef](./type_defs.md#createserviceinstanceoutputtypedef) 


```python
# create_service_instance method usage example with argument unpacking

kwargs: CreateServiceInstanceInputRequestTypeDef = {  # (1)
    "name": ...,
    "serviceName": ...,
    "spec": ...,
}

parent.create_service_instance(**kwargs)
```

1. See [:material-code-braces: CreateServiceInstanceInputRequestTypeDef](./type_defs.md#createserviceinstanceinputrequesttypedef) 

### create\_service\_sync\_config

Create the Proton Ops configuration file.

Type annotations and code completion for `#!python session.create_client("proton").create_service_sync_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_sync_config)

```python
# create_service_sync_config method definition

await def create_service_sync_config(
    self,
    *,
    branch: str,
    filePath: str,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    serviceName: str,
) -> CreateServiceSyncConfigOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-braces: CreateServiceSyncConfigOutputTypeDef](./type_defs.md#createservicesyncconfigoutputtypedef) 


```python
# create_service_sync_config method usage example with argument unpacking

kwargs: CreateServiceSyncConfigInputRequestTypeDef = {  # (1)
    "branch": ...,
    "filePath": ...,
    "repositoryName": ...,
    "repositoryProvider": ...,
    "serviceName": ...,
}

parent.create_service_sync_config(**kwargs)
```

1. See [:material-code-braces: CreateServiceSyncConfigInputRequestTypeDef](./type_defs.md#createservicesyncconfiginputrequesttypedef) 

### create\_service\_template

Create a service template.

Type annotations and code completion for `#!python session.create_client("proton").create_service_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template)

```python
# create_service_template method definition

await def create_service_template(
    self,
    *,
    name: str,
    description: str = ...,
    displayName: str = ...,
    encryptionKey: str = ...,
    pipelineProvisioning: ProvisioningType = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateServiceTemplateOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ProvisioningType](./literals.md#provisioningtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateServiceTemplateOutputTypeDef](./type_defs.md#createservicetemplateoutputtypedef) 


```python
# create_service_template method usage example with argument unpacking

kwargs: CreateServiceTemplateInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_service_template(**kwargs)
```

1. See [:material-code-braces: CreateServiceTemplateInputRequestTypeDef](./type_defs.md#createservicetemplateinputrequesttypedef) 

### create\_service\_template\_version

Create a new major or minor version of a service template.

Type annotations and code completion for `#!python session.create_client("proton").create_service_template_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template_version)

```python
# create_service_template_version method definition

await def create_service_template_version(
    self,
    *,
    compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef],  # (1)
    source: TemplateVersionSourceInputTypeDef,  # (2)
    templateName: str,
    clientToken: str = ...,
    description: str = ...,
    majorVersion: str = ...,
    supportedComponentSources: Sequence[ServiceTemplateSupportedComponentSourceTypeType] = ...,  # (3)
    tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateServiceTemplateVersionOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: CompatibleEnvironmentTemplateInputTypeDef](./type_defs.md#compatibleenvironmenttemplateinputtypedef) 
2. See [:material-code-braces: TemplateVersionSourceInputTypeDef](./type_defs.md#templateversionsourceinputtypedef) 
3. See [:material-code-brackets: ServiceTemplateSupportedComponentSourceTypeType](./literals.md#servicetemplatesupportedcomponentsourcetypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateServiceTemplateVersionOutputTypeDef](./type_defs.md#createservicetemplateversionoutputtypedef) 


```python
# create_service_template_version method usage example with argument unpacking

kwargs: CreateServiceTemplateVersionInputRequestTypeDef = {  # (1)
    "compatibleEnvironmentTemplates": ...,
    "source": ...,
    "templateName": ...,
}

parent.create_service_template_version(**kwargs)
```

1. See [:material-code-braces: CreateServiceTemplateVersionInputRequestTypeDef](./type_defs.md#createservicetemplateversioninputrequesttypedef) 

### create\_template\_sync\_config

Set up a template to create new template versions automatically by tracking a
linked repository.

Type annotations and code completion for `#!python session.create_client("proton").create_template_sync_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_template_sync_config)

```python
# create_template_sync_config method definition

await def create_template_sync_config(
    self,
    *,
    branch: str,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    templateName: str,
    templateType: TemplateTypeType,  # (2)
    subdirectory: str = ...,
) -> CreateTemplateSyncConfigOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
3. See [:material-code-braces: CreateTemplateSyncConfigOutputTypeDef](./type_defs.md#createtemplatesyncconfigoutputtypedef) 


```python
# create_template_sync_config method usage example with argument unpacking

kwargs: CreateTemplateSyncConfigInputRequestTypeDef = {  # (1)
    "branch": ...,
    "repositoryName": ...,
    "repositoryProvider": ...,
    "templateName": ...,
    "templateType": ...,
}

parent.create_template_sync_config(**kwargs)
```

1. See [:material-code-braces: CreateTemplateSyncConfigInputRequestTypeDef](./type_defs.md#createtemplatesyncconfiginputrequesttypedef) 

### delete\_component

Delete an Proton component resource.

Type annotations and code completion for `#!python session.create_client("proton").delete_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_component)

```python
# delete_component method definition

await def delete_component(
    self,
    *,
    name: str,
) -> DeleteComponentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteComponentOutputTypeDef](./type_defs.md#deletecomponentoutputtypedef) 


```python
# delete_component method usage example with argument unpacking

kwargs: DeleteComponentInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_component(**kwargs)
```

1. See [:material-code-braces: DeleteComponentInputRequestTypeDef](./type_defs.md#deletecomponentinputrequesttypedef) 

### delete\_deployment

Delete the deployment.

Type annotations and code completion for `#!python session.create_client("proton").delete_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_deployment)

```python
# delete_deployment method definition

await def delete_deployment(
    self,
    *,
    id: str,
) -> DeleteDeploymentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDeploymentOutputTypeDef](./type_defs.md#deletedeploymentoutputtypedef) 


```python
# delete_deployment method usage example with argument unpacking

kwargs: DeleteDeploymentInputRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_deployment(**kwargs)
```

1. See [:material-code-braces: DeleteDeploymentInputRequestTypeDef](./type_defs.md#deletedeploymentinputrequesttypedef) 

### delete\_environment

Delete an environment.

Type annotations and code completion for `#!python session.create_client("proton").delete_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment)

```python
# delete_environment method definition

await def delete_environment(
    self,
    *,
    name: str,
) -> DeleteEnvironmentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteEnvironmentOutputTypeDef](./type_defs.md#deleteenvironmentoutputtypedef) 


```python
# delete_environment method usage example with argument unpacking

kwargs: DeleteEnvironmentInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_environment(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentInputRequestTypeDef](./type_defs.md#deleteenvironmentinputrequesttypedef) 

### delete\_environment\_account\_connection

In an environment account, delete an environment account connection.

Type annotations and code completion for `#!python session.create_client("proton").delete_environment_account_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_account_connection)

```python
# delete_environment_account_connection method definition

await def delete_environment_account_connection(
    self,
    *,
    id: str,
) -> DeleteEnvironmentAccountConnectionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#deleteenvironmentaccountconnectionoutputtypedef) 


```python
# delete_environment_account_connection method usage example with argument unpacking

kwargs: DeleteEnvironmentAccountConnectionInputRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_environment_account_connection(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#deleteenvironmentaccountconnectioninputrequesttypedef) 

### delete\_environment\_template

If no other major or minor versions of an environment template exist, delete the
environment template.

Type annotations and code completion for `#!python session.create_client("proton").delete_environment_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template)

```python
# delete_environment_template method definition

await def delete_environment_template(
    self,
    *,
    name: str,
) -> DeleteEnvironmentTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteEnvironmentTemplateOutputTypeDef](./type_defs.md#deleteenvironmenttemplateoutputtypedef) 


```python
# delete_environment_template method usage example with argument unpacking

kwargs: DeleteEnvironmentTemplateInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_environment_template(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentTemplateInputRequestTypeDef](./type_defs.md#deleteenvironmenttemplateinputrequesttypedef) 

### delete\_environment\_template\_version

If no other minor versions of an environment template exist, delete a major
version of the environment template if it's not the `Recommended` version.

Type annotations and code completion for `#!python session.create_client("proton").delete_environment_template_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template_version)

```python
# delete_environment_template_version method definition

await def delete_environment_template_version(
    self,
    *,
    majorVersion: str,
    minorVersion: str,
    templateName: str,
) -> DeleteEnvironmentTemplateVersionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteEnvironmentTemplateVersionOutputTypeDef](./type_defs.md#deleteenvironmenttemplateversionoutputtypedef) 


```python
# delete_environment_template_version method usage example with argument unpacking

kwargs: DeleteEnvironmentTemplateVersionInputRequestTypeDef = {  # (1)
    "majorVersion": ...,
    "minorVersion": ...,
    "templateName": ...,
}

parent.delete_environment_template_version(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentTemplateVersionInputRequestTypeDef](./type_defs.md#deleteenvironmenttemplateversioninputrequesttypedef) 

### delete\_repository

De-register and unlink your repository.

Type annotations and code completion for `#!python session.create_client("proton").delete_repository` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_repository)

```python
# delete_repository method definition

await def delete_repository(
    self,
    *,
    name: str,
    provider: RepositoryProviderType,  # (1)
) -> DeleteRepositoryOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-braces: DeleteRepositoryOutputTypeDef](./type_defs.md#deleterepositoryoutputtypedef) 


```python
# delete_repository method usage example with argument unpacking

kwargs: DeleteRepositoryInputRequestTypeDef = {  # (1)
    "name": ...,
    "provider": ...,
}

parent.delete_repository(**kwargs)
```

1. See [:material-code-braces: DeleteRepositoryInputRequestTypeDef](./type_defs.md#deleterepositoryinputrequesttypedef) 

### delete\_service

Delete a service, with its instances and pipeline.

Type annotations and code completion for `#!python session.create_client("proton").delete_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service)

```python
# delete_service method definition

await def delete_service(
    self,
    *,
    name: str,
) -> DeleteServiceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteServiceOutputTypeDef](./type_defs.md#deleteserviceoutputtypedef) 


```python
# delete_service method usage example with argument unpacking

kwargs: DeleteServiceInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_service(**kwargs)
```

1. See [:material-code-braces: DeleteServiceInputRequestTypeDef](./type_defs.md#deleteserviceinputrequesttypedef) 

### delete\_service\_sync\_config

Delete the Proton Ops file.

Type annotations and code completion for `#!python session.create_client("proton").delete_service_sync_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_sync_config)

```python
# delete_service_sync_config method definition

await def delete_service_sync_config(
    self,
    *,
    serviceName: str,
) -> DeleteServiceSyncConfigOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteServiceSyncConfigOutputTypeDef](./type_defs.md#deleteservicesyncconfigoutputtypedef) 


```python
# delete_service_sync_config method usage example with argument unpacking

kwargs: DeleteServiceSyncConfigInputRequestTypeDef = {  # (1)
    "serviceName": ...,
}

parent.delete_service_sync_config(**kwargs)
```

1. See [:material-code-braces: DeleteServiceSyncConfigInputRequestTypeDef](./type_defs.md#deleteservicesyncconfiginputrequesttypedef) 

### delete\_service\_template

If no other major or minor versions of the service template exist, delete the
service template.

Type annotations and code completion for `#!python session.create_client("proton").delete_service_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template)

```python
# delete_service_template method definition

await def delete_service_template(
    self,
    *,
    name: str,
) -> DeleteServiceTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteServiceTemplateOutputTypeDef](./type_defs.md#deleteservicetemplateoutputtypedef) 


```python
# delete_service_template method usage example with argument unpacking

kwargs: DeleteServiceTemplateInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_service_template(**kwargs)
```

1. See [:material-code-braces: DeleteServiceTemplateInputRequestTypeDef](./type_defs.md#deleteservicetemplateinputrequesttypedef) 

### delete\_service\_template\_version

If no other minor versions of a service template exist, delete a major version
of the service template if it's not the `Recommended` version.

Type annotations and code completion for `#!python session.create_client("proton").delete_service_template_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template_version)

```python
# delete_service_template_version method definition

await def delete_service_template_version(
    self,
    *,
    majorVersion: str,
    minorVersion: str,
    templateName: str,
) -> DeleteServiceTemplateVersionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteServiceTemplateVersionOutputTypeDef](./type_defs.md#deleteservicetemplateversionoutputtypedef) 


```python
# delete_service_template_version method usage example with argument unpacking

kwargs: DeleteServiceTemplateVersionInputRequestTypeDef = {  # (1)
    "majorVersion": ...,
    "minorVersion": ...,
    "templateName": ...,
}

parent.delete_service_template_version(**kwargs)
```

1. See [:material-code-braces: DeleteServiceTemplateVersionInputRequestTypeDef](./type_defs.md#deleteservicetemplateversioninputrequesttypedef) 

### delete\_template\_sync\_config

Delete a template sync configuration.

Type annotations and code completion for `#!python session.create_client("proton").delete_template_sync_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_template_sync_config)

```python
# delete_template_sync_config method definition

await def delete_template_sync_config(
    self,
    *,
    templateName: str,
    templateType: TemplateTypeType,  # (1)
) -> DeleteTemplateSyncConfigOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
2. See [:material-code-braces: DeleteTemplateSyncConfigOutputTypeDef](./type_defs.md#deletetemplatesyncconfigoutputtypedef) 


```python
# delete_template_sync_config method usage example with argument unpacking

kwargs: DeleteTemplateSyncConfigInputRequestTypeDef = {  # (1)
    "templateName": ...,
    "templateType": ...,
}

parent.delete_template_sync_config(**kwargs)
```

1. See [:material-code-braces: DeleteTemplateSyncConfigInputRequestTypeDef](./type_defs.md#deletetemplatesyncconfiginputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("proton").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.generate_presigned_url)

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


### get\_account\_settings

Get detail data for Proton account-wide settings.

Type annotations and code completion for `#!python session.create_client("proton").get_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_account_settings)

```python
# get_account_settings method definition

await def get_account_settings(
    self,
) -> GetAccountSettingsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountSettingsOutputTypeDef](./type_defs.md#getaccountsettingsoutputtypedef) 

### get\_component

Get detailed data for a component.

Type annotations and code completion for `#!python session.create_client("proton").get_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_component)

```python
# get_component method definition

await def get_component(
    self,
    *,
    name: str,
) -> GetComponentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetComponentOutputTypeDef](./type_defs.md#getcomponentoutputtypedef) 


```python
# get_component method usage example with argument unpacking

kwargs: GetComponentInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.get_component(**kwargs)
```

1. See [:material-code-braces: GetComponentInputRequestTypeDef](./type_defs.md#getcomponentinputrequesttypedef) 

### get\_deployment

Get detailed data for a deployment.

Type annotations and code completion for `#!python session.create_client("proton").get_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_deployment)

```python
# get_deployment method definition

await def get_deployment(
    self,
    *,
    id: str,
    componentName: str = ...,
    environmentName: str = ...,
    serviceInstanceName: str = ...,
    serviceName: str = ...,
) -> GetDeploymentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeploymentOutputTypeDef](./type_defs.md#getdeploymentoutputtypedef) 


```python
# get_deployment method usage example with argument unpacking

kwargs: GetDeploymentInputRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_deployment(**kwargs)
```

1. See [:material-code-braces: GetDeploymentInputRequestTypeDef](./type_defs.md#getdeploymentinputrequesttypedef) 

### get\_environment

Get detailed data for an environment.

Type annotations and code completion for `#!python session.create_client("proton").get_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment)

```python
# get_environment method definition

await def get_environment(
    self,
    *,
    name: str,
) -> GetEnvironmentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnvironmentOutputTypeDef](./type_defs.md#getenvironmentoutputtypedef) 


```python
# get_environment method usage example with argument unpacking

kwargs: GetEnvironmentInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.get_environment(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentInputRequestTypeDef](./type_defs.md#getenvironmentinputrequesttypedef) 

### get\_environment\_account\_connection

In an environment account, get the detailed data for an environment account
connection.

Type annotations and code completion for `#!python session.create_client("proton").get_environment_account_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_account_connection)

```python
# get_environment_account_connection method definition

await def get_environment_account_connection(
    self,
    *,
    id: str,
) -> GetEnvironmentAccountConnectionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#getenvironmentaccountconnectionoutputtypedef) 


```python
# get_environment_account_connection method usage example with argument unpacking

kwargs: GetEnvironmentAccountConnectionInputRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_environment_account_connection(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#getenvironmentaccountconnectioninputrequesttypedef) 

### get\_environment\_template

Get detailed data for an environment template.

Type annotations and code completion for `#!python session.create_client("proton").get_environment_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template)

```python
# get_environment_template method definition

await def get_environment_template(
    self,
    *,
    name: str,
) -> GetEnvironmentTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnvironmentTemplateOutputTypeDef](./type_defs.md#getenvironmenttemplateoutputtypedef) 


```python
# get_environment_template method usage example with argument unpacking

kwargs: GetEnvironmentTemplateInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.get_environment_template(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentTemplateInputRequestTypeDef](./type_defs.md#getenvironmenttemplateinputrequesttypedef) 

### get\_environment\_template\_version

Get detailed data for a major or minor version of an environment template.

Type annotations and code completion for `#!python session.create_client("proton").get_environment_template_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template_version)

```python
# get_environment_template_version method definition

await def get_environment_template_version(
    self,
    *,
    majorVersion: str,
    minorVersion: str,
    templateName: str,
) -> GetEnvironmentTemplateVersionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnvironmentTemplateVersionOutputTypeDef](./type_defs.md#getenvironmenttemplateversionoutputtypedef) 


```python
# get_environment_template_version method usage example with argument unpacking

kwargs: GetEnvironmentTemplateVersionInputRequestTypeDef = {  # (1)
    "majorVersion": ...,
    "minorVersion": ...,
    "templateName": ...,
}

parent.get_environment_template_version(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentTemplateVersionInputRequestTypeDef](./type_defs.md#getenvironmenttemplateversioninputrequesttypedef) 

### get\_repository

Get detail data for a linked repository.

Type annotations and code completion for `#!python session.create_client("proton").get_repository` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository)

```python
# get_repository method definition

await def get_repository(
    self,
    *,
    name: str,
    provider: RepositoryProviderType,  # (1)
) -> GetRepositoryOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-braces: GetRepositoryOutputTypeDef](./type_defs.md#getrepositoryoutputtypedef) 


```python
# get_repository method usage example with argument unpacking

kwargs: GetRepositoryInputRequestTypeDef = {  # (1)
    "name": ...,
    "provider": ...,
}

parent.get_repository(**kwargs)
```

1. See [:material-code-braces: GetRepositoryInputRequestTypeDef](./type_defs.md#getrepositoryinputrequesttypedef) 

### get\_repository\_sync\_status

Get the sync status of a repository used for Proton template sync.

Type annotations and code completion for `#!python session.create_client("proton").get_repository_sync_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository_sync_status)

```python
# get_repository_sync_status method definition

await def get_repository_sync_status(
    self,
    *,
    branch: str,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    syncType: SyncTypeType,  # (2)
) -> GetRepositorySyncStatusOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-brackets: SyncTypeType](./literals.md#synctypetype) 
3. See [:material-code-braces: GetRepositorySyncStatusOutputTypeDef](./type_defs.md#getrepositorysyncstatusoutputtypedef) 


```python
# get_repository_sync_status method usage example with argument unpacking

kwargs: GetRepositorySyncStatusInputRequestTypeDef = {  # (1)
    "branch": ...,
    "repositoryName": ...,
    "repositoryProvider": ...,
    "syncType": ...,
}

parent.get_repository_sync_status(**kwargs)
```

1. See [:material-code-braces: GetRepositorySyncStatusInputRequestTypeDef](./type_defs.md#getrepositorysyncstatusinputrequesttypedef) 

### get\_resources\_summary

Get counts of Proton resources.

Type annotations and code completion for `#!python session.create_client("proton").get_resources_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_resources_summary)

```python
# get_resources_summary method definition

await def get_resources_summary(
    self,
) -> GetResourcesSummaryOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourcesSummaryOutputTypeDef](./type_defs.md#getresourcessummaryoutputtypedef) 

### get\_service

Get detailed data for a service.

Type annotations and code completion for `#!python session.create_client("proton").get_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service)

```python
# get_service method definition

await def get_service(
    self,
    *,
    name: str,
) -> GetServiceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceOutputTypeDef](./type_defs.md#getserviceoutputtypedef) 


```python
# get_service method usage example with argument unpacking

kwargs: GetServiceInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.get_service(**kwargs)
```

1. See [:material-code-braces: GetServiceInputRequestTypeDef](./type_defs.md#getserviceinputrequesttypedef) 

### get\_service\_instance

Get detailed data for a service instance.

Type annotations and code completion for `#!python session.create_client("proton").get_service_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance)

```python
# get_service_instance method definition

await def get_service_instance(
    self,
    *,
    name: str,
    serviceName: str,
) -> GetServiceInstanceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceInstanceOutputTypeDef](./type_defs.md#getserviceinstanceoutputtypedef) 


```python
# get_service_instance method usage example with argument unpacking

kwargs: GetServiceInstanceInputRequestTypeDef = {  # (1)
    "name": ...,
    "serviceName": ...,
}

parent.get_service_instance(**kwargs)
```

1. See [:material-code-braces: GetServiceInstanceInputRequestTypeDef](./type_defs.md#getserviceinstanceinputrequesttypedef) 

### get\_service\_instance\_sync\_status

Get the status of the synced service instance.

Type annotations and code completion for `#!python session.create_client("proton").get_service_instance_sync_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance_sync_status)

```python
# get_service_instance_sync_status method definition

await def get_service_instance_sync_status(
    self,
    *,
    serviceInstanceName: str,
    serviceName: str,
) -> GetServiceInstanceSyncStatusOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceInstanceSyncStatusOutputTypeDef](./type_defs.md#getserviceinstancesyncstatusoutputtypedef) 


```python
# get_service_instance_sync_status method usage example with argument unpacking

kwargs: GetServiceInstanceSyncStatusInputRequestTypeDef = {  # (1)
    "serviceInstanceName": ...,
    "serviceName": ...,
}

parent.get_service_instance_sync_status(**kwargs)
```

1. See [:material-code-braces: GetServiceInstanceSyncStatusInputRequestTypeDef](./type_defs.md#getserviceinstancesyncstatusinputrequesttypedef) 

### get\_service\_sync\_blocker\_summary

Get detailed data for the service sync blocker summary.

Type annotations and code completion for `#!python session.create_client("proton").get_service_sync_blocker_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_blocker_summary)

```python
# get_service_sync_blocker_summary method definition

await def get_service_sync_blocker_summary(
    self,
    *,
    serviceName: str,
    serviceInstanceName: str = ...,
) -> GetServiceSyncBlockerSummaryOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceSyncBlockerSummaryOutputTypeDef](./type_defs.md#getservicesyncblockersummaryoutputtypedef) 


```python
# get_service_sync_blocker_summary method usage example with argument unpacking

kwargs: GetServiceSyncBlockerSummaryInputRequestTypeDef = {  # (1)
    "serviceName": ...,
}

parent.get_service_sync_blocker_summary(**kwargs)
```

1. See [:material-code-braces: GetServiceSyncBlockerSummaryInputRequestTypeDef](./type_defs.md#getservicesyncblockersummaryinputrequesttypedef) 

### get\_service\_sync\_config

Get detailed information for the service sync configuration.

Type annotations and code completion for `#!python session.create_client("proton").get_service_sync_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_config)

```python
# get_service_sync_config method definition

await def get_service_sync_config(
    self,
    *,
    serviceName: str,
) -> GetServiceSyncConfigOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceSyncConfigOutputTypeDef](./type_defs.md#getservicesyncconfigoutputtypedef) 


```python
# get_service_sync_config method usage example with argument unpacking

kwargs: GetServiceSyncConfigInputRequestTypeDef = {  # (1)
    "serviceName": ...,
}

parent.get_service_sync_config(**kwargs)
```

1. See [:material-code-braces: GetServiceSyncConfigInputRequestTypeDef](./type_defs.md#getservicesyncconfiginputrequesttypedef) 

### get\_service\_template

Get detailed data for a service template.

Type annotations and code completion for `#!python session.create_client("proton").get_service_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template)

```python
# get_service_template method definition

await def get_service_template(
    self,
    *,
    name: str,
) -> GetServiceTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceTemplateOutputTypeDef](./type_defs.md#getservicetemplateoutputtypedef) 


```python
# get_service_template method usage example with argument unpacking

kwargs: GetServiceTemplateInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.get_service_template(**kwargs)
```

1. See [:material-code-braces: GetServiceTemplateInputRequestTypeDef](./type_defs.md#getservicetemplateinputrequesttypedef) 

### get\_service\_template\_version

Get detailed data for a major or minor version of a service template.

Type annotations and code completion for `#!python session.create_client("proton").get_service_template_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template_version)

```python
# get_service_template_version method definition

await def get_service_template_version(
    self,
    *,
    majorVersion: str,
    minorVersion: str,
    templateName: str,
) -> GetServiceTemplateVersionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceTemplateVersionOutputTypeDef](./type_defs.md#getservicetemplateversionoutputtypedef) 


```python
# get_service_template_version method usage example with argument unpacking

kwargs: GetServiceTemplateVersionInputRequestTypeDef = {  # (1)
    "majorVersion": ...,
    "minorVersion": ...,
    "templateName": ...,
}

parent.get_service_template_version(**kwargs)
```

1. See [:material-code-braces: GetServiceTemplateVersionInputRequestTypeDef](./type_defs.md#getservicetemplateversioninputrequesttypedef) 

### get\_template\_sync\_config

Get detail data for a template sync configuration.

Type annotations and code completion for `#!python session.create_client("proton").get_template_sync_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_config)

```python
# get_template_sync_config method definition

await def get_template_sync_config(
    self,
    *,
    templateName: str,
    templateType: TemplateTypeType,  # (1)
) -> GetTemplateSyncConfigOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
2. See [:material-code-braces: GetTemplateSyncConfigOutputTypeDef](./type_defs.md#gettemplatesyncconfigoutputtypedef) 


```python
# get_template_sync_config method usage example with argument unpacking

kwargs: GetTemplateSyncConfigInputRequestTypeDef = {  # (1)
    "templateName": ...,
    "templateType": ...,
}

parent.get_template_sync_config(**kwargs)
```

1. See [:material-code-braces: GetTemplateSyncConfigInputRequestTypeDef](./type_defs.md#gettemplatesyncconfiginputrequesttypedef) 

### get\_template\_sync\_status

Get the status of a template sync.

Type annotations and code completion for `#!python session.create_client("proton").get_template_sync_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_status)

```python
# get_template_sync_status method definition

await def get_template_sync_status(
    self,
    *,
    templateName: str,
    templateType: TemplateTypeType,  # (1)
    templateVersion: str,
) -> GetTemplateSyncStatusOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
2. See [:material-code-braces: GetTemplateSyncStatusOutputTypeDef](./type_defs.md#gettemplatesyncstatusoutputtypedef) 


```python
# get_template_sync_status method usage example with argument unpacking

kwargs: GetTemplateSyncStatusInputRequestTypeDef = {  # (1)
    "templateName": ...,
    "templateType": ...,
    "templateVersion": ...,
}

parent.get_template_sync_status(**kwargs)
```

1. See [:material-code-braces: GetTemplateSyncStatusInputRequestTypeDef](./type_defs.md#gettemplatesyncstatusinputrequesttypedef) 

### list\_component\_outputs

Get a list of component Infrastructure as Code (IaC) outputs.

Type annotations and code completion for `#!python session.create_client("proton").list_component_outputs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_outputs)

```python
# list_component_outputs method definition

await def list_component_outputs(
    self,
    *,
    componentName: str,
    deploymentId: str = ...,
    nextToken: str = ...,
) -> ListComponentOutputsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListComponentOutputsOutputTypeDef](./type_defs.md#listcomponentoutputsoutputtypedef) 


```python
# list_component_outputs method usage example with argument unpacking

kwargs: ListComponentOutputsInputRequestTypeDef = {  # (1)
    "componentName": ...,
}

parent.list_component_outputs(**kwargs)
```

1. See [:material-code-braces: ListComponentOutputsInputRequestTypeDef](./type_defs.md#listcomponentoutputsinputrequesttypedef) 

### list\_component\_provisioned\_resources

List provisioned resources for a component with details.

Type annotations and code completion for `#!python session.create_client("proton").list_component_provisioned_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_provisioned_resources)

```python
# list_component_provisioned_resources method definition

await def list_component_provisioned_resources(
    self,
    *,
    componentName: str,
    nextToken: str = ...,
) -> ListComponentProvisionedResourcesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListComponentProvisionedResourcesOutputTypeDef](./type_defs.md#listcomponentprovisionedresourcesoutputtypedef) 


```python
# list_component_provisioned_resources method usage example with argument unpacking

kwargs: ListComponentProvisionedResourcesInputRequestTypeDef = {  # (1)
    "componentName": ...,
}

parent.list_component_provisioned_resources(**kwargs)
```

1. See [:material-code-braces: ListComponentProvisionedResourcesInputRequestTypeDef](./type_defs.md#listcomponentprovisionedresourcesinputrequesttypedef) 

### list\_components

List components with summary data.

Type annotations and code completion for `#!python session.create_client("proton").list_components` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_components)

```python
# list_components method definition

await def list_components(
    self,
    *,
    environmentName: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    serviceInstanceName: str = ...,
    serviceName: str = ...,
) -> ListComponentsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListComponentsOutputTypeDef](./type_defs.md#listcomponentsoutputtypedef) 


```python
# list_components method usage example with argument unpacking

kwargs: ListComponentsInputRequestTypeDef = {  # (1)
    "environmentName": ...,
}

parent.list_components(**kwargs)
```

1. See [:material-code-braces: ListComponentsInputRequestTypeDef](./type_defs.md#listcomponentsinputrequesttypedef) 

### list\_deployments

List deployments.

Type annotations and code completion for `#!python session.create_client("proton").list_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_deployments)

```python
# list_deployments method definition

await def list_deployments(
    self,
    *,
    componentName: str = ...,
    environmentName: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    serviceInstanceName: str = ...,
    serviceName: str = ...,
) -> ListDeploymentsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDeploymentsOutputTypeDef](./type_defs.md#listdeploymentsoutputtypedef) 


```python
# list_deployments method usage example with argument unpacking

kwargs: ListDeploymentsInputRequestTypeDef = {  # (1)
    "componentName": ...,
}

parent.list_deployments(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsInputRequestTypeDef](./type_defs.md#listdeploymentsinputrequesttypedef) 

### list\_environment\_account\_connections

View a list of environment account connections.

Type annotations and code completion for `#!python session.create_client("proton").list_environment_account_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)

```python
# list_environment_account_connections method definition

await def list_environment_account_connections(
    self,
    *,
    requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,  # (1)
    environmentName: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...,  # (2)
) -> ListEnvironmentAccountConnectionsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: EnvironmentAccountConnectionRequesterAccountTypeType](./literals.md#environmentaccountconnectionrequesteraccounttypetype) 
2. See [:material-code-brackets: EnvironmentAccountConnectionStatusType](./literals.md#environmentaccountconnectionstatustype) 
3. See [:material-code-braces: ListEnvironmentAccountConnectionsOutputTypeDef](./type_defs.md#listenvironmentaccountconnectionsoutputtypedef) 


```python
# list_environment_account_connections method usage example with argument unpacking

kwargs: ListEnvironmentAccountConnectionsInputRequestTypeDef = {  # (1)
    "requestedBy": ...,
}

parent.list_environment_account_connections(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentAccountConnectionsInputRequestTypeDef](./type_defs.md#listenvironmentaccountconnectionsinputrequesttypedef) 

### list\_environment\_outputs

List the infrastructure as code outputs for your environment.

Type annotations and code completion for `#!python session.create_client("proton").list_environment_outputs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_outputs)

```python
# list_environment_outputs method definition

await def list_environment_outputs(
    self,
    *,
    environmentName: str,
    deploymentId: str = ...,
    nextToken: str = ...,
) -> ListEnvironmentOutputsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnvironmentOutputsOutputTypeDef](./type_defs.md#listenvironmentoutputsoutputtypedef) 


```python
# list_environment_outputs method usage example with argument unpacking

kwargs: ListEnvironmentOutputsInputRequestTypeDef = {  # (1)
    "environmentName": ...,
}

parent.list_environment_outputs(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentOutputsInputRequestTypeDef](./type_defs.md#listenvironmentoutputsinputrequesttypedef) 

### list\_environment\_provisioned\_resources

List the provisioned resources for your environment.

Type annotations and code completion for `#!python session.create_client("proton").list_environment_provisioned_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_provisioned_resources)

```python
# list_environment_provisioned_resources method definition

await def list_environment_provisioned_resources(
    self,
    *,
    environmentName: str,
    nextToken: str = ...,
) -> ListEnvironmentProvisionedResourcesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnvironmentProvisionedResourcesOutputTypeDef](./type_defs.md#listenvironmentprovisionedresourcesoutputtypedef) 


```python
# list_environment_provisioned_resources method usage example with argument unpacking

kwargs: ListEnvironmentProvisionedResourcesInputRequestTypeDef = {  # (1)
    "environmentName": ...,
}

parent.list_environment_provisioned_resources(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentProvisionedResourcesInputRequestTypeDef](./type_defs.md#listenvironmentprovisionedresourcesinputrequesttypedef) 

### list\_environment\_template\_versions

List major or minor versions of an environment template with detail data.

Type annotations and code completion for `#!python session.create_client("proton").list_environment_template_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_template_versions)

```python
# list_environment_template_versions method definition

await def list_environment_template_versions(
    self,
    *,
    templateName: str,
    majorVersion: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListEnvironmentTemplateVersionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnvironmentTemplateVersionsOutputTypeDef](./type_defs.md#listenvironmenttemplateversionsoutputtypedef) 


```python
# list_environment_template_versions method usage example with argument unpacking

kwargs: ListEnvironmentTemplateVersionsInputRequestTypeDef = {  # (1)
    "templateName": ...,
}

parent.list_environment_template_versions(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentTemplateVersionsInputRequestTypeDef](./type_defs.md#listenvironmenttemplateversionsinputrequesttypedef) 

### list\_environment\_templates

List environment templates.

Type annotations and code completion for `#!python session.create_client("proton").list_environment_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_templates)

```python
# list_environment_templates method definition

await def list_environment_templates(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListEnvironmentTemplatesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnvironmentTemplatesOutputTypeDef](./type_defs.md#listenvironmenttemplatesoutputtypedef) 


```python
# list_environment_templates method usage example with argument unpacking

kwargs: ListEnvironmentTemplatesInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_environment_templates(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentTemplatesInputRequestTypeDef](./type_defs.md#listenvironmenttemplatesinputrequesttypedef) 

### list\_environments

List environments with detail data summaries.

Type annotations and code completion for `#!python session.create_client("proton").list_environments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environments)

```python
# list_environments method definition

await def list_environments(
    self,
    *,
    environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListEnvironmentsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EnvironmentTemplateFilterTypeDef](./type_defs.md#environmenttemplatefiltertypedef) 
2. See [:material-code-braces: ListEnvironmentsOutputTypeDef](./type_defs.md#listenvironmentsoutputtypedef) 


```python
# list_environments method usage example with argument unpacking

kwargs: ListEnvironmentsInputRequestTypeDef = {  # (1)
    "environmentTemplates": ...,
}

parent.list_environments(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsInputRequestTypeDef](./type_defs.md#listenvironmentsinputrequesttypedef) 

### list\_repositories

List linked repositories with detail data.

Type annotations and code completion for `#!python session.create_client("proton").list_repositories` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repositories)

```python
# list_repositories method definition

await def list_repositories(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListRepositoriesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRepositoriesOutputTypeDef](./type_defs.md#listrepositoriesoutputtypedef) 


```python
# list_repositories method usage example with argument unpacking

kwargs: ListRepositoriesInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_repositories(**kwargs)
```

1. See [:material-code-braces: ListRepositoriesInputRequestTypeDef](./type_defs.md#listrepositoriesinputrequesttypedef) 

### list\_repository\_sync\_definitions

List repository sync definitions with detail data.

Type annotations and code completion for `#!python session.create_client("proton").list_repository_sync_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)

```python
# list_repository_sync_definitions method definition

await def list_repository_sync_definitions(
    self,
    *,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    syncType: SyncTypeType,  # (2)
    nextToken: str = ...,
) -> ListRepositorySyncDefinitionsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-brackets: SyncTypeType](./literals.md#synctypetype) 
3. See [:material-code-braces: ListRepositorySyncDefinitionsOutputTypeDef](./type_defs.md#listrepositorysyncdefinitionsoutputtypedef) 


```python
# list_repository_sync_definitions method usage example with argument unpacking

kwargs: ListRepositorySyncDefinitionsInputRequestTypeDef = {  # (1)
    "repositoryName": ...,
    "repositoryProvider": ...,
    "syncType": ...,
}

parent.list_repository_sync_definitions(**kwargs)
```

1. See [:material-code-braces: ListRepositorySyncDefinitionsInputRequestTypeDef](./type_defs.md#listrepositorysyncdefinitionsinputrequesttypedef) 

### list\_service\_instance\_outputs

Get a list service of instance Infrastructure as Code (IaC) outputs.

Type annotations and code completion for `#!python session.create_client("proton").list_service_instance_outputs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)

```python
# list_service_instance_outputs method definition

await def list_service_instance_outputs(
    self,
    *,
    serviceInstanceName: str,
    serviceName: str,
    deploymentId: str = ...,
    nextToken: str = ...,
) -> ListServiceInstanceOutputsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServiceInstanceOutputsOutputTypeDef](./type_defs.md#listserviceinstanceoutputsoutputtypedef) 


```python
# list_service_instance_outputs method usage example with argument unpacking

kwargs: ListServiceInstanceOutputsInputRequestTypeDef = {  # (1)
    "serviceInstanceName": ...,
    "serviceName": ...,
}

parent.list_service_instance_outputs(**kwargs)
```

1. See [:material-code-braces: ListServiceInstanceOutputsInputRequestTypeDef](./type_defs.md#listserviceinstanceoutputsinputrequesttypedef) 

### list\_service\_instance\_provisioned\_resources

List provisioned resources for a service instance with details.

Type annotations and code completion for `#!python session.create_client("proton").list_service_instance_provisioned_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_provisioned_resources)

```python
# list_service_instance_provisioned_resources method definition

await def list_service_instance_provisioned_resources(
    self,
    *,
    serviceInstanceName: str,
    serviceName: str,
    nextToken: str = ...,
) -> ListServiceInstanceProvisionedResourcesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServiceInstanceProvisionedResourcesOutputTypeDef](./type_defs.md#listserviceinstanceprovisionedresourcesoutputtypedef) 


```python
# list_service_instance_provisioned_resources method usage example with argument unpacking

kwargs: ListServiceInstanceProvisionedResourcesInputRequestTypeDef = {  # (1)
    "serviceInstanceName": ...,
    "serviceName": ...,
}

parent.list_service_instance_provisioned_resources(**kwargs)
```

1. See [:material-code-braces: ListServiceInstanceProvisionedResourcesInputRequestTypeDef](./type_defs.md#listserviceinstanceprovisionedresourcesinputrequesttypedef) 

### list\_service\_instances

List service instances with summary data.

Type annotations and code completion for `#!python session.create_client("proton").list_service_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)

```python
# list_service_instances method definition

await def list_service_instances(
    self,
    *,
    filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    serviceName: str = ...,
    sortBy: ListServiceInstancesSortByType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
) -> ListServiceInstancesOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ListServiceInstancesFilterTypeDef](./type_defs.md#listserviceinstancesfiltertypedef) 
2. See [:material-code-brackets: ListServiceInstancesSortByType](./literals.md#listserviceinstancessortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListServiceInstancesOutputTypeDef](./type_defs.md#listserviceinstancesoutputtypedef) 


```python
# list_service_instances method usage example with argument unpacking

kwargs: ListServiceInstancesInputRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_service_instances(**kwargs)
```

1. See [:material-code-braces: ListServiceInstancesInputRequestTypeDef](./type_defs.md#listserviceinstancesinputrequesttypedef) 

### list\_service\_pipeline\_outputs

Get a list of service pipeline Infrastructure as Code (IaC) outputs.

Type annotations and code completion for `#!python session.create_client("proton").list_service_pipeline_outputs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_outputs)

```python
# list_service_pipeline_outputs method definition

await def list_service_pipeline_outputs(
    self,
    *,
    serviceName: str,
    deploymentId: str = ...,
    nextToken: str = ...,
) -> ListServicePipelineOutputsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServicePipelineOutputsOutputTypeDef](./type_defs.md#listservicepipelineoutputsoutputtypedef) 


```python
# list_service_pipeline_outputs method usage example with argument unpacking

kwargs: ListServicePipelineOutputsInputRequestTypeDef = {  # (1)
    "serviceName": ...,
}

parent.list_service_pipeline_outputs(**kwargs)
```

1. See [:material-code-braces: ListServicePipelineOutputsInputRequestTypeDef](./type_defs.md#listservicepipelineoutputsinputrequesttypedef) 

### list\_service\_pipeline\_provisioned\_resources

List provisioned resources for a service and pipeline with details.

Type annotations and code completion for `#!python session.create_client("proton").list_service_pipeline_provisioned_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_provisioned_resources)

```python
# list_service_pipeline_provisioned_resources method definition

await def list_service_pipeline_provisioned_resources(
    self,
    *,
    serviceName: str,
    nextToken: str = ...,
) -> ListServicePipelineProvisionedResourcesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServicePipelineProvisionedResourcesOutputTypeDef](./type_defs.md#listservicepipelineprovisionedresourcesoutputtypedef) 


```python
# list_service_pipeline_provisioned_resources method usage example with argument unpacking

kwargs: ListServicePipelineProvisionedResourcesInputRequestTypeDef = {  # (1)
    "serviceName": ...,
}

parent.list_service_pipeline_provisioned_resources(**kwargs)
```

1. See [:material-code-braces: ListServicePipelineProvisionedResourcesInputRequestTypeDef](./type_defs.md#listservicepipelineprovisionedresourcesinputrequesttypedef) 

### list\_service\_template\_versions

List major or minor versions of a service template with detail data.

Type annotations and code completion for `#!python session.create_client("proton").list_service_template_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_template_versions)

```python
# list_service_template_versions method definition

await def list_service_template_versions(
    self,
    *,
    templateName: str,
    majorVersion: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListServiceTemplateVersionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServiceTemplateVersionsOutputTypeDef](./type_defs.md#listservicetemplateversionsoutputtypedef) 


```python
# list_service_template_versions method usage example with argument unpacking

kwargs: ListServiceTemplateVersionsInputRequestTypeDef = {  # (1)
    "templateName": ...,
}

parent.list_service_template_versions(**kwargs)
```

1. See [:material-code-braces: ListServiceTemplateVersionsInputRequestTypeDef](./type_defs.md#listservicetemplateversionsinputrequesttypedef) 

### list\_service\_templates

List service templates with detail data.

Type annotations and code completion for `#!python session.create_client("proton").list_service_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_templates)

```python
# list_service_templates method definition

await def list_service_templates(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListServiceTemplatesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServiceTemplatesOutputTypeDef](./type_defs.md#listservicetemplatesoutputtypedef) 


```python
# list_service_templates method usage example with argument unpacking

kwargs: ListServiceTemplatesInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_service_templates(**kwargs)
```

1. See [:material-code-braces: ListServiceTemplatesInputRequestTypeDef](./type_defs.md#listservicetemplatesinputrequesttypedef) 

### list\_services

List services with summaries of detail data.

Type annotations and code completion for `#!python session.create_client("proton").list_services` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_services)

```python
# list_services method definition

await def list_services(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListServicesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServicesOutputTypeDef](./type_defs.md#listservicesoutputtypedef) 


```python
# list_services method usage example with argument unpacking

kwargs: ListServicesInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_services(**kwargs)
```

1. See [:material-code-braces: ListServicesInputRequestTypeDef](./type_defs.md#listservicesinputrequesttypedef) 

### list\_tags\_for\_resource

List tags for a resource.

Type annotations and code completion for `#!python session.create_client("proton").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### notify\_resource\_deployment\_status\_change

Notify Proton of status changes to a provisioned resource when you use self-
managed provisioning.

Type annotations and code completion for `#!python session.create_client("proton").notify_resource_deployment_status_change` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.notify_resource_deployment_status_change)

```python
# notify_resource_deployment_status_change method definition

await def notify_resource_deployment_status_change(
    self,
    *,
    resourceArn: str,
    deploymentId: str = ...,
    outputs: Sequence[OutputTypeDef] = ...,  # (1)
    status: ResourceDeploymentStatusType = ...,  # (2)
    statusMessage: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
2. See [:material-code-brackets: ResourceDeploymentStatusType](./literals.md#resourcedeploymentstatustype) 


```python
# notify_resource_deployment_status_change method usage example with argument unpacking

kwargs: NotifyResourceDeploymentStatusChangeInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.notify_resource_deployment_status_change(**kwargs)
```

1. See [:material-code-braces: NotifyResourceDeploymentStatusChangeInputRequestTypeDef](./type_defs.md#notifyresourcedeploymentstatuschangeinputrequesttypedef) 

### reject\_environment\_account\_connection

In a management account, reject an environment account connection from another
environment account.

Type annotations and code completion for `#!python session.create_client("proton").reject_environment_account_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.reject_environment_account_connection)

```python
# reject_environment_account_connection method definition

await def reject_environment_account_connection(
    self,
    *,
    id: str,
) -> RejectEnvironmentAccountConnectionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RejectEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#rejectenvironmentaccountconnectionoutputtypedef) 


```python
# reject_environment_account_connection method usage example with argument unpacking

kwargs: RejectEnvironmentAccountConnectionInputRequestTypeDef = {  # (1)
    "id": ...,
}

parent.reject_environment_account_connection(**kwargs)
```

1. See [:material-code-braces: RejectEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#rejectenvironmentaccountconnectioninputrequesttypedef) 

### tag\_resource

Tag a resource.

Type annotations and code completion for `#!python session.create_client("proton").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Remove a customer tag from a resource.

Type annotations and code completion for `#!python session.create_client("proton").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.untag_resource)

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

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_account\_settings

Update Proton settings that are used for multiple services in the Amazon Web
Services account.

Type annotations and code completion for `#!python session.create_client("proton").update_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_account_settings)

```python
# update_account_settings method definition

await def update_account_settings(
    self,
    *,
    deletePipelineProvisioningRepository: bool = ...,
    pipelineCodebuildRoleArn: str = ...,
    pipelineProvisioningRepository: RepositoryBranchInputTypeDef = ...,  # (1)
    pipelineServiceRoleArn: str = ...,
) -> UpdateAccountSettingsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RepositoryBranchInputTypeDef](./type_defs.md#repositorybranchinputtypedef) 
2. See [:material-code-braces: UpdateAccountSettingsOutputTypeDef](./type_defs.md#updateaccountsettingsoutputtypedef) 


```python
# update_account_settings method usage example with argument unpacking

kwargs: UpdateAccountSettingsInputRequestTypeDef = {  # (1)
    "deletePipelineProvisioningRepository": ...,
}

parent.update_account_settings(**kwargs)
```

1. See [:material-code-braces: UpdateAccountSettingsInputRequestTypeDef](./type_defs.md#updateaccountsettingsinputrequesttypedef) 

### update\_component

Update a component.

Type annotations and code completion for `#!python session.create_client("proton").update_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_component)

```python
# update_component method definition

await def update_component(
    self,
    *,
    deploymentType: ComponentDeploymentUpdateTypeType,  # (1)
    name: str,
    clientToken: str = ...,
    description: str = ...,
    serviceInstanceName: str = ...,
    serviceName: str = ...,
    serviceSpec: str = ...,
    templateFile: str = ...,
) -> UpdateComponentOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ComponentDeploymentUpdateTypeType](./literals.md#componentdeploymentupdatetypetype) 
2. See [:material-code-braces: UpdateComponentOutputTypeDef](./type_defs.md#updatecomponentoutputtypedef) 


```python
# update_component method usage example with argument unpacking

kwargs: UpdateComponentInputRequestTypeDef = {  # (1)
    "deploymentType": ...,
    "name": ...,
}

parent.update_component(**kwargs)
```

1. See [:material-code-braces: UpdateComponentInputRequestTypeDef](./type_defs.md#updatecomponentinputrequesttypedef) 

### update\_environment

Update an environment.

Type annotations and code completion for `#!python session.create_client("proton").update_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment)

```python
# update_environment method definition

await def update_environment(
    self,
    *,
    deploymentType: DeploymentUpdateTypeType,  # (1)
    name: str,
    codebuildRoleArn: str = ...,
    componentRoleArn: str = ...,
    description: str = ...,
    environmentAccountConnectionId: str = ...,
    protonServiceRoleArn: str = ...,
    provisioningRepository: RepositoryBranchInputTypeDef = ...,  # (2)
    spec: str = ...,
    templateMajorVersion: str = ...,
    templateMinorVersion: str = ...,
) -> UpdateEnvironmentOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: DeploymentUpdateTypeType](./literals.md#deploymentupdatetypetype) 
2. See [:material-code-braces: RepositoryBranchInputTypeDef](./type_defs.md#repositorybranchinputtypedef) 
3. See [:material-code-braces: UpdateEnvironmentOutputTypeDef](./type_defs.md#updateenvironmentoutputtypedef) 


```python
# update_environment method usage example with argument unpacking

kwargs: UpdateEnvironmentInputRequestTypeDef = {  # (1)
    "deploymentType": ...,
    "name": ...,
}

parent.update_environment(**kwargs)
```

1. See [:material-code-braces: UpdateEnvironmentInputRequestTypeDef](./type_defs.md#updateenvironmentinputrequesttypedef) 

### update\_environment\_account\_connection

In an environment account, update an environment account connection to use a new
IAM role.

Type annotations and code completion for `#!python session.create_client("proton").update_environment_account_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_account_connection)

```python
# update_environment_account_connection method definition

await def update_environment_account_connection(
    self,
    *,
    id: str,
    codebuildRoleArn: str = ...,
    componentRoleArn: str = ...,
    roleArn: str = ...,
) -> UpdateEnvironmentAccountConnectionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#updateenvironmentaccountconnectionoutputtypedef) 


```python
# update_environment_account_connection method usage example with argument unpacking

kwargs: UpdateEnvironmentAccountConnectionInputRequestTypeDef = {  # (1)
    "id": ...,
}

parent.update_environment_account_connection(**kwargs)
```

1. See [:material-code-braces: UpdateEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#updateenvironmentaccountconnectioninputrequesttypedef) 

### update\_environment\_template

Update an environment template.

Type annotations and code completion for `#!python session.create_client("proton").update_environment_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template)

```python
# update_environment_template method definition

await def update_environment_template(
    self,
    *,
    name: str,
    description: str = ...,
    displayName: str = ...,
) -> UpdateEnvironmentTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateEnvironmentTemplateOutputTypeDef](./type_defs.md#updateenvironmenttemplateoutputtypedef) 


```python
# update_environment_template method usage example with argument unpacking

kwargs: UpdateEnvironmentTemplateInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.update_environment_template(**kwargs)
```

1. See [:material-code-braces: UpdateEnvironmentTemplateInputRequestTypeDef](./type_defs.md#updateenvironmenttemplateinputrequesttypedef) 

### update\_environment\_template\_version

Update a major or minor version of an environment template.

Type annotations and code completion for `#!python session.create_client("proton").update_environment_template_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template_version)

```python
# update_environment_template_version method definition

await def update_environment_template_version(
    self,
    *,
    majorVersion: str,
    minorVersion: str,
    templateName: str,
    description: str = ...,
    status: TemplateVersionStatusType = ...,  # (1)
) -> UpdateEnvironmentTemplateVersionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TemplateVersionStatusType](./literals.md#templateversionstatustype) 
2. See [:material-code-braces: UpdateEnvironmentTemplateVersionOutputTypeDef](./type_defs.md#updateenvironmenttemplateversionoutputtypedef) 


```python
# update_environment_template_version method usage example with argument unpacking

kwargs: UpdateEnvironmentTemplateVersionInputRequestTypeDef = {  # (1)
    "majorVersion": ...,
    "minorVersion": ...,
    "templateName": ...,
}

parent.update_environment_template_version(**kwargs)
```

1. See [:material-code-braces: UpdateEnvironmentTemplateVersionInputRequestTypeDef](./type_defs.md#updateenvironmenttemplateversioninputrequesttypedef) 

### update\_service

Edit a service description or use a spec to add and delete service instances.

Type annotations and code completion for `#!python session.create_client("proton").update_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service)

```python
# update_service method definition

await def update_service(
    self,
    *,
    name: str,
    description: str = ...,
    spec: str = ...,
) -> UpdateServiceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateServiceOutputTypeDef](./type_defs.md#updateserviceoutputtypedef) 


```python
# update_service method usage example with argument unpacking

kwargs: UpdateServiceInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.update_service(**kwargs)
```

1. See [:material-code-braces: UpdateServiceInputRequestTypeDef](./type_defs.md#updateserviceinputrequesttypedef) 

### update\_service\_instance

Update a service instance.

Type annotations and code completion for `#!python session.create_client("proton").update_service_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_instance)

```python
# update_service_instance method definition

await def update_service_instance(
    self,
    *,
    deploymentType: DeploymentUpdateTypeType,  # (1)
    name: str,
    serviceName: str,
    clientToken: str = ...,
    spec: str = ...,
    templateMajorVersion: str = ...,
    templateMinorVersion: str = ...,
) -> UpdateServiceInstanceOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DeploymentUpdateTypeType](./literals.md#deploymentupdatetypetype) 
2. See [:material-code-braces: UpdateServiceInstanceOutputTypeDef](./type_defs.md#updateserviceinstanceoutputtypedef) 


```python
# update_service_instance method usage example with argument unpacking

kwargs: UpdateServiceInstanceInputRequestTypeDef = {  # (1)
    "deploymentType": ...,
    "name": ...,
    "serviceName": ...,
}

parent.update_service_instance(**kwargs)
```

1. See [:material-code-braces: UpdateServiceInstanceInputRequestTypeDef](./type_defs.md#updateserviceinstanceinputrequesttypedef) 

### update\_service\_pipeline

Update the service pipeline.

Type annotations and code completion for `#!python session.create_client("proton").update_service_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_pipeline)

```python
# update_service_pipeline method definition

await def update_service_pipeline(
    self,
    *,
    deploymentType: DeploymentUpdateTypeType,  # (1)
    serviceName: str,
    spec: str,
    templateMajorVersion: str = ...,
    templateMinorVersion: str = ...,
) -> UpdateServicePipelineOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DeploymentUpdateTypeType](./literals.md#deploymentupdatetypetype) 
2. See [:material-code-braces: UpdateServicePipelineOutputTypeDef](./type_defs.md#updateservicepipelineoutputtypedef) 


```python
# update_service_pipeline method usage example with argument unpacking

kwargs: UpdateServicePipelineInputRequestTypeDef = {  # (1)
    "deploymentType": ...,
    "serviceName": ...,
    "spec": ...,
}

parent.update_service_pipeline(**kwargs)
```

1. See [:material-code-braces: UpdateServicePipelineInputRequestTypeDef](./type_defs.md#updateservicepipelineinputrequesttypedef) 

### update\_service\_sync\_blocker

Update the service sync blocker by resolving it.

Type annotations and code completion for `#!python session.create_client("proton").update_service_sync_blocker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_blocker)

```python
# update_service_sync_blocker method definition

await def update_service_sync_blocker(
    self,
    *,
    id: str,
    resolvedReason: str,
) -> UpdateServiceSyncBlockerOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateServiceSyncBlockerOutputTypeDef](./type_defs.md#updateservicesyncblockeroutputtypedef) 


```python
# update_service_sync_blocker method usage example with argument unpacking

kwargs: UpdateServiceSyncBlockerInputRequestTypeDef = {  # (1)
    "id": ...,
    "resolvedReason": ...,
}

parent.update_service_sync_blocker(**kwargs)
```

1. See [:material-code-braces: UpdateServiceSyncBlockerInputRequestTypeDef](./type_defs.md#updateservicesyncblockerinputrequesttypedef) 

### update\_service\_sync\_config

Update the Proton Ops config file.

Type annotations and code completion for `#!python session.create_client("proton").update_service_sync_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_config)

```python
# update_service_sync_config method definition

await def update_service_sync_config(
    self,
    *,
    branch: str,
    filePath: str,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    serviceName: str,
) -> UpdateServiceSyncConfigOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-braces: UpdateServiceSyncConfigOutputTypeDef](./type_defs.md#updateservicesyncconfigoutputtypedef) 


```python
# update_service_sync_config method usage example with argument unpacking

kwargs: UpdateServiceSyncConfigInputRequestTypeDef = {  # (1)
    "branch": ...,
    "filePath": ...,
    "repositoryName": ...,
    "repositoryProvider": ...,
    "serviceName": ...,
}

parent.update_service_sync_config(**kwargs)
```

1. See [:material-code-braces: UpdateServiceSyncConfigInputRequestTypeDef](./type_defs.md#updateservicesyncconfiginputrequesttypedef) 

### update\_service\_template

Update a service template.

Type annotations and code completion for `#!python session.create_client("proton").update_service_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template)

```python
# update_service_template method definition

await def update_service_template(
    self,
    *,
    name: str,
    description: str = ...,
    displayName: str = ...,
) -> UpdateServiceTemplateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateServiceTemplateOutputTypeDef](./type_defs.md#updateservicetemplateoutputtypedef) 


```python
# update_service_template method usage example with argument unpacking

kwargs: UpdateServiceTemplateInputRequestTypeDef = {  # (1)
    "name": ...,
}

parent.update_service_template(**kwargs)
```

1. See [:material-code-braces: UpdateServiceTemplateInputRequestTypeDef](./type_defs.md#updateservicetemplateinputrequesttypedef) 

### update\_service\_template\_version

Update a major or minor version of a service template.

Type annotations and code completion for `#!python session.create_client("proton").update_service_template_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template_version)

```python
# update_service_template_version method definition

await def update_service_template_version(
    self,
    *,
    majorVersion: str,
    minorVersion: str,
    templateName: str,
    compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef] = ...,  # (1)
    description: str = ...,
    status: TemplateVersionStatusType = ...,  # (2)
    supportedComponentSources: Sequence[ServiceTemplateSupportedComponentSourceTypeType] = ...,  # (3)
) -> UpdateServiceTemplateVersionOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: CompatibleEnvironmentTemplateInputTypeDef](./type_defs.md#compatibleenvironmenttemplateinputtypedef) 
2. See [:material-code-brackets: TemplateVersionStatusType](./literals.md#templateversionstatustype) 
3. See [:material-code-brackets: ServiceTemplateSupportedComponentSourceTypeType](./literals.md#servicetemplatesupportedcomponentsourcetypetype) 
4. See [:material-code-braces: UpdateServiceTemplateVersionOutputTypeDef](./type_defs.md#updateservicetemplateversionoutputtypedef) 


```python
# update_service_template_version method usage example with argument unpacking

kwargs: UpdateServiceTemplateVersionInputRequestTypeDef = {  # (1)
    "majorVersion": ...,
    "minorVersion": ...,
    "templateName": ...,
}

parent.update_service_template_version(**kwargs)
```

1. See [:material-code-braces: UpdateServiceTemplateVersionInputRequestTypeDef](./type_defs.md#updateservicetemplateversioninputrequesttypedef) 

### update\_template\_sync\_config

Update template sync configuration parameters, except for the `templateName` and
`templateType`.

Type annotations and code completion for `#!python session.create_client("proton").update_template_sync_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_template_sync_config)

```python
# update_template_sync_config method definition

await def update_template_sync_config(
    self,
    *,
    branch: str,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    templateName: str,
    templateType: TemplateTypeType,  # (2)
    subdirectory: str = ...,
) -> UpdateTemplateSyncConfigOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
3. See [:material-code-braces: UpdateTemplateSyncConfigOutputTypeDef](./type_defs.md#updatetemplatesyncconfigoutputtypedef) 


```python
# update_template_sync_config method usage example with argument unpacking

kwargs: UpdateTemplateSyncConfigInputRequestTypeDef = {  # (1)
    "branch": ...,
    "repositoryName": ...,
    "repositoryProvider": ...,
    "templateName": ...,
    "templateType": ...,
}

parent.update_template_sync_config(**kwargs)
```

1. See [:material-code-braces: UpdateTemplateSyncConfigInputRequestTypeDef](./type_defs.md#updatetemplatesyncconfiginputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("proton").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> ProtonClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("proton").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("proton").get_paginator` method with overloads.

- `client.get_paginator("list_component_outputs")` -> [ListComponentOutputsPaginator](./paginators.md#listcomponentoutputspaginator)
- `client.get_paginator("list_component_provisioned_resources")` -> [ListComponentProvisionedResourcesPaginator](./paginators.md#listcomponentprovisionedresourcespaginator)
- `client.get_paginator("list_components")` -> [ListComponentsPaginator](./paginators.md#listcomponentspaginator)
- `client.get_paginator("list_deployments")` -> [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
- `client.get_paginator("list_environment_account_connections")` -> [ListEnvironmentAccountConnectionsPaginator](./paginators.md#listenvironmentaccountconnectionspaginator)
- `client.get_paginator("list_environment_outputs")` -> [ListEnvironmentOutputsPaginator](./paginators.md#listenvironmentoutputspaginator)
- `client.get_paginator("list_environment_provisioned_resources")` -> [ListEnvironmentProvisionedResourcesPaginator](./paginators.md#listenvironmentprovisionedresourcespaginator)
- `client.get_paginator("list_environment_template_versions")` -> [ListEnvironmentTemplateVersionsPaginator](./paginators.md#listenvironmenttemplateversionspaginator)
- `client.get_paginator("list_environment_templates")` -> [ListEnvironmentTemplatesPaginator](./paginators.md#listenvironmenttemplatespaginator)
- `client.get_paginator("list_environments")` -> [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
- `client.get_paginator("list_repositories")` -> [ListRepositoriesPaginator](./paginators.md#listrepositoriespaginator)
- `client.get_paginator("list_repository_sync_definitions")` -> [ListRepositorySyncDefinitionsPaginator](./paginators.md#listrepositorysyncdefinitionspaginator)
- `client.get_paginator("list_service_instance_outputs")` -> [ListServiceInstanceOutputsPaginator](./paginators.md#listserviceinstanceoutputspaginator)
- `client.get_paginator("list_service_instance_provisioned_resources")` -> [ListServiceInstanceProvisionedResourcesPaginator](./paginators.md#listserviceinstanceprovisionedresourcespaginator)
- `client.get_paginator("list_service_instances")` -> [ListServiceInstancesPaginator](./paginators.md#listserviceinstancespaginator)
- `client.get_paginator("list_service_pipeline_outputs")` -> [ListServicePipelineOutputsPaginator](./paginators.md#listservicepipelineoutputspaginator)
- `client.get_paginator("list_service_pipeline_provisioned_resources")` -> [ListServicePipelineProvisionedResourcesPaginator](./paginators.md#listservicepipelineprovisionedresourcespaginator)
- `client.get_paginator("list_service_template_versions")` -> [ListServiceTemplateVersionsPaginator](./paginators.md#listservicetemplateversionspaginator)
- `client.get_paginator("list_service_templates")` -> [ListServiceTemplatesPaginator](./paginators.md#listservicetemplatespaginator)
- `client.get_paginator("list_services")` -> [ListServicesPaginator](./paginators.md#listservicespaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("proton").get_waiter` method with overloads.

- `client.get_waiter("component_deleted")` -> [ComponentDeletedWaiter](./waiters.md#componentdeletedwaiter)
- `client.get_waiter("component_deployed")` -> [ComponentDeployedWaiter](./waiters.md#componentdeployedwaiter)
- `client.get_waiter("environment_deployed")` -> [EnvironmentDeployedWaiter](./waiters.md#environmentdeployedwaiter)
- `client.get_waiter("environment_template_version_registered")` -> [EnvironmentTemplateVersionRegisteredWaiter](./waiters.md#environmenttemplateversionregisteredwaiter)
- `client.get_waiter("service_created")` -> [ServiceCreatedWaiter](./waiters.md#servicecreatedwaiter)
- `client.get_waiter("service_deleted")` -> [ServiceDeletedWaiter](./waiters.md#servicedeletedwaiter)
- `client.get_waiter("service_instance_deployed")` -> [ServiceInstanceDeployedWaiter](./waiters.md#serviceinstancedeployedwaiter)
- `client.get_waiter("service_pipeline_deployed")` -> [ServicePipelineDeployedWaiter](./waiters.md#servicepipelinedeployedwaiter)
- `client.get_waiter("service_template_version_registered")` -> [ServiceTemplateVersionRegisteredWaiter](./waiters.md#servicetemplateversionregisteredwaiter)
- `client.get_waiter("service_updated")` -> [ServiceUpdatedWaiter](./waiters.md#serviceupdatedwaiter)

