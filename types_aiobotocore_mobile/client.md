<a id="mobileclient-for-aiobotocore-mobile-module"></a>

# MobileClient for aiobotocore Mobile module

> [Index](..) > [Mobile](.) > MobileClient

Auto-generated documentation for
[Mobile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
type annotations stubs module
[types-aiobotocore-mobile](https://pypi.org/project/types-aiobotocore-mobile/).

- [MobileClient for aiobotocore Mobile module](#mobileclient-for-aiobotocore-mobile-module)
  - [MobileClient](#mobileclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_project](#create_project)
    - [delete_project](#delete_project)
    - [describe_bundle](#describe_bundle)
    - [describe_project](#describe_project)
    - [export_bundle](#export_bundle)
    - [export_project](#export_project)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_bundles](#list_bundles)
    - [list_projects](#list_projects)
    - [update_project](#update_project)
    - [get_paginator](#get_paginator)

<a id="mobileclient"></a>

## MobileClient

Type annotations for `aiobotocore.create_client("mobile")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_mobile.client import MobileClient

def get_mobile_client() -> MobileClient:
    return Session().client("mobile")
```

Boto3 documentation:
[Mobile.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_mobile.client import Exceptions

def handle_error(exc: Exceptions.AccountActionRequiredException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccountActionRequiredException`
- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.InternalFailureException`
- `Exceptions.LimitExceededException`
- `Exceptions.NotFoundException`
- `Exceptions.ServiceUnavailableException`
- `Exceptions.TooManyRequestsException`
- `Exceptions.UnauthorizedException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

MobileClient exceptions.

Type annotations for `aiobotocore.create_client("mobile").exceptions` method.

Boto3 documentation:
[Mobile.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("mobile").can_paginate` method.

Boto3 documentation:
[Mobile.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_project"></a>

### create_project

Creates an AWS Mobile Hub project.

Type annotations for `aiobotocore.create_client("mobile").create_project`
method.

Boto3 documentation:
[Mobile.Client.create_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.create_project)

Asynchronous method. Use `await create_project(...)` for a synchronous call.

Arguments mapping described in
[CreateProjectRequestRequestTypeDef](./type_defs.md#createprojectrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str`
- `region`: `str`
- `contents`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]
- `snapshotId`: `str`

Returns a `Coroutine` for
[CreateProjectResultTypeDef](./type_defs.md#createprojectresulttypedef).

<a id="delete_project"></a>

### delete_project

Delets a project in AWS Mobile Hub.

Type annotations for `aiobotocore.create_client("mobile").delete_project`
method.

Boto3 documentation:
[Mobile.Client.delete_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.delete_project)

Asynchronous method. Use `await delete_project(...)` for a synchronous call.

Arguments mapping described in
[DeleteProjectRequestRequestTypeDef](./type_defs.md#deleteprojectrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteProjectResultTypeDef](./type_defs.md#deleteprojectresulttypedef).

<a id="describe_bundle"></a>

### describe_bundle

Get the bundle details for the requested bundle id.

Type annotations for `aiobotocore.create_client("mobile").describe_bundle`
method.

Boto3 documentation:
[Mobile.Client.describe_bundle](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.describe_bundle)

Asynchronous method. Use `await describe_bundle(...)` for a synchronous call.

Arguments mapping described in
[DescribeBundleRequestRequestTypeDef](./type_defs.md#describebundlerequestrequesttypedef).

Keyword-only arguments:

- `bundleId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeBundleResultTypeDef](./type_defs.md#describebundleresulttypedef).

<a id="describe_project"></a>

### describe_project

Gets details about a project in AWS Mobile Hub.

Type annotations for `aiobotocore.create_client("mobile").describe_project`
method.

Boto3 documentation:
[Mobile.Client.describe_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.describe_project)

Asynchronous method. Use `await describe_project(...)` for a synchronous call.

Arguments mapping described in
[DescribeProjectRequestRequestTypeDef](./type_defs.md#describeprojectrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `syncFromResources`: `bool`

Returns a `Coroutine` for
[DescribeProjectResultTypeDef](./type_defs.md#describeprojectresulttypedef).

<a id="export_bundle"></a>

### export_bundle

Generates customized software development kit (SDK) and or tool packages used
to integrate mobile web or mobile app clients with backend AWS resources.

Type annotations for `aiobotocore.create_client("mobile").export_bundle`
method.

Boto3 documentation:
[Mobile.Client.export_bundle](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.export_bundle)

Asynchronous method. Use `await export_bundle(...)` for a synchronous call.

Arguments mapping described in
[ExportBundleRequestRequestTypeDef](./type_defs.md#exportbundlerequestrequesttypedef).

Keyword-only arguments:

- `bundleId`: `str` *(required)*
- `projectId`: `str`
- `platform`: [PlatformType](./literals.md#platformtype)

Returns a `Coroutine` for
[ExportBundleResultTypeDef](./type_defs.md#exportbundleresulttypedef).

<a id="export_project"></a>

### export_project

Exports project configuration to a snapshot which can be downloaded and shared.

Type annotations for `aiobotocore.create_client("mobile").export_project`
method.

Boto3 documentation:
[Mobile.Client.export_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.export_project)

Asynchronous method. Use `await export_project(...)` for a synchronous call.

Arguments mapping described in
[ExportProjectRequestRequestTypeDef](./type_defs.md#exportprojectrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*

Returns a `Coroutine` for
[ExportProjectResultTypeDef](./type_defs.md#exportprojectresulttypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("mobile").generate_presigned_url` method.

Boto3 documentation:
[Mobile.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_bundles"></a>

### list_bundles

List all available bundles.

Type annotations for `aiobotocore.create_client("mobile").list_bundles` method.

Boto3 documentation:
[Mobile.Client.list_bundles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.list_bundles)

Asynchronous method. Use `await list_bundles(...)` for a synchronous call.

Arguments mapping described in
[ListBundlesRequestRequestTypeDef](./type_defs.md#listbundlesrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListBundlesResultTypeDef](./type_defs.md#listbundlesresulttypedef).

<a id="list_projects"></a>

### list_projects

Lists projects in AWS Mobile Hub.

Type annotations for `aiobotocore.create_client("mobile").list_projects`
method.

Boto3 documentation:
[Mobile.Client.list_projects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.list_projects)

Asynchronous method. Use `await list_projects(...)` for a synchronous call.

Arguments mapping described in
[ListProjectsRequestRequestTypeDef](./type_defs.md#listprojectsrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef).

<a id="update_project"></a>

### update_project

Update an existing project.

Type annotations for `aiobotocore.create_client("mobile").update_project`
method.

Boto3 documentation:
[Mobile.Client.update_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.update_project)

Asynchronous method. Use `await update_project(...)` for a synchronous call.

Arguments mapping described in
[UpdateProjectRequestRequestTypeDef](./type_defs.md#updateprojectrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `contents`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]

Returns a `Coroutine` for
[UpdateProjectResultTypeDef](./type_defs.md#updateprojectresulttypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("mobile").get_paginator` method
with overloads.

- `client.get_paginator("list_bundles")` ->
  [ListBundlesPaginator](./paginators.md#listbundlespaginator)
- `client.get_paginator("list_projects")` ->
  [ListProjectsPaginator](./paginators.md#listprojectspaginator)
