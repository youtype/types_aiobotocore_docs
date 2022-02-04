<a id="appconfigclient-for-aiobotocore-appconfig-module"></a>

# AppConfigClient for aiobotocore AppConfig module

> [Index](..) > [AppConfig](.) > AppConfigClient

Auto-generated documentation for
[AppConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
type annotations stubs module
[types-aiobotocore-appconfig](https://pypi.org/project/types-aiobotocore-appconfig/).

- [AppConfigClient for aiobotocore AppConfig module](#appconfigclient-for-aiobotocore-appconfig-module)
  - [AppConfigClient](#appconfigclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_application](#create_application)
    - [create_configuration_profile](#create_configuration_profile)
    - [create_deployment_strategy](#create_deployment_strategy)
    - [create_environment](#create_environment)
    - [create_hosted_configuration_version](#create_hosted_configuration_version)
    - [delete_application](#delete_application)
    - [delete_configuration_profile](#delete_configuration_profile)
    - [delete_deployment_strategy](#delete_deployment_strategy)
    - [delete_environment](#delete_environment)
    - [delete_hosted_configuration_version](#delete_hosted_configuration_version)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_application](#get_application)
    - [get_configuration](#get_configuration)
    - [get_configuration_profile](#get_configuration_profile)
    - [get_deployment](#get_deployment)
    - [get_deployment_strategy](#get_deployment_strategy)
    - [get_environment](#get_environment)
    - [get_hosted_configuration_version](#get_hosted_configuration_version)
    - [list_applications](#list_applications)
    - [list_configuration_profiles](#list_configuration_profiles)
    - [list_deployment_strategies](#list_deployment_strategies)
    - [list_deployments](#list_deployments)
    - [list_environments](#list_environments)
    - [list_hosted_configuration_versions](#list_hosted_configuration_versions)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [start_deployment](#start_deployment)
    - [stop_deployment](#stop_deployment)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_application](#update_application)
    - [update_configuration_profile](#update_configuration_profile)
    - [update_deployment_strategy](#update_deployment_strategy)
    - [update_environment](#update_environment)
    - [validate_configuration](#validate_configuration)

<a id="appconfigclient"></a>

## AppConfigClient

Type annotations for `aiobotocore.create_client("appconfig")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_appconfig.client import AppConfigClient

def get_appconfig_client() -> AppConfigClient:
    return Session().client("appconfig")
```

Boto3 documentation:
[AppConfig.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_appconfig.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.PayloadTooLargeException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

AppConfigClient exceptions.

Type annotations for `aiobotocore.create_client("appconfig").exceptions`
method.

Boto3 documentation:
[AppConfig.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("appconfig").can_paginate`
method.

Boto3 documentation:
[AppConfig.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_application"></a>

### create_application

Creates an application.

Type annotations for
`aiobotocore.create_client("appconfig").create_application` method.

Boto3 documentation:
[AppConfig.Client.create_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_application)

Asynchronous method. Use `await create_application(...)` for a synchronous
call.

Arguments mapping described in
[CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Description`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[ApplicationResponseMetadataTypeDef](./type_defs.md#applicationresponsemetadatatypedef).

<a id="create_configuration_profile"></a>

### create_configuration_profile

Creates a configuration profile, which is information that enables AppConfig to
access the configuration source.

Type annotations for
`aiobotocore.create_client("appconfig").create_configuration_profile` method.

Boto3 documentation:
[AppConfig.Client.create_configuration_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_configuration_profile)

Asynchronous method. Use `await create_configuration_profile(...)` for a
synchronous call.

Arguments mapping described in
[CreateConfigurationProfileRequestRequestTypeDef](./type_defs.md#createconfigurationprofilerequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `Name`: `str` *(required)*
- `LocationUri`: `str` *(required)*
- `Description`: `str`
- `RetrievalRoleArn`: `str`
- `Validators`:
  `Sequence`\[[ValidatorTypeDef](./type_defs.md#validatortypedef)\]
- `Tags`: `Mapping`\[`str`, `str`\]
- `Type`: `str`

Returns a `Coroutine` for
[ConfigurationProfileTypeDef](./type_defs.md#configurationprofiletypedef).

<a id="create_deployment_strategy"></a>

### create_deployment_strategy

Creates a deployment strategy that defines important criteria for rolling out
your configuration to the designated targets.

Type annotations for
`aiobotocore.create_client("appconfig").create_deployment_strategy` method.

Boto3 documentation:
[AppConfig.Client.create_deployment_strategy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_deployment_strategy)

Asynchronous method. Use `await create_deployment_strategy(...)` for a
synchronous call.

Arguments mapping described in
[CreateDeploymentStrategyRequestRequestTypeDef](./type_defs.md#createdeploymentstrategyrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `DeploymentDurationInMinutes`: `int` *(required)*
- `GrowthFactor`: `float` *(required)*
- `ReplicateTo`: [ReplicateToType](./literals.md#replicatetotype) *(required)*
- `Description`: `str`
- `FinalBakeTimeInMinutes`: `int`
- `GrowthType`: [GrowthTypeType](./literals.md#growthtypetype)
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[DeploymentStrategyResponseMetadataTypeDef](./type_defs.md#deploymentstrategyresponsemetadatatypedef).

<a id="create_environment"></a>

### create_environment

Creates an environment.

Type annotations for
`aiobotocore.create_client("appconfig").create_environment` method.

Boto3 documentation:
[AppConfig.Client.create_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_environment)

Asynchronous method. Use `await create_environment(...)` for a synchronous
call.

Arguments mapping described in
[CreateEnvironmentRequestRequestTypeDef](./type_defs.md#createenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `Name`: `str` *(required)*
- `Description`: `str`
- `Monitors`: `Sequence`\[[MonitorTypeDef](./type_defs.md#monitortypedef)\]
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[EnvironmentResponseMetadataTypeDef](./type_defs.md#environmentresponsemetadatatypedef).

<a id="create_hosted_configuration_version"></a>

### create_hosted_configuration_version

Creates a new configuration in the AppConfig hosted configuration store.

Type annotations for
`aiobotocore.create_client("appconfig").create_hosted_configuration_version`
method.

Boto3 documentation:
[AppConfig.Client.create_hosted_configuration_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_hosted_configuration_version)

Asynchronous method. Use `await create_hosted_configuration_version(...)` for a
synchronous call.

Arguments mapping described in
[CreateHostedConfigurationVersionRequestRequestTypeDef](./type_defs.md#createhostedconfigurationversionrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `ConfigurationProfileId`: `str` *(required)*
- `Content`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\] *(required)*
- `ContentType`: `str` *(required)*
- `Description`: `str`
- `LatestVersionNumber`: `int`

Returns a `Coroutine` for
[HostedConfigurationVersionTypeDef](./type_defs.md#hostedconfigurationversiontypedef).

<a id="delete_application"></a>

### delete_application

Deletes an application.

Type annotations for
`aiobotocore.create_client("appconfig").delete_application` method.

Boto3 documentation:
[AppConfig.Client.delete_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.delete_application)

Asynchronous method. Use `await delete_application(...)` for a synchronous
call.

Arguments mapping described in
[DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

<a id="delete_configuration_profile"></a>

### delete_configuration_profile

Deletes a configuration profile.

Type annotations for
`aiobotocore.create_client("appconfig").delete_configuration_profile` method.

Boto3 documentation:
[AppConfig.Client.delete_configuration_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.delete_configuration_profile)

Asynchronous method. Use `await delete_configuration_profile(...)` for a
synchronous call.

Arguments mapping described in
[DeleteConfigurationProfileRequestRequestTypeDef](./type_defs.md#deleteconfigurationprofilerequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `ConfigurationProfileId`: `str` *(required)*

<a id="delete_deployment_strategy"></a>

### delete_deployment_strategy

Deletes a deployment strategy.

Type annotations for
`aiobotocore.create_client("appconfig").delete_deployment_strategy` method.

Boto3 documentation:
[AppConfig.Client.delete_deployment_strategy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.delete_deployment_strategy)

Asynchronous method. Use `await delete_deployment_strategy(...)` for a
synchronous call.

Arguments mapping described in
[DeleteDeploymentStrategyRequestRequestTypeDef](./type_defs.md#deletedeploymentstrategyrequestrequesttypedef).

Keyword-only arguments:

- `DeploymentStrategyId`: `str` *(required)*

<a id="delete_environment"></a>

### delete_environment

Deletes an environment.

Type annotations for
`aiobotocore.create_client("appconfig").delete_environment` method.

Boto3 documentation:
[AppConfig.Client.delete_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.delete_environment)

Asynchronous method. Use `await delete_environment(...)` for a synchronous
call.

Arguments mapping described in
[DeleteEnvironmentRequestRequestTypeDef](./type_defs.md#deleteenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EnvironmentId`: `str` *(required)*

<a id="delete_hosted_configuration_version"></a>

### delete_hosted_configuration_version

Deletes a version of a configuration from the AppConfig hosted configuration
store.

Type annotations for
`aiobotocore.create_client("appconfig").delete_hosted_configuration_version`
method.

Boto3 documentation:
[AppConfig.Client.delete_hosted_configuration_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.delete_hosted_configuration_version)

Asynchronous method. Use `await delete_hosted_configuration_version(...)` for a
synchronous call.

Arguments mapping described in
[DeleteHostedConfigurationVersionRequestRequestTypeDef](./type_defs.md#deletehostedconfigurationversionrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `ConfigurationProfileId`: `str` *(required)*
- `VersionNumber`: `int` *(required)*

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("appconfig").generate_presigned_url` method.

Boto3 documentation:
[AppConfig.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_application"></a>

### get_application

Retrieves information about an application.

Type annotations for `aiobotocore.create_client("appconfig").get_application`
method.

Boto3 documentation:
[AppConfig.Client.get_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_application)

Asynchronous method. Use `await get_application(...)` for a synchronous call.

Arguments mapping described in
[GetApplicationRequestRequestTypeDef](./type_defs.md#getapplicationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[ApplicationResponseMetadataTypeDef](./type_defs.md#applicationresponsemetadatatypedef).

<a id="get_configuration"></a>

### get_configuration

Retrieves information about a configuration.

Type annotations for `aiobotocore.create_client("appconfig").get_configuration`
method.

Boto3 documentation:
[AppConfig.Client.get_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_configuration)

Asynchronous method. Use `await get_configuration(...)` for a synchronous call.

Arguments mapping described in
[GetConfigurationRequestRequestTypeDef](./type_defs.md#getconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `Application`: `str` *(required)*
- `Environment`: `str` *(required)*
- `Configuration`: `str` *(required)*
- `ClientId`: `str` *(required)*
- `ClientConfigurationVersion`: `str`

Returns a `Coroutine` for
[ConfigurationTypeDef](./type_defs.md#configurationtypedef).

<a id="get_configuration_profile"></a>

### get_configuration_profile

Retrieves information about a configuration profile.

Type annotations for
`aiobotocore.create_client("appconfig").get_configuration_profile` method.

Boto3 documentation:
[AppConfig.Client.get_configuration_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_configuration_profile)

Asynchronous method. Use `await get_configuration_profile(...)` for a
synchronous call.

Arguments mapping described in
[GetConfigurationProfileRequestRequestTypeDef](./type_defs.md#getconfigurationprofilerequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `ConfigurationProfileId`: `str` *(required)*

Returns a `Coroutine` for
[ConfigurationProfileTypeDef](./type_defs.md#configurationprofiletypedef).

<a id="get_deployment"></a>

### get_deployment

Retrieves information about a configuration deployment.

Type annotations for `aiobotocore.create_client("appconfig").get_deployment`
method.

Boto3 documentation:
[AppConfig.Client.get_deployment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_deployment)

Asynchronous method. Use `await get_deployment(...)` for a synchronous call.

Arguments mapping described in
[GetDeploymentRequestRequestTypeDef](./type_defs.md#getdeploymentrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EnvironmentId`: `str` *(required)*
- `DeploymentNumber`: `int` *(required)*

Returns a `Coroutine` for
[DeploymentTypeDef](./type_defs.md#deploymenttypedef).

<a id="get_deployment_strategy"></a>

### get_deployment_strategy

Retrieves information about a deployment strategy.

Type annotations for
`aiobotocore.create_client("appconfig").get_deployment_strategy` method.

Boto3 documentation:
[AppConfig.Client.get_deployment_strategy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_deployment_strategy)

Asynchronous method. Use `await get_deployment_strategy(...)` for a synchronous
call.

Arguments mapping described in
[GetDeploymentStrategyRequestRequestTypeDef](./type_defs.md#getdeploymentstrategyrequestrequesttypedef).

Keyword-only arguments:

- `DeploymentStrategyId`: `str` *(required)*

Returns a `Coroutine` for
[DeploymentStrategyResponseMetadataTypeDef](./type_defs.md#deploymentstrategyresponsemetadatatypedef).

<a id="get_environment"></a>

### get_environment

Retrieves information about an environment.

Type annotations for `aiobotocore.create_client("appconfig").get_environment`
method.

Boto3 documentation:
[AppConfig.Client.get_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_environment)

Asynchronous method. Use `await get_environment(...)` for a synchronous call.

Arguments mapping described in
[GetEnvironmentRequestRequestTypeDef](./type_defs.md#getenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EnvironmentId`: `str` *(required)*

Returns a `Coroutine` for
[EnvironmentResponseMetadataTypeDef](./type_defs.md#environmentresponsemetadatatypedef).

<a id="get_hosted_configuration_version"></a>

### get_hosted_configuration_version

Retrieves information about a specific configuration version.

Type annotations for
`aiobotocore.create_client("appconfig").get_hosted_configuration_version`
method.

Boto3 documentation:
[AppConfig.Client.get_hosted_configuration_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_hosted_configuration_version)

Asynchronous method. Use `await get_hosted_configuration_version(...)` for a
synchronous call.

Arguments mapping described in
[GetHostedConfigurationVersionRequestRequestTypeDef](./type_defs.md#gethostedconfigurationversionrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `ConfigurationProfileId`: `str` *(required)*
- `VersionNumber`: `int` *(required)*

Returns a `Coroutine` for
[HostedConfigurationVersionTypeDef](./type_defs.md#hostedconfigurationversiontypedef).

<a id="list_applications"></a>

### list_applications

Lists all applications in your Amazon Web Services account.

Type annotations for `aiobotocore.create_client("appconfig").list_applications`
method.

Boto3 documentation:
[AppConfig.Client.list_applications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.list_applications)

Asynchronous method. Use `await list_applications(...)` for a synchronous call.

Arguments mapping described in
[ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ApplicationsTypeDef](./type_defs.md#applicationstypedef).

<a id="list_configuration_profiles"></a>

### list_configuration_profiles

Lists the configuration profiles for an application.

Type annotations for
`aiobotocore.create_client("appconfig").list_configuration_profiles` method.

Boto3 documentation:
[AppConfig.Client.list_configuration_profiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.list_configuration_profiles)

Asynchronous method. Use `await list_configuration_profiles(...)` for a
synchronous call.

Arguments mapping described in
[ListConfigurationProfilesRequestRequestTypeDef](./type_defs.md#listconfigurationprofilesrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`
- `Type`: `str`

Returns a `Coroutine` for
[ConfigurationProfilesTypeDef](./type_defs.md#configurationprofilestypedef).

<a id="list_deployment_strategies"></a>

### list_deployment_strategies

Lists deployment strategies.

Type annotations for
`aiobotocore.create_client("appconfig").list_deployment_strategies` method.

Boto3 documentation:
[AppConfig.Client.list_deployment_strategies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.list_deployment_strategies)

Asynchronous method. Use `await list_deployment_strategies(...)` for a
synchronous call.

Arguments mapping described in
[ListDeploymentStrategiesRequestRequestTypeDef](./type_defs.md#listdeploymentstrategiesrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DeploymentStrategiesTypeDef](./type_defs.md#deploymentstrategiestypedef).

<a id="list_deployments"></a>

### list_deployments

Lists the deployments for an environment.

Type annotations for `aiobotocore.create_client("appconfig").list_deployments`
method.

Boto3 documentation:
[AppConfig.Client.list_deployments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.list_deployments)

Asynchronous method. Use `await list_deployments(...)` for a synchronous call.

Arguments mapping described in
[ListDeploymentsRequestRequestTypeDef](./type_defs.md#listdeploymentsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EnvironmentId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DeploymentsTypeDef](./type_defs.md#deploymentstypedef).

<a id="list_environments"></a>

### list_environments

Lists the environments for an application.

Type annotations for `aiobotocore.create_client("appconfig").list_environments`
method.

Boto3 documentation:
[AppConfig.Client.list_environments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.list_environments)

Asynchronous method. Use `await list_environments(...)` for a synchronous call.

Arguments mapping described in
[ListEnvironmentsRequestRequestTypeDef](./type_defs.md#listenvironmentsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[EnvironmentsTypeDef](./type_defs.md#environmentstypedef).

<a id="list_hosted_configuration_versions"></a>

### list_hosted_configuration_versions

Lists configurations stored in the AppConfig hosted configuration store by
version.

Type annotations for
`aiobotocore.create_client("appconfig").list_hosted_configuration_versions`
method.

Boto3 documentation:
[AppConfig.Client.list_hosted_configuration_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.list_hosted_configuration_versions)

Asynchronous method. Use `await list_hosted_configuration_versions(...)` for a
synchronous call.

Arguments mapping described in
[ListHostedConfigurationVersionsRequestRequestTypeDef](./type_defs.md#listhostedconfigurationversionsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `ConfigurationProfileId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[HostedConfigurationVersionsTypeDef](./type_defs.md#hostedconfigurationversionstypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Retrieves the list of key-value tags assigned to the resource.

Type annotations for
`aiobotocore.create_client("appconfig").list_tags_for_resource` method.

Boto3 documentation:
[AppConfig.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ResourceTagsTypeDef](./type_defs.md#resourcetagstypedef).

<a id="start_deployment"></a>

### start_deployment

Starts a deployment.

Type annotations for `aiobotocore.create_client("appconfig").start_deployment`
method.

Boto3 documentation:
[AppConfig.Client.start_deployment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.start_deployment)

Asynchronous method. Use `await start_deployment(...)` for a synchronous call.

Arguments mapping described in
[StartDeploymentRequestRequestTypeDef](./type_defs.md#startdeploymentrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EnvironmentId`: `str` *(required)*
- `DeploymentStrategyId`: `str` *(required)*
- `ConfigurationProfileId`: `str` *(required)*
- `ConfigurationVersion`: `str` *(required)*
- `Description`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[DeploymentTypeDef](./type_defs.md#deploymenttypedef).

<a id="stop_deployment"></a>

### stop_deployment

Stops a deployment.

Type annotations for `aiobotocore.create_client("appconfig").stop_deployment`
method.

Boto3 documentation:
[AppConfig.Client.stop_deployment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.stop_deployment)

Asynchronous method. Use `await stop_deployment(...)` for a synchronous call.

Arguments mapping described in
[StopDeploymentRequestRequestTypeDef](./type_defs.md#stopdeploymentrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EnvironmentId`: `str` *(required)*
- `DeploymentNumber`: `int` *(required)*

Returns a `Coroutine` for
[DeploymentTypeDef](./type_defs.md#deploymenttypedef).

<a id="tag_resource"></a>

### tag_resource

Assigns metadata to an AppConfig resource.

Type annotations for `aiobotocore.create_client("appconfig").tag_resource`
method.

Boto3 documentation:
[AppConfig.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

<a id="untag_resource"></a>

### untag_resource

Deletes a tag key and value from an AppConfig resource.

Type annotations for `aiobotocore.create_client("appconfig").untag_resource`
method.

Boto3 documentation:
[AppConfig.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

<a id="update_application"></a>

### update_application

Updates an application.

Type annotations for
`aiobotocore.create_client("appconfig").update_application` method.

Boto3 documentation:
[AppConfig.Client.update_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_application)

Asynchronous method. Use `await update_application(...)` for a synchronous
call.

Arguments mapping described in
[UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `Name`: `str`
- `Description`: `str`

Returns a `Coroutine` for
[ApplicationResponseMetadataTypeDef](./type_defs.md#applicationresponsemetadatatypedef).

<a id="update_configuration_profile"></a>

### update_configuration_profile

Updates a configuration profile.

Type annotations for
`aiobotocore.create_client("appconfig").update_configuration_profile` method.

Boto3 documentation:
[AppConfig.Client.update_configuration_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_configuration_profile)

Asynchronous method. Use `await update_configuration_profile(...)` for a
synchronous call.

Arguments mapping described in
[UpdateConfigurationProfileRequestRequestTypeDef](./type_defs.md#updateconfigurationprofilerequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `ConfigurationProfileId`: `str` *(required)*
- `Name`: `str`
- `Description`: `str`
- `RetrievalRoleArn`: `str`
- `Validators`:
  `Sequence`\[[ValidatorTypeDef](./type_defs.md#validatortypedef)\]

Returns a `Coroutine` for
[ConfigurationProfileTypeDef](./type_defs.md#configurationprofiletypedef).

<a id="update_deployment_strategy"></a>

### update_deployment_strategy

Updates a deployment strategy.

Type annotations for
`aiobotocore.create_client("appconfig").update_deployment_strategy` method.

Boto3 documentation:
[AppConfig.Client.update_deployment_strategy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_deployment_strategy)

Asynchronous method. Use `await update_deployment_strategy(...)` for a
synchronous call.

Arguments mapping described in
[UpdateDeploymentStrategyRequestRequestTypeDef](./type_defs.md#updatedeploymentstrategyrequestrequesttypedef).

Keyword-only arguments:

- `DeploymentStrategyId`: `str` *(required)*
- `Description`: `str`
- `DeploymentDurationInMinutes`: `int`
- `FinalBakeTimeInMinutes`: `int`
- `GrowthFactor`: `float`
- `GrowthType`: [GrowthTypeType](./literals.md#growthtypetype)

Returns a `Coroutine` for
[DeploymentStrategyResponseMetadataTypeDef](./type_defs.md#deploymentstrategyresponsemetadatatypedef).

<a id="update_environment"></a>

### update_environment

Updates an environment.

Type annotations for
`aiobotocore.create_client("appconfig").update_environment` method.

Boto3 documentation:
[AppConfig.Client.update_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_environment)

Asynchronous method. Use `await update_environment(...)` for a synchronous
call.

Arguments mapping described in
[UpdateEnvironmentRequestRequestTypeDef](./type_defs.md#updateenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `EnvironmentId`: `str` *(required)*
- `Name`: `str`
- `Description`: `str`
- `Monitors`: `Sequence`\[[MonitorTypeDef](./type_defs.md#monitortypedef)\]

Returns a `Coroutine` for
[EnvironmentResponseMetadataTypeDef](./type_defs.md#environmentresponsemetadatatypedef).

<a id="validate_configuration"></a>

### validate_configuration

Uses the validators in a configuration profile to validate a configuration.

Type annotations for
`aiobotocore.create_client("appconfig").validate_configuration` method.

Boto3 documentation:
[AppConfig.Client.validate_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.validate_configuration)

Asynchronous method. Use `await validate_configuration(...)` for a synchronous
call.

Arguments mapping described in
[ValidateConfigurationRequestRequestTypeDef](./type_defs.md#validateconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `ConfigurationProfileId`: `str` *(required)*
- `ConfigurationVersion`: `str` *(required)*
