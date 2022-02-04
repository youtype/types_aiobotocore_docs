<a id="amplifyclient-for-aiobotocore-amplify-module"></a>

# AmplifyClient for aiobotocore Amplify module

> [Index](..) > [Amplify](.) > AmplifyClient

Auto-generated documentation for
[Amplify](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
type annotations stubs module
[types-aiobotocore-amplify](https://pypi.org/project/types-aiobotocore-amplify/).

- [AmplifyClient for aiobotocore Amplify module](#amplifyclient-for-aiobotocore-amplify-module)
  - [AmplifyClient](#amplifyclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_app](#create_app)
    - [create_backend_environment](#create_backend_environment)
    - [create_branch](#create_branch)
    - [create_deployment](#create_deployment)
    - [create_domain_association](#create_domain_association)
    - [create_webhook](#create_webhook)
    - [delete_app](#delete_app)
    - [delete_backend_environment](#delete_backend_environment)
    - [delete_branch](#delete_branch)
    - [delete_domain_association](#delete_domain_association)
    - [delete_job](#delete_job)
    - [delete_webhook](#delete_webhook)
    - [generate_access_logs](#generate_access_logs)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_app](#get_app)
    - [get_artifact_url](#get_artifact_url)
    - [get_backend_environment](#get_backend_environment)
    - [get_branch](#get_branch)
    - [get_domain_association](#get_domain_association)
    - [get_job](#get_job)
    - [get_webhook](#get_webhook)
    - [list_apps](#list_apps)
    - [list_artifacts](#list_artifacts)
    - [list_backend_environments](#list_backend_environments)
    - [list_branches](#list_branches)
    - [list_domain_associations](#list_domain_associations)
    - [list_jobs](#list_jobs)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_webhooks](#list_webhooks)
    - [start_deployment](#start_deployment)
    - [start_job](#start_job)
    - [stop_job](#stop_job)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_app](#update_app)
    - [update_branch](#update_branch)
    - [update_domain_association](#update_domain_association)
    - [update_webhook](#update_webhook)
    - [get_paginator](#get_paginator)

<a id="amplifyclient"></a>

## AmplifyClient

Type annotations for `aiobotocore.create_client("amplify")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_amplify.client import AmplifyClient

def get_amplify_client() -> AmplifyClient:
    return Session().client("amplify")
```

Boto3 documentation:
[Amplify.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_amplify.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.DependentServiceFailureException`
- `Exceptions.InternalFailureException`
- `Exceptions.LimitExceededException`
- `Exceptions.NotFoundException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.UnauthorizedException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

AmplifyClient exceptions.

Type annotations for `aiobotocore.create_client("amplify").exceptions` method.

Boto3 documentation:
[Amplify.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("amplify").can_paginate`
method.

Boto3 documentation:
[Amplify.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_app"></a>

### create_app

Creates a new Amplify app.

Type annotations for `aiobotocore.create_client("amplify").create_app` method.

Boto3 documentation:
[Amplify.Client.create_app](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_app)

Asynchronous method. Use `await create_app(...)` for a synchronous call.

Arguments mapping described in
[CreateAppRequestRequestTypeDef](./type_defs.md#createapprequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `description`: `str`
- `repository`: `str`
- `platform`: `Literal['WEB']` (see [PlatformType](./literals.md#platformtype))
- `iamServiceRoleArn`: `str`
- `oauthToken`: `str`
- `accessToken`: `str`
- `environmentVariables`: `Mapping`\[`str`, `str`\]
- `enableBranchAutoBuild`: `bool`
- `enableBranchAutoDeletion`: `bool`
- `enableBasicAuth`: `bool`
- `basicAuthCredentials`: `str`
- `customRules`:
  `Sequence`\[[CustomRuleTypeDef](./type_defs.md#customruletypedef)\]
- `tags`: `Mapping`\[`str`, `str`\]
- `buildSpec`: `str`
- `customHeaders`: `str`
- `enableAutoBranchCreation`: `bool`
- `autoBranchCreationPatterns`: `Sequence`\[`str`\]
- `autoBranchCreationConfig`:
  [AutoBranchCreationConfigTypeDef](./type_defs.md#autobranchcreationconfigtypedef)

Returns a `Coroutine` for
[CreateAppResultTypeDef](./type_defs.md#createappresulttypedef).

<a id="create_backend_environment"></a>

### create_backend_environment

Creates a new backend environment for an Amplify app.

Type annotations for
`aiobotocore.create_client("amplify").create_backend_environment` method.

Boto3 documentation:
[Amplify.Client.create_backend_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_backend_environment)

Asynchronous method. Use `await create_backend_environment(...)` for a
synchronous call.

Arguments mapping described in
[CreateBackendEnvironmentRequestRequestTypeDef](./type_defs.md#createbackendenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `stackName`: `str`
- `deploymentArtifacts`: `str`

Returns a `Coroutine` for
[CreateBackendEnvironmentResultTypeDef](./type_defs.md#createbackendenvironmentresulttypedef).

<a id="create_branch"></a>

### create_branch

Creates a new branch for an Amplify app.

Type annotations for `aiobotocore.create_client("amplify").create_branch`
method.

Boto3 documentation:
[Amplify.Client.create_branch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_branch)

Asynchronous method. Use `await create_branch(...)` for a synchronous call.

Arguments mapping described in
[CreateBranchRequestRequestTypeDef](./type_defs.md#createbranchrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*
- `description`: `str`
- `stage`: [StageType](./literals.md#stagetype)
- `framework`: `str`
- `enableNotification`: `bool`
- `enableAutoBuild`: `bool`
- `environmentVariables`: `Mapping`\[`str`, `str`\]
- `basicAuthCredentials`: `str`
- `enableBasicAuth`: `bool`
- `enablePerformanceMode`: `bool`
- `tags`: `Mapping`\[`str`, `str`\]
- `buildSpec`: `str`
- `ttl`: `str`
- `displayName`: `str`
- `enablePullRequestPreview`: `bool`
- `pullRequestEnvironmentName`: `str`
- `backendEnvironmentArn`: `str`

Returns a `Coroutine` for
[CreateBranchResultTypeDef](./type_defs.md#createbranchresulttypedef).

<a id="create_deployment"></a>

### create_deployment

Creates a deployment for a manually deployed Amplify app.

Type annotations for `aiobotocore.create_client("amplify").create_deployment`
method.

Boto3 documentation:
[Amplify.Client.create_deployment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_deployment)

Asynchronous method. Use `await create_deployment(...)` for a synchronous call.

Arguments mapping described in
[CreateDeploymentRequestRequestTypeDef](./type_defs.md#createdeploymentrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*
- `fileMap`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateDeploymentResultTypeDef](./type_defs.md#createdeploymentresulttypedef).

<a id="create_domain_association"></a>

### create_domain_association

Creates a new domain association for an Amplify app.

Type annotations for
`aiobotocore.create_client("amplify").create_domain_association` method.

Boto3 documentation:
[Amplify.Client.create_domain_association](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_domain_association)

Asynchronous method. Use `await create_domain_association(...)` for a
synchronous call.

Arguments mapping described in
[CreateDomainAssociationRequestRequestTypeDef](./type_defs.md#createdomainassociationrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `domainName`: `str` *(required)*
- `subDomainSettings`:
  `Sequence`\[[SubDomainSettingTypeDef](./type_defs.md#subdomainsettingtypedef)\]
  *(required)*
- `enableAutoSubDomain`: `bool`
- `autoSubDomainCreationPatterns`: `Sequence`\[`str`\]
- `autoSubDomainIAMRole`: `str`

Returns a `Coroutine` for
[CreateDomainAssociationResultTypeDef](./type_defs.md#createdomainassociationresulttypedef).

<a id="create_webhook"></a>

### create_webhook

Creates a new webhook on an Amplify app.

Type annotations for `aiobotocore.create_client("amplify").create_webhook`
method.

Boto3 documentation:
[Amplify.Client.create_webhook](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_webhook)

Asynchronous method. Use `await create_webhook(...)` for a synchronous call.

Arguments mapping described in
[CreateWebhookRequestRequestTypeDef](./type_defs.md#createwebhookrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*
- `description`: `str`

Returns a `Coroutine` for
[CreateWebhookResultTypeDef](./type_defs.md#createwebhookresulttypedef).

<a id="delete_app"></a>

### delete_app

Deletes an existing Amplify app specified by an app ID.

Type annotations for `aiobotocore.create_client("amplify").delete_app` method.

Boto3 documentation:
[Amplify.Client.delete_app](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.delete_app)

Asynchronous method. Use `await delete_app(...)` for a synchronous call.

Arguments mapping described in
[DeleteAppRequestRequestTypeDef](./type_defs.md#deleteapprequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteAppResultTypeDef](./type_defs.md#deleteappresulttypedef).

<a id="delete_backend_environment"></a>

### delete_backend_environment

Deletes a backend environment for an Amplify app.

Type annotations for
`aiobotocore.create_client("amplify").delete_backend_environment` method.

Boto3 documentation:
[Amplify.Client.delete_backend_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.delete_backend_environment)

Asynchronous method. Use `await delete_backend_environment(...)` for a
synchronous call.

Arguments mapping described in
[DeleteBackendEnvironmentRequestRequestTypeDef](./type_defs.md#deletebackendenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteBackendEnvironmentResultTypeDef](./type_defs.md#deletebackendenvironmentresulttypedef).

<a id="delete_branch"></a>

### delete_branch

Deletes a branch for an Amplify app.

Type annotations for `aiobotocore.create_client("amplify").delete_branch`
method.

Boto3 documentation:
[Amplify.Client.delete_branch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.delete_branch)

Asynchronous method. Use `await delete_branch(...)` for a synchronous call.

Arguments mapping described in
[DeleteBranchRequestRequestTypeDef](./type_defs.md#deletebranchrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteBranchResultTypeDef](./type_defs.md#deletebranchresulttypedef).

<a id="delete_domain_association"></a>

### delete_domain_association

Deletes a domain association for an Amplify app.

Type annotations for
`aiobotocore.create_client("amplify").delete_domain_association` method.

Boto3 documentation:
[Amplify.Client.delete_domain_association](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.delete_domain_association)

Asynchronous method. Use `await delete_domain_association(...)` for a
synchronous call.

Arguments mapping described in
[DeleteDomainAssociationRequestRequestTypeDef](./type_defs.md#deletedomainassociationrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `domainName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteDomainAssociationResultTypeDef](./type_defs.md#deletedomainassociationresulttypedef).

<a id="delete_job"></a>

### delete_job

Deletes a job for a branch of an Amplify app.

Type annotations for `aiobotocore.create_client("amplify").delete_job` method.

Boto3 documentation:
[Amplify.Client.delete_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.delete_job)

Asynchronous method. Use `await delete_job(...)` for a synchronous call.

Arguments mapping described in
[DeleteJobRequestRequestTypeDef](./type_defs.md#deletejobrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*
- `jobId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteJobResultTypeDef](./type_defs.md#deletejobresulttypedef).

<a id="delete_webhook"></a>

### delete_webhook

Deletes a webhook.

Type annotations for `aiobotocore.create_client("amplify").delete_webhook`
method.

Boto3 documentation:
[Amplify.Client.delete_webhook](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.delete_webhook)

Asynchronous method. Use `await delete_webhook(...)` for a synchronous call.

Arguments mapping described in
[DeleteWebhookRequestRequestTypeDef](./type_defs.md#deletewebhookrequestrequesttypedef).

Keyword-only arguments:

- `webhookId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteWebhookResultTypeDef](./type_defs.md#deletewebhookresulttypedef).

<a id="generate_access_logs"></a>

### generate_access_logs

Returns the website access logs for a specific time range using a presigned
URL.

Type annotations for
`aiobotocore.create_client("amplify").generate_access_logs` method.

Boto3 documentation:
[Amplify.Client.generate_access_logs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.generate_access_logs)

Asynchronous method. Use `await generate_access_logs(...)` for a synchronous
call.

Arguments mapping described in
[GenerateAccessLogsRequestRequestTypeDef](./type_defs.md#generateaccesslogsrequestrequesttypedef).

Keyword-only arguments:

- `domainName`: `str` *(required)*
- `appId`: `str` *(required)*
- `startTime`: `Union`\[`datetime`, `str`\]
- `endTime`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for
[GenerateAccessLogsResultTypeDef](./type_defs.md#generateaccesslogsresulttypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("amplify").generate_presigned_url` method.

Boto3 documentation:
[Amplify.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_app"></a>

### get_app

Returns an existing Amplify app by appID.

Type annotations for `aiobotocore.create_client("amplify").get_app` method.

Boto3 documentation:
[Amplify.Client.get_app](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.get_app)

Asynchronous method. Use `await get_app(...)` for a synchronous call.

Arguments mapping described in
[GetAppRequestRequestTypeDef](./type_defs.md#getapprequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*

Returns a `Coroutine` for
[GetAppResultTypeDef](./type_defs.md#getappresulttypedef).

<a id="get_artifact_url"></a>

### get_artifact_url

Returns the artifact info that corresponds to an artifact id.

Type annotations for `aiobotocore.create_client("amplify").get_artifact_url`
method.

Boto3 documentation:
[Amplify.Client.get_artifact_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.get_artifact_url)

Asynchronous method. Use `await get_artifact_url(...)` for a synchronous call.

Arguments mapping described in
[GetArtifactUrlRequestRequestTypeDef](./type_defs.md#getartifacturlrequestrequesttypedef).

Keyword-only arguments:

- `artifactId`: `str` *(required)*

Returns a `Coroutine` for
[GetArtifactUrlResultTypeDef](./type_defs.md#getartifacturlresulttypedef).

<a id="get_backend_environment"></a>

### get_backend_environment

Returns a backend environment for an Amplify app.

Type annotations for
`aiobotocore.create_client("amplify").get_backend_environment` method.

Boto3 documentation:
[Amplify.Client.get_backend_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.get_backend_environment)

Asynchronous method. Use `await get_backend_environment(...)` for a synchronous
call.

Arguments mapping described in
[GetBackendEnvironmentRequestRequestTypeDef](./type_defs.md#getbackendenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*

Returns a `Coroutine` for
[GetBackendEnvironmentResultTypeDef](./type_defs.md#getbackendenvironmentresulttypedef).

<a id="get_branch"></a>

### get_branch

Returns a branch for an Amplify app.

Type annotations for `aiobotocore.create_client("amplify").get_branch` method.

Boto3 documentation:
[Amplify.Client.get_branch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.get_branch)

Asynchronous method. Use `await get_branch(...)` for a synchronous call.

Arguments mapping described in
[GetBranchRequestRequestTypeDef](./type_defs.md#getbranchrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*

Returns a `Coroutine` for
[GetBranchResultTypeDef](./type_defs.md#getbranchresulttypedef).

<a id="get_domain_association"></a>

### get_domain_association

Returns the domain information for an Amplify app.

Type annotations for
`aiobotocore.create_client("amplify").get_domain_association` method.

Boto3 documentation:
[Amplify.Client.get_domain_association](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.get_domain_association)

Asynchronous method. Use `await get_domain_association(...)` for a synchronous
call.

Arguments mapping described in
[GetDomainAssociationRequestRequestTypeDef](./type_defs.md#getdomainassociationrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `domainName`: `str` *(required)*

Returns a `Coroutine` for
[GetDomainAssociationResultTypeDef](./type_defs.md#getdomainassociationresulttypedef).

<a id="get_job"></a>

### get_job

Returns a job for a branch of an Amplify app.

Type annotations for `aiobotocore.create_client("amplify").get_job` method.

Boto3 documentation:
[Amplify.Client.get_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.get_job)

Asynchronous method. Use `await get_job(...)` for a synchronous call.

Arguments mapping described in
[GetJobRequestRequestTypeDef](./type_defs.md#getjobrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*
- `jobId`: `str` *(required)*

Returns a `Coroutine` for
[GetJobResultTypeDef](./type_defs.md#getjobresulttypedef).

<a id="get_webhook"></a>

### get_webhook

Returns the webhook information that corresponds to a specified webhook ID.

Type annotations for `aiobotocore.create_client("amplify").get_webhook` method.

Boto3 documentation:
[Amplify.Client.get_webhook](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.get_webhook)

Asynchronous method. Use `await get_webhook(...)` for a synchronous call.

Arguments mapping described in
[GetWebhookRequestRequestTypeDef](./type_defs.md#getwebhookrequestrequesttypedef).

Keyword-only arguments:

- `webhookId`: `str` *(required)*

Returns a `Coroutine` for
[GetWebhookResultTypeDef](./type_defs.md#getwebhookresulttypedef).

<a id="list_apps"></a>

### list_apps

Returns a list of the existing Amplify apps.

Type annotations for `aiobotocore.create_client("amplify").list_apps` method.

Boto3 documentation:
[Amplify.Client.list_apps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.list_apps)

Asynchronous method. Use `await list_apps(...)` for a synchronous call.

Arguments mapping described in
[ListAppsRequestRequestTypeDef](./type_defs.md#listappsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListAppsResultTypeDef](./type_defs.md#listappsresulttypedef).

<a id="list_artifacts"></a>

### list_artifacts

Returns a list of artifacts for a specified app, branch, and job.

Type annotations for `aiobotocore.create_client("amplify").list_artifacts`
method.

Boto3 documentation:
[Amplify.Client.list_artifacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.list_artifacts)

Asynchronous method. Use `await list_artifacts(...)` for a synchronous call.

Arguments mapping described in
[ListArtifactsRequestRequestTypeDef](./type_defs.md#listartifactsrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*
- `jobId`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListArtifactsResultTypeDef](./type_defs.md#listartifactsresulttypedef).

<a id="list_backend_environments"></a>

### list_backend_environments

Lists the backend environments for an Amplify app.

Type annotations for
`aiobotocore.create_client("amplify").list_backend_environments` method.

Boto3 documentation:
[Amplify.Client.list_backend_environments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.list_backend_environments)

Asynchronous method. Use `await list_backend_environments(...)` for a
synchronous call.

Arguments mapping described in
[ListBackendEnvironmentsRequestRequestTypeDef](./type_defs.md#listbackendenvironmentsrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `environmentName`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListBackendEnvironmentsResultTypeDef](./type_defs.md#listbackendenvironmentsresulttypedef).

<a id="list_branches"></a>

### list_branches

Lists the branches of an Amplify app.

Type annotations for `aiobotocore.create_client("amplify").list_branches`
method.

Boto3 documentation:
[Amplify.Client.list_branches](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.list_branches)

Asynchronous method. Use `await list_branches(...)` for a synchronous call.

Arguments mapping described in
[ListBranchesRequestRequestTypeDef](./type_defs.md#listbranchesrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListBranchesResultTypeDef](./type_defs.md#listbranchesresulttypedef).

<a id="list_domain_associations"></a>

### list_domain_associations

Returns the domain associations for an Amplify app.

Type annotations for
`aiobotocore.create_client("amplify").list_domain_associations` method.

Boto3 documentation:
[Amplify.Client.list_domain_associations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.list_domain_associations)

Asynchronous method. Use `await list_domain_associations(...)` for a
synchronous call.

Arguments mapping described in
[ListDomainAssociationsRequestRequestTypeDef](./type_defs.md#listdomainassociationsrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListDomainAssociationsResultTypeDef](./type_defs.md#listdomainassociationsresulttypedef).

<a id="list_jobs"></a>

### list_jobs

Lists the jobs for a branch of an Amplify app.

Type annotations for `aiobotocore.create_client("amplify").list_jobs` method.

Boto3 documentation:
[Amplify.Client.list_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.list_jobs)

Asynchronous method. Use `await list_jobs(...)` for a synchronous call.

Arguments mapping described in
[ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Returns a list of tags for a specified Amazon Resource Name (ARN).

Type annotations for
`aiobotocore.create_client("amplify").list_tags_for_resource` method.

Boto3 documentation:
[Amplify.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="list_webhooks"></a>

### list_webhooks

Returns a list of webhooks for an Amplify app.

Type annotations for `aiobotocore.create_client("amplify").list_webhooks`
method.

Boto3 documentation:
[Amplify.Client.list_webhooks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.list_webhooks)

Asynchronous method. Use `await list_webhooks(...)` for a synchronous call.

Arguments mapping described in
[ListWebhooksRequestRequestTypeDef](./type_defs.md#listwebhooksrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListWebhooksResultTypeDef](./type_defs.md#listwebhooksresulttypedef).

<a id="start_deployment"></a>

### start_deployment

Starts a deployment for a manually deployed app.

Type annotations for `aiobotocore.create_client("amplify").start_deployment`
method.

Boto3 documentation:
[Amplify.Client.start_deployment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.start_deployment)

Asynchronous method. Use `await start_deployment(...)` for a synchronous call.

Arguments mapping described in
[StartDeploymentRequestRequestTypeDef](./type_defs.md#startdeploymentrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*
- `jobId`: `str`
- `sourceUrl`: `str`

Returns a `Coroutine` for
[StartDeploymentResultTypeDef](./type_defs.md#startdeploymentresulttypedef).

<a id="start_job"></a>

### start_job

Starts a new job for a branch of an Amplify app.

Type annotations for `aiobotocore.create_client("amplify").start_job` method.

Boto3 documentation:
[Amplify.Client.start_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.start_job)

Asynchronous method. Use `await start_job(...)` for a synchronous call.

Arguments mapping described in
[StartJobRequestRequestTypeDef](./type_defs.md#startjobrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*
- `jobType`: [JobTypeType](./literals.md#jobtypetype) *(required)*
- `jobId`: `str`
- `jobReason`: `str`
- `commitId`: `str`
- `commitMessage`: `str`
- `commitTime`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for
[StartJobResultTypeDef](./type_defs.md#startjobresulttypedef).

<a id="stop_job"></a>

### stop_job

Stops a job that is in progress for a branch of an Amplify app.

Type annotations for `aiobotocore.create_client("amplify").stop_job` method.

Boto3 documentation:
[Amplify.Client.stop_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.stop_job)

Asynchronous method. Use `await stop_job(...)` for a synchronous call.

Arguments mapping described in
[StopJobRequestRequestTypeDef](./type_defs.md#stopjobrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*
- `jobId`: `str` *(required)*

Returns a `Coroutine` for
[StopJobResultTypeDef](./type_defs.md#stopjobresulttypedef).

<a id="tag_resource"></a>

### tag_resource

Tags the resource with a tag key and value.

Type annotations for `aiobotocore.create_client("amplify").tag_resource`
method.

Boto3 documentation:
[Amplify.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Untags a resource with a specified Amazon Resource Name (ARN).

Type annotations for `aiobotocore.create_client("amplify").untag_resource`
method.

Boto3 documentation:
[Amplify.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_app"></a>

### update_app

Updates an existing Amplify app.

Type annotations for `aiobotocore.create_client("amplify").update_app` method.

Boto3 documentation:
[Amplify.Client.update_app](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.update_app)

Asynchronous method. Use `await update_app(...)` for a synchronous call.

Arguments mapping described in
[UpdateAppRequestRequestTypeDef](./type_defs.md#updateapprequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `name`: `str`
- `description`: `str`
- `platform`: `Literal['WEB']` (see [PlatformType](./literals.md#platformtype))
- `iamServiceRoleArn`: `str`
- `environmentVariables`: `Mapping`\[`str`, `str`\]
- `enableBranchAutoBuild`: `bool`
- `enableBranchAutoDeletion`: `bool`
- `enableBasicAuth`: `bool`
- `basicAuthCredentials`: `str`
- `customRules`:
  `Sequence`\[[CustomRuleTypeDef](./type_defs.md#customruletypedef)\]
- `buildSpec`: `str`
- `customHeaders`: `str`
- `enableAutoBranchCreation`: `bool`
- `autoBranchCreationPatterns`: `Sequence`\[`str`\]
- `autoBranchCreationConfig`:
  [AutoBranchCreationConfigTypeDef](./type_defs.md#autobranchcreationconfigtypedef)
- `repository`: `str`
- `oauthToken`: `str`
- `accessToken`: `str`

Returns a `Coroutine` for
[UpdateAppResultTypeDef](./type_defs.md#updateappresulttypedef).

<a id="update_branch"></a>

### update_branch

Updates a branch for an Amplify app.

Type annotations for `aiobotocore.create_client("amplify").update_branch`
method.

Boto3 documentation:
[Amplify.Client.update_branch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.update_branch)

Asynchronous method. Use `await update_branch(...)` for a synchronous call.

Arguments mapping described in
[UpdateBranchRequestRequestTypeDef](./type_defs.md#updatebranchrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*
- `description`: `str`
- `framework`: `str`
- `stage`: [StageType](./literals.md#stagetype)
- `enableNotification`: `bool`
- `enableAutoBuild`: `bool`
- `environmentVariables`: `Mapping`\[`str`, `str`\]
- `basicAuthCredentials`: `str`
- `enableBasicAuth`: `bool`
- `enablePerformanceMode`: `bool`
- `buildSpec`: `str`
- `ttl`: `str`
- `displayName`: `str`
- `enablePullRequestPreview`: `bool`
- `pullRequestEnvironmentName`: `str`
- `backendEnvironmentArn`: `str`

Returns a `Coroutine` for
[UpdateBranchResultTypeDef](./type_defs.md#updatebranchresulttypedef).

<a id="update_domain_association"></a>

### update_domain_association

Creates a new domain association for an Amplify app.

Type annotations for
`aiobotocore.create_client("amplify").update_domain_association` method.

Boto3 documentation:
[Amplify.Client.update_domain_association](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.update_domain_association)

Asynchronous method. Use `await update_domain_association(...)` for a
synchronous call.

Arguments mapping described in
[UpdateDomainAssociationRequestRequestTypeDef](./type_defs.md#updatedomainassociationrequestrequesttypedef).

Keyword-only arguments:

- `appId`: `str` *(required)*
- `domainName`: `str` *(required)*
- `subDomainSettings`:
  `Sequence`\[[SubDomainSettingTypeDef](./type_defs.md#subdomainsettingtypedef)\]
  *(required)*
- `enableAutoSubDomain`: `bool`
- `autoSubDomainCreationPatterns`: `Sequence`\[`str`\]
- `autoSubDomainIAMRole`: `str`

Returns a `Coroutine` for
[UpdateDomainAssociationResultTypeDef](./type_defs.md#updatedomainassociationresulttypedef).

<a id="update_webhook"></a>

### update_webhook

Updates a webhook.

Type annotations for `aiobotocore.create_client("amplify").update_webhook`
method.

Boto3 documentation:
[Amplify.Client.update_webhook](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.update_webhook)

Asynchronous method. Use `await update_webhook(...)` for a synchronous call.

Arguments mapping described in
[UpdateWebhookRequestRequestTypeDef](./type_defs.md#updatewebhookrequestrequesttypedef).

Keyword-only arguments:

- `webhookId`: `str` *(required)*
- `branchName`: `str`
- `description`: `str`

Returns a `Coroutine` for
[UpdateWebhookResultTypeDef](./type_defs.md#updatewebhookresulttypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("amplify").get_paginator`
method with overloads.

- `client.get_paginator("list_apps")` ->
  [ListAppsPaginator](./paginators.md#listappspaginator)
- `client.get_paginator("list_branches")` ->
  [ListBranchesPaginator](./paginators.md#listbranchespaginator)
- `client.get_paginator("list_domain_associations")` ->
  [ListDomainAssociationsPaginator](./paginators.md#listdomainassociationspaginator)
- `client.get_paginator("list_jobs")` ->
  [ListJobsPaginator](./paginators.md#listjobspaginator)
