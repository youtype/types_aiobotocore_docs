<a id="protonclient-for-aiobotocore-proton-module"></a>

# ProtonClient for aiobotocore Proton module

> [Index](..) > [Proton](.) > ProtonClient

Auto-generated documentation for
[Proton](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
type annotations stubs module
[types-aiobotocore-proton](https://pypi.org/project/types-aiobotocore-proton/).

- [ProtonClient for aiobotocore Proton module](#protonclient-for-aiobotocore-proton-module)
  - [ProtonClient](#protonclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [accept_environment_account_connection](#accept_environment_account_connection)
    - [can_paginate](#can_paginate)
    - [cancel_environment_deployment](#cancel_environment_deployment)
    - [cancel_service_instance_deployment](#cancel_service_instance_deployment)
    - [cancel_service_pipeline_deployment](#cancel_service_pipeline_deployment)
    - [create_environment](#create_environment)
    - [create_environment_account_connection](#create_environment_account_connection)
    - [create_environment_template](#create_environment_template)
    - [create_environment_template_version](#create_environment_template_version)
    - [create_repository](#create_repository)
    - [create_service](#create_service)
    - [create_service_template](#create_service_template)
    - [create_service_template_version](#create_service_template_version)
    - [create_template_sync_config](#create_template_sync_config)
    - [delete_environment](#delete_environment)
    - [delete_environment_account_connection](#delete_environment_account_connection)
    - [delete_environment_template](#delete_environment_template)
    - [delete_environment_template_version](#delete_environment_template_version)
    - [delete_repository](#delete_repository)
    - [delete_service](#delete_service)
    - [delete_service_template](#delete_service_template)
    - [delete_service_template_version](#delete_service_template_version)
    - [delete_template_sync_config](#delete_template_sync_config)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_account_settings](#get_account_settings)
    - [get_environment](#get_environment)
    - [get_environment_account_connection](#get_environment_account_connection)
    - [get_environment_template](#get_environment_template)
    - [get_environment_template_version](#get_environment_template_version)
    - [get_repository](#get_repository)
    - [get_repository_sync_status](#get_repository_sync_status)
    - [get_service](#get_service)
    - [get_service_instance](#get_service_instance)
    - [get_service_template](#get_service_template)
    - [get_service_template_version](#get_service_template_version)
    - [get_template_sync_config](#get_template_sync_config)
    - [get_template_sync_status](#get_template_sync_status)
    - [list_environment_account_connections](#list_environment_account_connections)
    - [list_environment_outputs](#list_environment_outputs)
    - [list_environment_provisioned_resources](#list_environment_provisioned_resources)
    - [list_environment_template_versions](#list_environment_template_versions)
    - [list_environment_templates](#list_environment_templates)
    - [list_environments](#list_environments)
    - [list_repositories](#list_repositories)
    - [list_repository_sync_definitions](#list_repository_sync_definitions)
    - [list_service_instance_outputs](#list_service_instance_outputs)
    - [list_service_instance_provisioned_resources](#list_service_instance_provisioned_resources)
    - [list_service_instances](#list_service_instances)
    - [list_service_pipeline_outputs](#list_service_pipeline_outputs)
    - [list_service_pipeline_provisioned_resources](#list_service_pipeline_provisioned_resources)
    - [list_service_template_versions](#list_service_template_versions)
    - [list_service_templates](#list_service_templates)
    - [list_services](#list_services)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [notify_resource_deployment_status_change](#notify_resource_deployment_status_change)
    - [reject_environment_account_connection](#reject_environment_account_connection)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_account_settings](#update_account_settings)
    - [update_environment](#update_environment)
    - [update_environment_account_connection](#update_environment_account_connection)
    - [update_environment_template](#update_environment_template)
    - [update_environment_template_version](#update_environment_template_version)
    - [update_service](#update_service)
    - [update_service_instance](#update_service_instance)
    - [update_service_pipeline](#update_service_pipeline)
    - [update_service_template](#update_service_template)
    - [update_service_template_version](#update_service_template_version)
    - [update_template_sync_config](#update_template_sync_config)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="protonclient"></a>

## ProtonClient

Type annotations for `session.create_client("proton")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_proton.client import ProtonClient

session = get_session()
async with session.create_client("proton") as client:
    client: ProtonClient
```

Boto3 documentation:
[Proton.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_proton.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ProtonClient exceptions.

Type annotations for `session.create_client("proton").exceptions` method.

Boto3 documentation:
[Proton.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="accept_environment_account_connection"></a>

### accept_environment_account_connection

In a management account, an environment account connection request is accepted.

Type annotations for
`session.create_client("proton").accept_environment_account_connection` method.

Boto3 documentation:
[Proton.Client.accept_environment_account_connection](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.accept_environment_account_connection)

Asynchronous method. Use `await accept_environment_account_connection(...)` for
a synchronous call.

Arguments mapping described in
[AcceptEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#acceptenvironmentaccountconnectioninputrequesttypedef).

Keyword-only arguments:

- `id`: `str` *(required)*

Returns a `Coroutine` for
[AcceptEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#acceptenvironmentaccountconnectionoutputtypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("proton").can_paginate` method.

Boto3 documentation:
[Proton.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel_environment_deployment"></a>

### cancel_environment_deployment

Attempts to cancel an environment deployment on an UpdateEnvironment action, if
the deployment is `IN_PROGRESS`.

Type annotations for
`session.create_client("proton").cancel_environment_deployment` method.

Boto3 documentation:
[Proton.Client.cancel_environment_deployment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_environment_deployment)

Asynchronous method. Use `await cancel_environment_deployment(...)` for a
synchronous call.

Arguments mapping described in
[CancelEnvironmentDeploymentInputRequestTypeDef](./type_defs.md#cancelenvironmentdeploymentinputrequesttypedef).

Keyword-only arguments:

- `environmentName`: `str` *(required)*

Returns a `Coroutine` for
[CancelEnvironmentDeploymentOutputTypeDef](./type_defs.md#cancelenvironmentdeploymentoutputtypedef).

<a id="cancel_service_instance_deployment"></a>

### cancel_service_instance_deployment

Attempts to cancel a service instance deployment on an UpdateServiceInstance
action, if the deployment is `IN_PROGRESS`.

Type annotations for
`session.create_client("proton").cancel_service_instance_deployment` method.

Boto3 documentation:
[Proton.Client.cancel_service_instance_deployment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_instance_deployment)

Asynchronous method. Use `await cancel_service_instance_deployment(...)` for a
synchronous call.

Arguments mapping described in
[CancelServiceInstanceDeploymentInputRequestTypeDef](./type_defs.md#cancelserviceinstancedeploymentinputrequesttypedef).

Keyword-only arguments:

- `serviceInstanceName`: `str` *(required)*
- `serviceName`: `str` *(required)*

Returns a `Coroutine` for
[CancelServiceInstanceDeploymentOutputTypeDef](./type_defs.md#cancelserviceinstancedeploymentoutputtypedef).

<a id="cancel_service_pipeline_deployment"></a>

### cancel_service_pipeline_deployment

Attempts to cancel a service pipeline deployment on an UpdateServicePipeline
action, if the deployment is `IN_PROGRESS`.

Type annotations for
`session.create_client("proton").cancel_service_pipeline_deployment` method.

Boto3 documentation:
[Proton.Client.cancel_service_pipeline_deployment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_pipeline_deployment)

Asynchronous method. Use `await cancel_service_pipeline_deployment(...)` for a
synchronous call.

Arguments mapping described in
[CancelServicePipelineDeploymentInputRequestTypeDef](./type_defs.md#cancelservicepipelinedeploymentinputrequesttypedef).

Keyword-only arguments:

- `serviceName`: `str` *(required)*

Returns a `Coroutine` for
[CancelServicePipelineDeploymentOutputTypeDef](./type_defs.md#cancelservicepipelinedeploymentoutputtypedef).

<a id="create_environment"></a>

### create_environment

Deploy a new environment.

Type annotations for `session.create_client("proton").create_environment`
method.

Boto3 documentation:
[Proton.Client.create_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment)

Asynchronous method. Use `await create_environment(...)` for a synchronous
call.

Arguments mapping described in
[CreateEnvironmentInputRequestTypeDef](./type_defs.md#createenvironmentinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `spec`: `str` *(required)*
- `templateMajorVersion`: `str` *(required)*
- `templateName`: `str` *(required)*
- `description`: `str`
- `environmentAccountConnectionId`: `str`
- `protonServiceRoleArn`: `str`
- `provisioningRepository`:
  [RepositoryBranchInputTypeDef](./type_defs.md#repositorybranchinputtypedef)
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `templateMinorVersion`: `str`

Returns a `Coroutine` for
[CreateEnvironmentOutputTypeDef](./type_defs.md#createenvironmentoutputtypedef).

<a id="create_environment_account_connection"></a>

### create_environment_account_connection

Create an environment account connection in an environment account so that
environment infrastructure resources can be provisioned in the environment
account from a management account.

Type annotations for
`session.create_client("proton").create_environment_account_connection` method.

Boto3 documentation:
[Proton.Client.create_environment_account_connection](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_account_connection)

Asynchronous method. Use `await create_environment_account_connection(...)` for
a synchronous call.

Arguments mapping described in
[CreateEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#createenvironmentaccountconnectioninputrequesttypedef).

Keyword-only arguments:

- `environmentName`: `str` *(required)*
- `managementAccountId`: `str` *(required)*
- `roleArn`: `str` *(required)*
- `clientToken`: `str`
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#createenvironmentaccountconnectionoutputtypedef).

<a id="create_environment_template"></a>

### create_environment_template

Create an environment template for Proton.

Type annotations for
`session.create_client("proton").create_environment_template` method.

Boto3 documentation:
[Proton.Client.create_environment_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template)

Asynchronous method. Use `await create_environment_template(...)` for a
synchronous call.

Arguments mapping described in
[CreateEnvironmentTemplateInputRequestTypeDef](./type_defs.md#createenvironmenttemplateinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `description`: `str`
- `displayName`: `str`
- `encryptionKey`: `str`
- `provisioning`: `Literal['CUSTOMER_MANAGED']` (see
  [ProvisioningType](./literals.md#provisioningtype))
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateEnvironmentTemplateOutputTypeDef](./type_defs.md#createenvironmenttemplateoutputtypedef).

<a id="create_environment_template_version"></a>

### create_environment_template_version

Create a new major or minor version of an environment template.

Type annotations for
`session.create_client("proton").create_environment_template_version` method.

Boto3 documentation:
[Proton.Client.create_environment_template_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template_version)

Asynchronous method. Use `await create_environment_template_version(...)` for a
synchronous call.

Arguments mapping described in
[CreateEnvironmentTemplateVersionInputRequestTypeDef](./type_defs.md#createenvironmenttemplateversioninputrequesttypedef).

Keyword-only arguments:

- `source`:
  [TemplateVersionSourceInputTypeDef](./type_defs.md#templateversionsourceinputtypedef)
  *(required)*
- `templateName`: `str` *(required)*
- `clientToken`: `str`
- `description`: `str`
- `majorVersion`: `str`
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateEnvironmentTemplateVersionOutputTypeDef](./type_defs.md#createenvironmenttemplateversionoutputtypedef).

<a id="create_repository"></a>

### create_repository

Create and register a link to a repository that can be used with pull request
provisioning or template sync configurations.

Type annotations for `session.create_client("proton").create_repository`
method.

Boto3 documentation:
[Proton.Client.create_repository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_repository)

Asynchronous method. Use `await create_repository(...)` for a synchronous call.

Arguments mapping described in
[CreateRepositoryInputRequestTypeDef](./type_defs.md#createrepositoryinputrequesttypedef).

Keyword-only arguments:

- `connectionArn`: `str` *(required)*
- `name`: `str` *(required)*
- `provider`: [RepositoryProviderType](./literals.md#repositoryprovidertype)
  *(required)*
- `encryptionKey`: `str`

Returns a `Coroutine` for
[CreateRepositoryOutputTypeDef](./type_defs.md#createrepositoryoutputtypedef).

<a id="create_service"></a>

### create_service

Create an Proton service.

Type annotations for `session.create_client("proton").create_service` method.

Boto3 documentation:
[Proton.Client.create_service](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service)

Asynchronous method. Use `await create_service(...)` for a synchronous call.

Arguments mapping described in
[CreateServiceInputRequestTypeDef](./type_defs.md#createserviceinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `spec`: `str` *(required)*
- `templateMajorVersion`: `str` *(required)*
- `templateName`: `str` *(required)*
- `branchName`: `str`
- `description`: `str`
- `repositoryConnectionArn`: `str`
- `repositoryId`: `str`
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `templateMinorVersion`: `str`

Returns a `Coroutine` for
[CreateServiceOutputTypeDef](./type_defs.md#createserviceoutputtypedef).

<a id="create_service_template"></a>

### create_service_template

Create a service template.

Type annotations for `session.create_client("proton").create_service_template`
method.

Boto3 documentation:
[Proton.Client.create_service_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template)

Asynchronous method. Use `await create_service_template(...)` for a synchronous
call.

Arguments mapping described in
[CreateServiceTemplateInputRequestTypeDef](./type_defs.md#createservicetemplateinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `description`: `str`
- `displayName`: `str`
- `encryptionKey`: `str`
- `pipelineProvisioning`: `Literal['CUSTOMER_MANAGED']` (see
  [ProvisioningType](./literals.md#provisioningtype))
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateServiceTemplateOutputTypeDef](./type_defs.md#createservicetemplateoutputtypedef).

<a id="create_service_template_version"></a>

### create_service_template_version

Create a new major or minor version of a service template.

Type annotations for
`session.create_client("proton").create_service_template_version` method.

Boto3 documentation:
[Proton.Client.create_service_template_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template_version)

Asynchronous method. Use `await create_service_template_version(...)` for a
synchronous call.

Arguments mapping described in
[CreateServiceTemplateVersionInputRequestTypeDef](./type_defs.md#createservicetemplateversioninputrequesttypedef).

Keyword-only arguments:

- `compatibleEnvironmentTemplates`:
  `Sequence`\[[CompatibleEnvironmentTemplateInputTypeDef](./type_defs.md#compatibleenvironmenttemplateinputtypedef)\]
  *(required)*
- `source`:
  [TemplateVersionSourceInputTypeDef](./type_defs.md#templateversionsourceinputtypedef)
  *(required)*
- `templateName`: `str` *(required)*
- `clientToken`: `str`
- `description`: `str`
- `majorVersion`: `str`
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateServiceTemplateVersionOutputTypeDef](./type_defs.md#createservicetemplateversionoutputtypedef).

<a id="create_template_sync_config"></a>

### create_template_sync_config

Set up a template for automated template version creation.

Type annotations for
`session.create_client("proton").create_template_sync_config` method.

Boto3 documentation:
[Proton.Client.create_template_sync_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_template_sync_config)

Asynchronous method. Use `await create_template_sync_config(...)` for a
synchronous call.

Arguments mapping described in
[CreateTemplateSyncConfigInputRequestTypeDef](./type_defs.md#createtemplatesyncconfiginputrequesttypedef).

Keyword-only arguments:

- `branch`: `str` *(required)*
- `repositoryName`: `str` *(required)*
- `repositoryProvider`:
  [RepositoryProviderType](./literals.md#repositoryprovidertype) *(required)*
- `templateName`: `str` *(required)*
- `templateType`: [TemplateTypeType](./literals.md#templatetypetype)
  *(required)*
- `subdirectory`: `str`

Returns a `Coroutine` for
[CreateTemplateSyncConfigOutputTypeDef](./type_defs.md#createtemplatesyncconfigoutputtypedef).

<a id="delete_environment"></a>

### delete_environment

Delete an environment.

Type annotations for `session.create_client("proton").delete_environment`
method.

Boto3 documentation:
[Proton.Client.delete_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment)

Asynchronous method. Use `await delete_environment(...)` for a synchronous
call.

Arguments mapping described in
[DeleteEnvironmentInputRequestTypeDef](./type_defs.md#deleteenvironmentinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*

Returns a `Coroutine` for
[DeleteEnvironmentOutputTypeDef](./type_defs.md#deleteenvironmentoutputtypedef).

<a id="delete_environment_account_connection"></a>

### delete_environment_account_connection

In an environment account, delete an environment account connection.

Type annotations for
`session.create_client("proton").delete_environment_account_connection` method.

Boto3 documentation:
[Proton.Client.delete_environment_account_connection](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_account_connection)

Asynchronous method. Use `await delete_environment_account_connection(...)` for
a synchronous call.

Arguments mapping described in
[DeleteEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#deleteenvironmentaccountconnectioninputrequesttypedef).

Keyword-only arguments:

- `id`: `str` *(required)*

Returns a `Coroutine` for
[DeleteEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#deleteenvironmentaccountconnectionoutputtypedef).

<a id="delete_environment_template"></a>

### delete_environment_template

If no other major or minor versions of an environment template exist, delete
the environment template.

Type annotations for
`session.create_client("proton").delete_environment_template` method.

Boto3 documentation:
[Proton.Client.delete_environment_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template)

Asynchronous method. Use `await delete_environment_template(...)` for a
synchronous call.

Arguments mapping described in
[DeleteEnvironmentTemplateInputRequestTypeDef](./type_defs.md#deleteenvironmenttemplateinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*

Returns a `Coroutine` for
[DeleteEnvironmentTemplateOutputTypeDef](./type_defs.md#deleteenvironmenttemplateoutputtypedef).

<a id="delete_environment_template_version"></a>

### delete_environment_template_version

If no other minor versions of an environment template exist, delete a major
version of the environment template if it's not the `Recommended` version.

Type annotations for
`session.create_client("proton").delete_environment_template_version` method.

Boto3 documentation:
[Proton.Client.delete_environment_template_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template_version)

Asynchronous method. Use `await delete_environment_template_version(...)` for a
synchronous call.

Arguments mapping described in
[DeleteEnvironmentTemplateVersionInputRequestTypeDef](./type_defs.md#deleteenvironmenttemplateversioninputrequesttypedef).

Keyword-only arguments:

- `majorVersion`: `str` *(required)*
- `minorVersion`: `str` *(required)*
- `templateName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteEnvironmentTemplateVersionOutputTypeDef](./type_defs.md#deleteenvironmenttemplateversionoutputtypedef).

<a id="delete_repository"></a>

### delete_repository

De-register and unlink your repository.

Type annotations for `session.create_client("proton").delete_repository`
method.

Boto3 documentation:
[Proton.Client.delete_repository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_repository)

Asynchronous method. Use `await delete_repository(...)` for a synchronous call.

Arguments mapping described in
[DeleteRepositoryInputRequestTypeDef](./type_defs.md#deleterepositoryinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `provider`: [RepositoryProviderType](./literals.md#repositoryprovidertype)
  *(required)*

Returns a `Coroutine` for
[DeleteRepositoryOutputTypeDef](./type_defs.md#deleterepositoryoutputtypedef).

<a id="delete_service"></a>

### delete_service

Delete a service.

Type annotations for `session.create_client("proton").delete_service` method.

Boto3 documentation:
[Proton.Client.delete_service](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service)

Asynchronous method. Use `await delete_service(...)` for a synchronous call.

Arguments mapping described in
[DeleteServiceInputRequestTypeDef](./type_defs.md#deleteserviceinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*

Returns a `Coroutine` for
[DeleteServiceOutputTypeDef](./type_defs.md#deleteserviceoutputtypedef).

<a id="delete_service_template"></a>

### delete_service_template

If no other major or minor versions of the service template exist, delete the
service template.

Type annotations for `session.create_client("proton").delete_service_template`
method.

Boto3 documentation:
[Proton.Client.delete_service_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template)

Asynchronous method. Use `await delete_service_template(...)` for a synchronous
call.

Arguments mapping described in
[DeleteServiceTemplateInputRequestTypeDef](./type_defs.md#deleteservicetemplateinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*

Returns a `Coroutine` for
[DeleteServiceTemplateOutputTypeDef](./type_defs.md#deleteservicetemplateoutputtypedef).

<a id="delete_service_template_version"></a>

### delete_service_template_version

If no other minor versions of a service template exist, delete a major version
of the service template if it's not the `Recommended` version.

Type annotations for
`session.create_client("proton").delete_service_template_version` method.

Boto3 documentation:
[Proton.Client.delete_service_template_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template_version)

Asynchronous method. Use `await delete_service_template_version(...)` for a
synchronous call.

Arguments mapping described in
[DeleteServiceTemplateVersionInputRequestTypeDef](./type_defs.md#deleteservicetemplateversioninputrequesttypedef).

Keyword-only arguments:

- `majorVersion`: `str` *(required)*
- `minorVersion`: `str` *(required)*
- `templateName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteServiceTemplateVersionOutputTypeDef](./type_defs.md#deleteservicetemplateversionoutputtypedef).

<a id="delete_template_sync_config"></a>

### delete_template_sync_config

Delete a template sync configuration.

Type annotations for
`session.create_client("proton").delete_template_sync_config` method.

Boto3 documentation:
[Proton.Client.delete_template_sync_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_template_sync_config)

Asynchronous method. Use `await delete_template_sync_config(...)` for a
synchronous call.

Arguments mapping described in
[DeleteTemplateSyncConfigInputRequestTypeDef](./type_defs.md#deletetemplatesyncconfiginputrequesttypedef).

Keyword-only arguments:

- `templateName`: `str` *(required)*
- `templateType`: [TemplateTypeType](./literals.md#templatetypetype)
  *(required)*

Returns a `Coroutine` for
[DeleteTemplateSyncConfigOutputTypeDef](./type_defs.md#deletetemplatesyncconfigoutputtypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("proton").generate_presigned_url`
method.

Boto3 documentation:
[Proton.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_account_settings"></a>

### get_account_settings

Get detail data for the Proton pipeline service role.

Type annotations for `session.create_client("proton").get_account_settings`
method.

Boto3 documentation:
[Proton.Client.get_account_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_account_settings)

Asynchronous method. Use `await get_account_settings(...)` for a synchronous
call.

Returns a `Coroutine` for
[GetAccountSettingsOutputTypeDef](./type_defs.md#getaccountsettingsoutputtypedef).

<a id="get_environment"></a>

### get_environment

Get detail data for an environment.

Type annotations for `session.create_client("proton").get_environment` method.

Boto3 documentation:
[Proton.Client.get_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment)

Asynchronous method. Use `await get_environment(...)` for a synchronous call.

Arguments mapping described in
[GetEnvironmentInputRequestTypeDef](./type_defs.md#getenvironmentinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*

Returns a `Coroutine` for
[GetEnvironmentOutputTypeDef](./type_defs.md#getenvironmentoutputtypedef).

<a id="get_environment_account_connection"></a>

### get_environment_account_connection

In an environment account, view the detail data for an environment account
connection.

Type annotations for
`session.create_client("proton").get_environment_account_connection` method.

Boto3 documentation:
[Proton.Client.get_environment_account_connection](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_account_connection)

Asynchronous method. Use `await get_environment_account_connection(...)` for a
synchronous call.

Arguments mapping described in
[GetEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#getenvironmentaccountconnectioninputrequesttypedef).

Keyword-only arguments:

- `id`: `str` *(required)*

Returns a `Coroutine` for
[GetEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#getenvironmentaccountconnectionoutputtypedef).

<a id="get_environment_template"></a>

### get_environment_template

Get detail data for an environment template.

Type annotations for `session.create_client("proton").get_environment_template`
method.

Boto3 documentation:
[Proton.Client.get_environment_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template)

Asynchronous method. Use `await get_environment_template(...)` for a
synchronous call.

Arguments mapping described in
[GetEnvironmentTemplateInputRequestTypeDef](./type_defs.md#getenvironmenttemplateinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*

Returns a `Coroutine` for
[GetEnvironmentTemplateOutputTypeDef](./type_defs.md#getenvironmenttemplateoutputtypedef).

<a id="get_environment_template_version"></a>

### get_environment_template_version

View detail data for a major or minor version of an environment template.

Type annotations for
`session.create_client("proton").get_environment_template_version` method.

Boto3 documentation:
[Proton.Client.get_environment_template_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template_version)

Asynchronous method. Use `await get_environment_template_version(...)` for a
synchronous call.

Arguments mapping described in
[GetEnvironmentTemplateVersionInputRequestTypeDef](./type_defs.md#getenvironmenttemplateversioninputrequesttypedef).

Keyword-only arguments:

- `majorVersion`: `str` *(required)*
- `minorVersion`: `str` *(required)*
- `templateName`: `str` *(required)*

Returns a `Coroutine` for
[GetEnvironmentTemplateVersionOutputTypeDef](./type_defs.md#getenvironmenttemplateversionoutputtypedef).

<a id="get_repository"></a>

### get_repository

Get detail data for a repository.

Type annotations for `session.create_client("proton").get_repository` method.

Boto3 documentation:
[Proton.Client.get_repository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository)

Asynchronous method. Use `await get_repository(...)` for a synchronous call.

Arguments mapping described in
[GetRepositoryInputRequestTypeDef](./type_defs.md#getrepositoryinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `provider`: [RepositoryProviderType](./literals.md#repositoryprovidertype)
  *(required)*

Returns a `Coroutine` for
[GetRepositoryOutputTypeDef](./type_defs.md#getrepositoryoutputtypedef).

<a id="get_repository_sync_status"></a>

### get_repository_sync_status

Get the repository sync status.

Type annotations for
`session.create_client("proton").get_repository_sync_status` method.

Boto3 documentation:
[Proton.Client.get_repository_sync_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository_sync_status)

Asynchronous method. Use `await get_repository_sync_status(...)` for a
synchronous call.

Arguments mapping described in
[GetRepositorySyncStatusInputRequestTypeDef](./type_defs.md#getrepositorysyncstatusinputrequesttypedef).

Keyword-only arguments:

- `branch`: `str` *(required)*
- `repositoryName`: `str` *(required)*
- `repositoryProvider`:
  [RepositoryProviderType](./literals.md#repositoryprovidertype) *(required)*
- `syncType`: `Literal['TEMPLATE_SYNC']` (see
  [SyncTypeType](./literals.md#synctypetype)) *(required)*

Returns a `Coroutine` for
[GetRepositorySyncStatusOutputTypeDef](./type_defs.md#getrepositorysyncstatusoutputtypedef).

<a id="get_service"></a>

### get_service

Get detail data for a service.

Type annotations for `session.create_client("proton").get_service` method.

Boto3 documentation:
[Proton.Client.get_service](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service)

Asynchronous method. Use `await get_service(...)` for a synchronous call.

Arguments mapping described in
[GetServiceInputRequestTypeDef](./type_defs.md#getserviceinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*

Returns a `Coroutine` for
[GetServiceOutputTypeDef](./type_defs.md#getserviceoutputtypedef).

<a id="get_service_instance"></a>

### get_service_instance

Get detail data for a service instance.

Type annotations for `session.create_client("proton").get_service_instance`
method.

Boto3 documentation:
[Proton.Client.get_service_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance)

Asynchronous method. Use `await get_service_instance(...)` for a synchronous
call.

Arguments mapping described in
[GetServiceInstanceInputRequestTypeDef](./type_defs.md#getserviceinstanceinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `serviceName`: `str` *(required)*

Returns a `Coroutine` for
[GetServiceInstanceOutputTypeDef](./type_defs.md#getserviceinstanceoutputtypedef).

<a id="get_service_template"></a>

### get_service_template

Get detail data for a service template.

Type annotations for `session.create_client("proton").get_service_template`
method.

Boto3 documentation:
[Proton.Client.get_service_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template)

Asynchronous method. Use `await get_service_template(...)` for a synchronous
call.

Arguments mapping described in
[GetServiceTemplateInputRequestTypeDef](./type_defs.md#getservicetemplateinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*

Returns a `Coroutine` for
[GetServiceTemplateOutputTypeDef](./type_defs.md#getservicetemplateoutputtypedef).

<a id="get_service_template_version"></a>

### get_service_template_version

View detail data for a major or minor version of a service template.

Type annotations for
`session.create_client("proton").get_service_template_version` method.

Boto3 documentation:
[Proton.Client.get_service_template_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template_version)

Asynchronous method. Use `await get_service_template_version(...)` for a
synchronous call.

Arguments mapping described in
[GetServiceTemplateVersionInputRequestTypeDef](./type_defs.md#getservicetemplateversioninputrequesttypedef).

Keyword-only arguments:

- `majorVersion`: `str` *(required)*
- `minorVersion`: `str` *(required)*
- `templateName`: `str` *(required)*

Returns a `Coroutine` for
[GetServiceTemplateVersionOutputTypeDef](./type_defs.md#getservicetemplateversionoutputtypedef).

<a id="get_template_sync_config"></a>

### get_template_sync_config

Get detail data for a template sync configuration.

Type annotations for `session.create_client("proton").get_template_sync_config`
method.

Boto3 documentation:
[Proton.Client.get_template_sync_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_config)

Asynchronous method. Use `await get_template_sync_config(...)` for a
synchronous call.

Arguments mapping described in
[GetTemplateSyncConfigInputRequestTypeDef](./type_defs.md#gettemplatesyncconfiginputrequesttypedef).

Keyword-only arguments:

- `templateName`: `str` *(required)*
- `templateType`: [TemplateTypeType](./literals.md#templatetypetype)
  *(required)*

Returns a `Coroutine` for
[GetTemplateSyncConfigOutputTypeDef](./type_defs.md#gettemplatesyncconfigoutputtypedef).

<a id="get_template_sync_status"></a>

### get_template_sync_status

Get the status of a template sync.

Type annotations for `session.create_client("proton").get_template_sync_status`
method.

Boto3 documentation:
[Proton.Client.get_template_sync_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_status)

Asynchronous method. Use `await get_template_sync_status(...)` for a
synchronous call.

Arguments mapping described in
[GetTemplateSyncStatusInputRequestTypeDef](./type_defs.md#gettemplatesyncstatusinputrequesttypedef).

Keyword-only arguments:

- `templateName`: `str` *(required)*
- `templateType`: [TemplateTypeType](./literals.md#templatetypetype)
  *(required)*
- `templateVersion`: `str` *(required)*

Returns a `Coroutine` for
[GetTemplateSyncStatusOutputTypeDef](./type_defs.md#gettemplatesyncstatusoutputtypedef).

<a id="list_environment_account_connections"></a>

### list_environment_account_connections

View a list of environment account connections.

Type annotations for
`session.create_client("proton").list_environment_account_connections` method.

Boto3 documentation:
[Proton.Client.list_environment_account_connections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)

Asynchronous method. Use `await list_environment_account_connections(...)` for
a synchronous call.

Arguments mapping described in
[ListEnvironmentAccountConnectionsInputRequestTypeDef](./type_defs.md#listenvironmentaccountconnectionsinputrequesttypedef).

Keyword-only arguments:

- `requestedBy`:
  [EnvironmentAccountConnectionRequesterAccountTypeType](./literals.md#environmentaccountconnectionrequesteraccounttypetype)
  *(required)*
- `environmentName`: `str`
- `maxResults`: `int`
- `nextToken`: `str`
- `statuses`:
  `Sequence`\[[EnvironmentAccountConnectionStatusType](./literals.md#environmentaccountconnectionstatustype)\]

Returns a `Coroutine` for
[ListEnvironmentAccountConnectionsOutputTypeDef](./type_defs.md#listenvironmentaccountconnectionsoutputtypedef).

<a id="list_environment_outputs"></a>

### list_environment_outputs

List the infrastructure as code outputs for your environment.

Type annotations for `session.create_client("proton").list_environment_outputs`
method.

Boto3 documentation:
[Proton.Client.list_environment_outputs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_outputs)

Asynchronous method. Use `await list_environment_outputs(...)` for a
synchronous call.

Arguments mapping described in
[ListEnvironmentOutputsInputRequestTypeDef](./type_defs.md#listenvironmentoutputsinputrequesttypedef).

Keyword-only arguments:

- `environmentName`: `str` *(required)*
- `nextToken`: `str`

Returns a `Coroutine` for
[ListEnvironmentOutputsOutputTypeDef](./type_defs.md#listenvironmentoutputsoutputtypedef).

<a id="list_environment_provisioned_resources"></a>

### list_environment_provisioned_resources

List the provisioned resources for your environment.

Type annotations for
`session.create_client("proton").list_environment_provisioned_resources`
method.

Boto3 documentation:
[Proton.Client.list_environment_provisioned_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_provisioned_resources)

Asynchronous method. Use `await list_environment_provisioned_resources(...)`
for a synchronous call.

Arguments mapping described in
[ListEnvironmentProvisionedResourcesInputRequestTypeDef](./type_defs.md#listenvironmentprovisionedresourcesinputrequesttypedef).

Keyword-only arguments:

- `environmentName`: `str` *(required)*
- `nextToken`: `str`

Returns a `Coroutine` for
[ListEnvironmentProvisionedResourcesOutputTypeDef](./type_defs.md#listenvironmentprovisionedresourcesoutputtypedef).

<a id="list_environment_template_versions"></a>

### list_environment_template_versions

List major or minor versions of an environment template with detail data.

Type annotations for
`session.create_client("proton").list_environment_template_versions` method.

Boto3 documentation:
[Proton.Client.list_environment_template_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_template_versions)

Asynchronous method. Use `await list_environment_template_versions(...)` for a
synchronous call.

Arguments mapping described in
[ListEnvironmentTemplateVersionsInputRequestTypeDef](./type_defs.md#listenvironmenttemplateversionsinputrequesttypedef).

Keyword-only arguments:

- `templateName`: `str` *(required)*
- `majorVersion`: `str`
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListEnvironmentTemplateVersionsOutputTypeDef](./type_defs.md#listenvironmenttemplateversionsoutputtypedef).

<a id="list_environment_templates"></a>

### list_environment_templates

List environment templates.

Type annotations for
`session.create_client("proton").list_environment_templates` method.

Boto3 documentation:
[Proton.Client.list_environment_templates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_templates)

Asynchronous method. Use `await list_environment_templates(...)` for a
synchronous call.

Arguments mapping described in
[ListEnvironmentTemplatesInputRequestTypeDef](./type_defs.md#listenvironmenttemplatesinputrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListEnvironmentTemplatesOutputTypeDef](./type_defs.md#listenvironmenttemplatesoutputtypedef).

<a id="list_environments"></a>

### list_environments

List environments with detail data summaries.

Type annotations for `session.create_client("proton").list_environments`
method.

Boto3 documentation:
[Proton.Client.list_environments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environments)

Asynchronous method. Use `await list_environments(...)` for a synchronous call.

Arguments mapping described in
[ListEnvironmentsInputRequestTypeDef](./type_defs.md#listenvironmentsinputrequesttypedef).

Keyword-only arguments:

- `environmentTemplates`:
  `Sequence`\[[EnvironmentTemplateFilterTypeDef](./type_defs.md#environmenttemplatefiltertypedef)\]
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListEnvironmentsOutputTypeDef](./type_defs.md#listenvironmentsoutputtypedef).

<a id="list_repositories"></a>

### list_repositories

List repositories with detail data.

Type annotations for `session.create_client("proton").list_repositories`
method.

Boto3 documentation:
[Proton.Client.list_repositories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repositories)

Asynchronous method. Use `await list_repositories(...)` for a synchronous call.

Arguments mapping described in
[ListRepositoriesInputRequestTypeDef](./type_defs.md#listrepositoriesinputrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListRepositoriesOutputTypeDef](./type_defs.md#listrepositoriesoutputtypedef).

<a id="list_repository_sync_definitions"></a>

### list_repository_sync_definitions

List repository sync definitions with detail data.

Type annotations for
`session.create_client("proton").list_repository_sync_definitions` method.

Boto3 documentation:
[Proton.Client.list_repository_sync_definitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)

Asynchronous method. Use `await list_repository_sync_definitions(...)` for a
synchronous call.

Arguments mapping described in
[ListRepositorySyncDefinitionsInputRequestTypeDef](./type_defs.md#listrepositorysyncdefinitionsinputrequesttypedef).

Keyword-only arguments:

- `repositoryName`: `str` *(required)*
- `repositoryProvider`:
  [RepositoryProviderType](./literals.md#repositoryprovidertype) *(required)*
- `syncType`: `Literal['TEMPLATE_SYNC']` (see
  [SyncTypeType](./literals.md#synctypetype)) *(required)*
- `nextToken`: `str`

Returns a `Coroutine` for
[ListRepositorySyncDefinitionsOutputTypeDef](./type_defs.md#listrepositorysyncdefinitionsoutputtypedef).

<a id="list_service_instance_outputs"></a>

### list_service_instance_outputs

View a list service instance infrastructure as code outputs with detail data.

Type annotations for
`session.create_client("proton").list_service_instance_outputs` method.

Boto3 documentation:
[Proton.Client.list_service_instance_outputs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)

Asynchronous method. Use `await list_service_instance_outputs(...)` for a
synchronous call.

Arguments mapping described in
[ListServiceInstanceOutputsInputRequestTypeDef](./type_defs.md#listserviceinstanceoutputsinputrequesttypedef).

Keyword-only arguments:

- `serviceInstanceName`: `str` *(required)*
- `serviceName`: `str` *(required)*
- `nextToken`: `str`

Returns a `Coroutine` for
[ListServiceInstanceOutputsOutputTypeDef](./type_defs.md#listserviceinstanceoutputsoutputtypedef).

<a id="list_service_instance_provisioned_resources"></a>

### list_service_instance_provisioned_resources

List provisioned resources for a service instance with details.

Type annotations for
`session.create_client("proton").list_service_instance_provisioned_resources`
method.

Boto3 documentation:
[Proton.Client.list_service_instance_provisioned_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_provisioned_resources)

Asynchronous method. Use
`await list_service_instance_provisioned_resources(...)` for a synchronous
call.

Arguments mapping described in
[ListServiceInstanceProvisionedResourcesInputRequestTypeDef](./type_defs.md#listserviceinstanceprovisionedresourcesinputrequesttypedef).

Keyword-only arguments:

- `serviceInstanceName`: `str` *(required)*
- `serviceName`: `str` *(required)*
- `nextToken`: `str`

Returns a `Coroutine` for
[ListServiceInstanceProvisionedResourcesOutputTypeDef](./type_defs.md#listserviceinstanceprovisionedresourcesoutputtypedef).

<a id="list_service_instances"></a>

### list_service_instances

List service instances with summaries of detail data.

Type annotations for `session.create_client("proton").list_service_instances`
method.

Boto3 documentation:
[Proton.Client.list_service_instances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)

Asynchronous method. Use `await list_service_instances(...)` for a synchronous
call.

Arguments mapping described in
[ListServiceInstancesInputRequestTypeDef](./type_defs.md#listserviceinstancesinputrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`
- `serviceName`: `str`

Returns a `Coroutine` for
[ListServiceInstancesOutputTypeDef](./type_defs.md#listserviceinstancesoutputtypedef).

<a id="list_service_pipeline_outputs"></a>

### list_service_pipeline_outputs

View a list service pipeline infrastructure as code outputs with detail.

Type annotations for
`session.create_client("proton").list_service_pipeline_outputs` method.

Boto3 documentation:
[Proton.Client.list_service_pipeline_outputs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_outputs)

Asynchronous method. Use `await list_service_pipeline_outputs(...)` for a
synchronous call.

Arguments mapping described in
[ListServicePipelineOutputsInputRequestTypeDef](./type_defs.md#listservicepipelineoutputsinputrequesttypedef).

Keyword-only arguments:

- `serviceName`: `str` *(required)*
- `nextToken`: `str`

Returns a `Coroutine` for
[ListServicePipelineOutputsOutputTypeDef](./type_defs.md#listservicepipelineoutputsoutputtypedef).

<a id="list_service_pipeline_provisioned_resources"></a>

### list_service_pipeline_provisioned_resources

List provisioned resources for a service and pipeline with details.

Type annotations for
`session.create_client("proton").list_service_pipeline_provisioned_resources`
method.

Boto3 documentation:
[Proton.Client.list_service_pipeline_provisioned_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_provisioned_resources)

Asynchronous method. Use
`await list_service_pipeline_provisioned_resources(...)` for a synchronous
call.

Arguments mapping described in
[ListServicePipelineProvisionedResourcesInputRequestTypeDef](./type_defs.md#listservicepipelineprovisionedresourcesinputrequesttypedef).

Keyword-only arguments:

- `serviceName`: `str` *(required)*
- `nextToken`: `str`

Returns a `Coroutine` for
[ListServicePipelineProvisionedResourcesOutputTypeDef](./type_defs.md#listservicepipelineprovisionedresourcesoutputtypedef).

<a id="list_service_template_versions"></a>

### list_service_template_versions

List major or minor versions of a service template with detail data.

Type annotations for
`session.create_client("proton").list_service_template_versions` method.

Boto3 documentation:
[Proton.Client.list_service_template_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_template_versions)

Asynchronous method. Use `await list_service_template_versions(...)` for a
synchronous call.

Arguments mapping described in
[ListServiceTemplateVersionsInputRequestTypeDef](./type_defs.md#listservicetemplateversionsinputrequesttypedef).

Keyword-only arguments:

- `templateName`: `str` *(required)*
- `majorVersion`: `str`
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListServiceTemplateVersionsOutputTypeDef](./type_defs.md#listservicetemplateversionsoutputtypedef).

<a id="list_service_templates"></a>

### list_service_templates

List service templates with detail data.

Type annotations for `session.create_client("proton").list_service_templates`
method.

Boto3 documentation:
[Proton.Client.list_service_templates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_templates)

Asynchronous method. Use `await list_service_templates(...)` for a synchronous
call.

Arguments mapping described in
[ListServiceTemplatesInputRequestTypeDef](./type_defs.md#listservicetemplatesinputrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListServiceTemplatesOutputTypeDef](./type_defs.md#listservicetemplatesoutputtypedef).

<a id="list_services"></a>

### list_services

List services with summaries of detail data.

Type annotations for `session.create_client("proton").list_services` method.

Boto3 documentation:
[Proton.Client.list_services](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_services)

Asynchronous method. Use `await list_services(...)` for a synchronous call.

Arguments mapping described in
[ListServicesInputRequestTypeDef](./type_defs.md#listservicesinputrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListServicesOutputTypeDef](./type_defs.md#listservicesoutputtypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

List tags for a resource.

Type annotations for `session.create_client("proton").list_tags_for_resource`
method.

Boto3 documentation:
[Proton.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef).

<a id="notify_resource_deployment_status_change"></a>

### notify_resource_deployment_status_change

Notify Proton of status changes to a provisioned resource when you use pull
request provisioning.

Type annotations for
`session.create_client("proton").notify_resource_deployment_status_change`
method.

Boto3 documentation:
[Proton.Client.notify_resource_deployment_status_change](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.notify_resource_deployment_status_change)

Asynchronous method. Use `await notify_resource_deployment_status_change(...)`
for a synchronous call.

Arguments mapping described in
[NotifyResourceDeploymentStatusChangeInputRequestTypeDef](./type_defs.md#notifyresourcedeploymentstatuschangeinputrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `status`:
  [ResourceDeploymentStatusType](./literals.md#resourcedeploymentstatustype)
  *(required)*
- `deploymentId`: `str`
- `outputs`: `Sequence`\[[OutputTypeDef](./type_defs.md#outputtypedef)\]
- `statusMessage`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="reject_environment_account_connection"></a>

### reject_environment_account_connection

In a management account, reject an environment account connection from another
environment account.

Type annotations for
`session.create_client("proton").reject_environment_account_connection` method.

Boto3 documentation:
[Proton.Client.reject_environment_account_connection](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.reject_environment_account_connection)

Asynchronous method. Use `await reject_environment_account_connection(...)` for
a synchronous call.

Arguments mapping described in
[RejectEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#rejectenvironmentaccountconnectioninputrequesttypedef).

Keyword-only arguments:

- `id`: `str` *(required)*

Returns a `Coroutine` for
[RejectEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#rejectenvironmentaccountconnectionoutputtypedef).

<a id="tag_resource"></a>

### tag_resource

Tag a resource.

Type annotations for `session.create_client("proton").tag_resource` method.

Boto3 documentation:
[Proton.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Remove a tag from a resource.

Type annotations for `session.create_client("proton").untag_resource` method.

Boto3 documentation:
[Proton.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_account_settings"></a>

### update_account_settings

Update the Proton service pipeline role or repository settings.

Type annotations for `session.create_client("proton").update_account_settings`
method.

Boto3 documentation:
[Proton.Client.update_account_settings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_account_settings)

Asynchronous method. Use `await update_account_settings(...)` for a synchronous
call.

Arguments mapping described in
[UpdateAccountSettingsInputRequestTypeDef](./type_defs.md#updateaccountsettingsinputrequesttypedef).

Keyword-only arguments:

- `pipelineProvisioningRepository`:
  [RepositoryBranchInputTypeDef](./type_defs.md#repositorybranchinputtypedef)
- `pipelineServiceRoleArn`: `str`

Returns a `Coroutine` for
[UpdateAccountSettingsOutputTypeDef](./type_defs.md#updateaccountsettingsoutputtypedef).

<a id="update_environment"></a>

### update_environment

Update an environment.

Type annotations for `session.create_client("proton").update_environment`
method.

Boto3 documentation:
[Proton.Client.update_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment)

Asynchronous method. Use `await update_environment(...)` for a synchronous
call.

Arguments mapping described in
[UpdateEnvironmentInputRequestTypeDef](./type_defs.md#updateenvironmentinputrequesttypedef).

Keyword-only arguments:

- `deploymentType`:
  [DeploymentUpdateTypeType](./literals.md#deploymentupdatetypetype)
  *(required)*
- `name`: `str` *(required)*
- `description`: `str`
- `environmentAccountConnectionId`: `str`
- `protonServiceRoleArn`: `str`
- `provisioningRepository`:
  [RepositoryBranchInputTypeDef](./type_defs.md#repositorybranchinputtypedef)
- `spec`: `str`
- `templateMajorVersion`: `str`
- `templateMinorVersion`: `str`

Returns a `Coroutine` for
[UpdateEnvironmentOutputTypeDef](./type_defs.md#updateenvironmentoutputtypedef).

<a id="update_environment_account_connection"></a>

### update_environment_account_connection

In an environment account, update an environment account connection to use a
new IAM role.

Type annotations for
`session.create_client("proton").update_environment_account_connection` method.

Boto3 documentation:
[Proton.Client.update_environment_account_connection](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_account_connection)

Asynchronous method. Use `await update_environment_account_connection(...)` for
a synchronous call.

Arguments mapping described in
[UpdateEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#updateenvironmentaccountconnectioninputrequesttypedef).

Keyword-only arguments:

- `id`: `str` *(required)*
- `roleArn`: `str` *(required)*

Returns a `Coroutine` for
[UpdateEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#updateenvironmentaccountconnectionoutputtypedef).

<a id="update_environment_template"></a>

### update_environment_template

Update an environment template.

Type annotations for
`session.create_client("proton").update_environment_template` method.

Boto3 documentation:
[Proton.Client.update_environment_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template)

Asynchronous method. Use `await update_environment_template(...)` for a
synchronous call.

Arguments mapping described in
[UpdateEnvironmentTemplateInputRequestTypeDef](./type_defs.md#updateenvironmenttemplateinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `description`: `str`
- `displayName`: `str`

Returns a `Coroutine` for
[UpdateEnvironmentTemplateOutputTypeDef](./type_defs.md#updateenvironmenttemplateoutputtypedef).

<a id="update_environment_template_version"></a>

### update_environment_template_version

Update a major or minor version of an environment template.

Type annotations for
`session.create_client("proton").update_environment_template_version` method.

Boto3 documentation:
[Proton.Client.update_environment_template_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template_version)

Asynchronous method. Use `await update_environment_template_version(...)` for a
synchronous call.

Arguments mapping described in
[UpdateEnvironmentTemplateVersionInputRequestTypeDef](./type_defs.md#updateenvironmenttemplateversioninputrequesttypedef).

Keyword-only arguments:

- `majorVersion`: `str` *(required)*
- `minorVersion`: `str` *(required)*
- `templateName`: `str` *(required)*
- `description`: `str`
- `status`:
  [TemplateVersionStatusType](./literals.md#templateversionstatustype)

Returns a `Coroutine` for
[UpdateEnvironmentTemplateVersionOutputTypeDef](./type_defs.md#updateenvironmenttemplateversionoutputtypedef).

<a id="update_service"></a>

### update_service

Edit a service description or use a spec to add and delete service instances.

Type annotations for `session.create_client("proton").update_service` method.

Boto3 documentation:
[Proton.Client.update_service](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service)

Asynchronous method. Use `await update_service(...)` for a synchronous call.

Arguments mapping described in
[UpdateServiceInputRequestTypeDef](./type_defs.md#updateserviceinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `description`: `str`
- `spec`: `str`

Returns a `Coroutine` for
[UpdateServiceOutputTypeDef](./type_defs.md#updateserviceoutputtypedef).

<a id="update_service_instance"></a>

### update_service_instance

Update a service instance.

Type annotations for `session.create_client("proton").update_service_instance`
method.

Boto3 documentation:
[Proton.Client.update_service_instance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_instance)

Asynchronous method. Use `await update_service_instance(...)` for a synchronous
call.

Arguments mapping described in
[UpdateServiceInstanceInputRequestTypeDef](./type_defs.md#updateserviceinstanceinputrequesttypedef).

Keyword-only arguments:

- `deploymentType`:
  [DeploymentUpdateTypeType](./literals.md#deploymentupdatetypetype)
  *(required)*
- `name`: `str` *(required)*
- `serviceName`: `str` *(required)*
- `spec`: `str`
- `templateMajorVersion`: `str`
- `templateMinorVersion`: `str`

Returns a `Coroutine` for
[UpdateServiceInstanceOutputTypeDef](./type_defs.md#updateserviceinstanceoutputtypedef).

<a id="update_service_pipeline"></a>

### update_service_pipeline

Update the service pipeline.

Type annotations for `session.create_client("proton").update_service_pipeline`
method.

Boto3 documentation:
[Proton.Client.update_service_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_pipeline)

Asynchronous method. Use `await update_service_pipeline(...)` for a synchronous
call.

Arguments mapping described in
[UpdateServicePipelineInputRequestTypeDef](./type_defs.md#updateservicepipelineinputrequesttypedef).

Keyword-only arguments:

- `deploymentType`:
  [DeploymentUpdateTypeType](./literals.md#deploymentupdatetypetype)
  *(required)*
- `serviceName`: `str` *(required)*
- `spec`: `str` *(required)*
- `templateMajorVersion`: `str`
- `templateMinorVersion`: `str`

Returns a `Coroutine` for
[UpdateServicePipelineOutputTypeDef](./type_defs.md#updateservicepipelineoutputtypedef).

<a id="update_service_template"></a>

### update_service_template

Update a service template.

Type annotations for `session.create_client("proton").update_service_template`
method.

Boto3 documentation:
[Proton.Client.update_service_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template)

Asynchronous method. Use `await update_service_template(...)` for a synchronous
call.

Arguments mapping described in
[UpdateServiceTemplateInputRequestTypeDef](./type_defs.md#updateservicetemplateinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `description`: `str`
- `displayName`: `str`

Returns a `Coroutine` for
[UpdateServiceTemplateOutputTypeDef](./type_defs.md#updateservicetemplateoutputtypedef).

<a id="update_service_template_version"></a>

### update_service_template_version

Update a major or minor version of a service template.

Type annotations for
`session.create_client("proton").update_service_template_version` method.

Boto3 documentation:
[Proton.Client.update_service_template_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template_version)

Asynchronous method. Use `await update_service_template_version(...)` for a
synchronous call.

Arguments mapping described in
[UpdateServiceTemplateVersionInputRequestTypeDef](./type_defs.md#updateservicetemplateversioninputrequesttypedef).

Keyword-only arguments:

- `majorVersion`: `str` *(required)*
- `minorVersion`: `str` *(required)*
- `templateName`: `str` *(required)*
- `compatibleEnvironmentTemplates`:
  `Sequence`\[[CompatibleEnvironmentTemplateInputTypeDef](./type_defs.md#compatibleenvironmenttemplateinputtypedef)\]
- `description`: `str`
- `status`:
  [TemplateVersionStatusType](./literals.md#templateversionstatustype)

Returns a `Coroutine` for
[UpdateServiceTemplateVersionOutputTypeDef](./type_defs.md#updateservicetemplateversionoutputtypedef).

<a id="update_template_sync_config"></a>

### update_template_sync_config

Update template sync configuration parameters, except for the `templateName`
and `templateType` .

Type annotations for
`session.create_client("proton").update_template_sync_config` method.

Boto3 documentation:
[Proton.Client.update_template_sync_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_template_sync_config)

Asynchronous method. Use `await update_template_sync_config(...)` for a
synchronous call.

Arguments mapping described in
[UpdateTemplateSyncConfigInputRequestTypeDef](./type_defs.md#updatetemplatesyncconfiginputrequesttypedef).

Keyword-only arguments:

- `branch`: `str` *(required)*
- `repositoryName`: `str` *(required)*
- `repositoryProvider`:
  [RepositoryProviderType](./literals.md#repositoryprovidertype) *(required)*
- `templateName`: `str` *(required)*
- `templateType`: [TemplateTypeType](./literals.md#templatetypetype)
  *(required)*
- `subdirectory`: `str`

Returns a `Coroutine` for
[UpdateTemplateSyncConfigOutputTypeDef](./type_defs.md#updatetemplatesyncconfigoutputtypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("proton").__aenter__` method.

Boto3 documentation:
[Proton.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [ProtonClient](#protonclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("proton").__aexit__` method.

Boto3 documentation:
[Proton.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("proton").get_paginator` method
with overloads.

- `client.get_paginator("list_environment_account_connections")` ->
  [ListEnvironmentAccountConnectionsPaginator](./paginators.md#listenvironmentaccountconnectionspaginator)
- `client.get_paginator("list_environment_outputs")` ->
  [ListEnvironmentOutputsPaginator](./paginators.md#listenvironmentoutputspaginator)
- `client.get_paginator("list_environment_provisioned_resources")` ->
  [ListEnvironmentProvisionedResourcesPaginator](./paginators.md#listenvironmentprovisionedresourcespaginator)
- `client.get_paginator("list_environment_template_versions")` ->
  [ListEnvironmentTemplateVersionsPaginator](./paginators.md#listenvironmenttemplateversionspaginator)
- `client.get_paginator("list_environment_templates")` ->
  [ListEnvironmentTemplatesPaginator](./paginators.md#listenvironmenttemplatespaginator)
- `client.get_paginator("list_environments")` ->
  [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
- `client.get_paginator("list_repositories")` ->
  [ListRepositoriesPaginator](./paginators.md#listrepositoriespaginator)
- `client.get_paginator("list_repository_sync_definitions")` ->
  [ListRepositorySyncDefinitionsPaginator](./paginators.md#listrepositorysyncdefinitionspaginator)
- `client.get_paginator("list_service_instance_outputs")` ->
  [ListServiceInstanceOutputsPaginator](./paginators.md#listserviceinstanceoutputspaginator)
- `client.get_paginator("list_service_instance_provisioned_resources")` ->
  [ListServiceInstanceProvisionedResourcesPaginator](./paginators.md#listserviceinstanceprovisionedresourcespaginator)
- `client.get_paginator("list_service_instances")` ->
  [ListServiceInstancesPaginator](./paginators.md#listserviceinstancespaginator)
- `client.get_paginator("list_service_pipeline_outputs")` ->
  [ListServicePipelineOutputsPaginator](./paginators.md#listservicepipelineoutputspaginator)
- `client.get_paginator("list_service_pipeline_provisioned_resources")` ->
  [ListServicePipelineProvisionedResourcesPaginator](./paginators.md#listservicepipelineprovisionedresourcespaginator)
- `client.get_paginator("list_service_template_versions")` ->
  [ListServiceTemplateVersionsPaginator](./paginators.md#listservicetemplateversionspaginator)
- `client.get_paginator("list_service_templates")` ->
  [ListServiceTemplatesPaginator](./paginators.md#listservicetemplatespaginator)
- `client.get_paginator("list_services")` ->
  [ListServicesPaginator](./paginators.md#listservicespaginator)
- `client.get_paginator("list_tags_for_resource")` ->
  [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("proton").get_waiter` method with
overloads.

- `client.get_waiter("environment_deployed")` ->
  [EnvironmentDeployedWaiter](./waiters.md#environmentdeployedwaiter)
- `client.get_waiter("environment_template_version_registered")` ->
  [EnvironmentTemplateVersionRegisteredWaiter](./waiters.md#environmenttemplateversionregisteredwaiter)
- `client.get_waiter("service_created")` ->
  [ServiceCreatedWaiter](./waiters.md#servicecreatedwaiter)
- `client.get_waiter("service_deleted")` ->
  [ServiceDeletedWaiter](./waiters.md#servicedeletedwaiter)
- `client.get_waiter("service_instance_deployed")` ->
  [ServiceInstanceDeployedWaiter](./waiters.md#serviceinstancedeployedwaiter)
- `client.get_waiter("service_pipeline_deployed")` ->
  [ServicePipelineDeployedWaiter](./waiters.md#servicepipelinedeployedwaiter)
- `client.get_waiter("service_template_version_registered")` ->
  [ServiceTemplateVersionRegisteredWaiter](./waiters.md#servicetemplateversionregisteredwaiter)
- `client.get_waiter("service_updated")` ->
  [ServiceUpdatedWaiter](./waiters.md#serviceupdatedwaiter)
