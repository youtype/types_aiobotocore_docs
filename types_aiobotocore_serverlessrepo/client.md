<a id="serverlessapplicationrepositoryclient-for-aiobotocore-serverlessapplicationrepository-module"></a>

# ServerlessApplicationRepositoryClient for aiobotocore ServerlessApplicationRepository module

> [Index](..) > [ServerlessApplicationRepository](.) >
> ServerlessApplicationRepositoryClient

Auto-generated documentation for
[ServerlessApplicationRepository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
type annotations stubs module
[types-aiobotocore-serverlessrepo](https://pypi.org/project/types-aiobotocore-serverlessrepo/).

- [ServerlessApplicationRepositoryClient for aiobotocore ServerlessApplicationRepository module](#serverlessapplicationrepositoryclient-for-aiobotocore-serverlessapplicationrepository-module)
  - [ServerlessApplicationRepositoryClient](#serverlessapplicationrepositoryclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_application](#create_application)
    - [create_application_version](#create_application_version)
    - [create_cloud_formation_change_set](#create_cloud_formation_change_set)
    - [create_cloud_formation_template](#create_cloud_formation_template)
    - [delete_application](#delete_application)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_application](#get_application)
    - [get_application_policy](#get_application_policy)
    - [get_cloud_formation_template](#get_cloud_formation_template)
    - [list_application_dependencies](#list_application_dependencies)
    - [list_application_versions](#list_application_versions)
    - [list_applications](#list_applications)
    - [put_application_policy](#put_application_policy)
    - [unshare_application](#unshare_application)
    - [update_application](#update_application)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="serverlessapplicationrepositoryclient"></a>

## ServerlessApplicationRepositoryClient

Type annotations for `session.create_client("serverlessrepo")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_serverlessrepo.client import ServerlessApplicationRepositoryClient

session = get_session()
async with session.create_client("serverlessrepo") as client:
    client: ServerlessApplicationRepositoryClient
```

Boto3 documentation:
[ServerlessApplicationRepository.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_serverlessrepo.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.ForbiddenException`
- `Exceptions.InternalServerErrorException`
- `Exceptions.NotFoundException`
- `Exceptions.TooManyRequestsException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ServerlessApplicationRepositoryClient exceptions.

Type annotations for `session.create_client("serverlessrepo").exceptions`
method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("serverlessrepo").can_paginate`
method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_application"></a>

### create_application

Creates an application, optionally including an AWS SAM file to create the
first application version in the same call.

Type annotations for
`session.create_client("serverlessrepo").create_application` method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.create_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.create_application)

Asynchronous method. Use `await create_application(...)` for a synchronous
call.

Arguments mapping described in
[CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef).

Keyword-only arguments:

- `Author`: `str` *(required)*
- `Description`: `str` *(required)*
- `Name`: `str` *(required)*
- `HomePageUrl`: `str`
- `Labels`: `Sequence`\[`str`\]
- `LicenseBody`: `str`
- `LicenseUrl`: `str`
- `ReadmeBody`: `str`
- `ReadmeUrl`: `str`
- `SemanticVersion`: `str`
- `SourceCodeArchiveUrl`: `str`
- `SourceCodeUrl`: `str`
- `SpdxLicenseId`: `str`
- `TemplateBody`: `str`
- `TemplateUrl`: `str`

Returns a `Coroutine` for
[CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef).

<a id="create_application_version"></a>

### create_application_version

Creates an application version.

Type annotations for
`session.create_client("serverlessrepo").create_application_version` method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.create_application_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.create_application_version)

Asynchronous method. Use `await create_application_version(...)` for a
synchronous call.

Arguments mapping described in
[CreateApplicationVersionRequestRequestTypeDef](./type_defs.md#createapplicationversionrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `SemanticVersion`: `str` *(required)*
- `SourceCodeArchiveUrl`: `str`
- `SourceCodeUrl`: `str`
- `TemplateBody`: `str`
- `TemplateUrl`: `str`

Returns a `Coroutine` for
[CreateApplicationVersionResponseTypeDef](./type_defs.md#createapplicationversionresponsetypedef).

<a id="create_cloud_formation_change_set"></a>

### create_cloud_formation_change_set

Creates an AWS CloudFormation change set for the given application.

Type annotations for
`session.create_client("serverlessrepo").create_cloud_formation_change_set`
method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.create_cloud_formation_change_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.create_cloud_formation_change_set)

Asynchronous method. Use `await create_cloud_formation_change_set(...)` for a
synchronous call.

Arguments mapping described in
[CreateCloudFormationChangeSetRequestRequestTypeDef](./type_defs.md#createcloudformationchangesetrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `StackName`: `str` *(required)*
- `Capabilities`: `Sequence`\[`str`\]
- `ChangeSetName`: `str`
- `ClientToken`: `str`
- `Description`: `str`
- `NotificationArns`: `Sequence`\[`str`\]
- `ParameterOverrides`:
  `Sequence`\[[ParameterValueTypeDef](./type_defs.md#parametervaluetypedef)\]
- `ResourceTypes`: `Sequence`\[`str`\]
- `RollbackConfiguration`:
  [RollbackConfigurationTypeDef](./type_defs.md#rollbackconfigurationtypedef)
- `SemanticVersion`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `TemplateId`: `str`

Returns a `Coroutine` for
[CreateCloudFormationChangeSetResponseTypeDef](./type_defs.md#createcloudformationchangesetresponsetypedef).

<a id="create_cloud_formation_template"></a>

### create_cloud_formation_template

Creates an AWS CloudFormation template.

Type annotations for
`session.create_client("serverlessrepo").create_cloud_formation_template`
method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.create_cloud_formation_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.create_cloud_formation_template)

Asynchronous method. Use `await create_cloud_formation_template(...)` for a
synchronous call.

Arguments mapping described in
[CreateCloudFormationTemplateRequestRequestTypeDef](./type_defs.md#createcloudformationtemplaterequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `SemanticVersion`: `str`

Returns a `Coroutine` for
[CreateCloudFormationTemplateResponseTypeDef](./type_defs.md#createcloudformationtemplateresponsetypedef).

<a id="delete_application"></a>

### delete_application

Deletes the specified application.

Type annotations for
`session.create_client("serverlessrepo").delete_application` method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.delete_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.delete_application)

Asynchronous method. Use `await delete_application(...)` for a synchronous
call.

Arguments mapping described in
[DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("serverlessrepo").generate_presigned_url` method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.generate_presigned_url)

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

Gets the specified application.

Type annotations for `session.create_client("serverlessrepo").get_application`
method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.get_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.get_application)

Asynchronous method. Use `await get_application(...)` for a synchronous call.

Arguments mapping described in
[GetApplicationRequestRequestTypeDef](./type_defs.md#getapplicationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `SemanticVersion`: `str`

Returns a `Coroutine` for
[GetApplicationResponseTypeDef](./type_defs.md#getapplicationresponsetypedef).

<a id="get_application_policy"></a>

### get_application_policy

Retrieves the policy for the application.

Type annotations for
`session.create_client("serverlessrepo").get_application_policy` method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.get_application_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.get_application_policy)

Asynchronous method. Use `await get_application_policy(...)` for a synchronous
call.

Arguments mapping described in
[GetApplicationPolicyRequestRequestTypeDef](./type_defs.md#getapplicationpolicyrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*

Returns a `Coroutine` for
[GetApplicationPolicyResponseTypeDef](./type_defs.md#getapplicationpolicyresponsetypedef).

<a id="get_cloud_formation_template"></a>

### get_cloud_formation_template

Gets the specified AWS CloudFormation template.

Type annotations for
`session.create_client("serverlessrepo").get_cloud_formation_template` method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.get_cloud_formation_template](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.get_cloud_formation_template)

Asynchronous method. Use `await get_cloud_formation_template(...)` for a
synchronous call.

Arguments mapping described in
[GetCloudFormationTemplateRequestRequestTypeDef](./type_defs.md#getcloudformationtemplaterequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `TemplateId`: `str` *(required)*

Returns a `Coroutine` for
[GetCloudFormationTemplateResponseTypeDef](./type_defs.md#getcloudformationtemplateresponsetypedef).

<a id="list_application_dependencies"></a>

### list_application_dependencies

Retrieves the list of applications nested in the containing application.

Type annotations for
`session.create_client("serverlessrepo").list_application_dependencies` method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.list_application_dependencies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.list_application_dependencies)

Asynchronous method. Use `await list_application_dependencies(...)` for a
synchronous call.

Arguments mapping described in
[ListApplicationDependenciesRequestRequestTypeDef](./type_defs.md#listapplicationdependenciesrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `MaxItems`: `int`
- `NextToken`: `str`
- `SemanticVersion`: `str`

Returns a `Coroutine` for
[ListApplicationDependenciesResponseTypeDef](./type_defs.md#listapplicationdependenciesresponsetypedef).

<a id="list_application_versions"></a>

### list_application_versions

Lists versions for the specified application.

Type annotations for
`session.create_client("serverlessrepo").list_application_versions` method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.list_application_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.list_application_versions)

Asynchronous method. Use `await list_application_versions(...)` for a
synchronous call.

Arguments mapping described in
[ListApplicationVersionsRequestRequestTypeDef](./type_defs.md#listapplicationversionsrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `MaxItems`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListApplicationVersionsResponseTypeDef](./type_defs.md#listapplicationversionsresponsetypedef).

<a id="list_applications"></a>

### list_applications

Lists applications owned by the requester.

Type annotations for
`session.create_client("serverlessrepo").list_applications` method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.list_applications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.list_applications)

Asynchronous method. Use `await list_applications(...)` for a synchronous call.

Arguments mapping described in
[ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef).

Keyword-only arguments:

- `MaxItems`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef).

<a id="put_application_policy"></a>

### put_application_policy

Sets the permission policy for an application.

Type annotations for
`session.create_client("serverlessrepo").put_application_policy` method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.put_application_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.put_application_policy)

Asynchronous method. Use `await put_application_policy(...)` for a synchronous
call.

Arguments mapping described in
[PutApplicationPolicyRequestRequestTypeDef](./type_defs.md#putapplicationpolicyrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `Statements`:
  `Sequence`\[[ApplicationPolicyStatementTypeDef](./type_defs.md#applicationpolicystatementtypedef)\]
  *(required)*

Returns a `Coroutine` for
[PutApplicationPolicyResponseTypeDef](./type_defs.md#putapplicationpolicyresponsetypedef).

<a id="unshare_application"></a>

### unshare_application

Unshares an application from an AWS Organization.

Type annotations for
`session.create_client("serverlessrepo").unshare_application` method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.unshare_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.unshare_application)

Asynchronous method. Use `await unshare_application(...)` for a synchronous
call.

Arguments mapping described in
[UnshareApplicationRequestRequestTypeDef](./type_defs.md#unshareapplicationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `OrganizationId`: `str` *(required)*

<a id="update_application"></a>

### update_application

Updates the specified application.

Type annotations for
`session.create_client("serverlessrepo").update_application` method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.update_application](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.update_application)

Asynchronous method. Use `await update_application(...)` for a synchronous
call.

Arguments mapping described in
[UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationId`: `str` *(required)*
- `Author`: `str`
- `Description`: `str`
- `HomePageUrl`: `str`
- `Labels`: `Sequence`\[`str`\]
- `ReadmeBody`: `str`
- `ReadmeUrl`: `str`

Returns a `Coroutine` for
[UpdateApplicationResponseTypeDef](./type_defs.md#updateapplicationresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("serverlessrepo").__aenter__`
method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[ServerlessApplicationRepositoryClient](#serverlessapplicationrepositoryclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("serverlessrepo").__aexit__`
method.

Boto3 documentation:
[ServerlessApplicationRepository.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("serverlessrepo").get_paginator`
method with overloads.

- `client.get_paginator("list_application_dependencies")` ->
  [ListApplicationDependenciesPaginator](./paginators.md#listapplicationdependenciespaginator)
- `client.get_paginator("list_application_versions")` ->
  [ListApplicationVersionsPaginator](./paginators.md#listapplicationversionspaginator)
- `client.get_paginator("list_applications")` ->
  [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
