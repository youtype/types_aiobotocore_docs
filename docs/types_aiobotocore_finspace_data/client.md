<a id="finspacedataclient-for-aiobotocore-finspacedata-module"></a>

# FinSpaceDataClient for aiobotocore FinSpaceData module

> [Index](../README.md) > [FinSpaceData](./README.md) > FinSpaceDataClient

Auto-generated documentation for
[FinSpaceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
type annotations stubs module
[types-aiobotocore-finspace-data](https://pypi.org/project/types-aiobotocore-finspace-data/).

- [FinSpaceDataClient for aiobotocore FinSpaceData module](#finspacedataclient-for-aiobotocore-finspacedata-module)
  - [FinSpaceDataClient](#finspacedataclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_changeset](#create_changeset)
    - [create_data_view](#create_data_view)
    - [create_dataset](#create_dataset)
    - [create_permission_group](#create_permission_group)
    - [create_user](#create_user)
    - [delete_dataset](#delete_dataset)
    - [delete_permission_group](#delete_permission_group)
    - [disable_user](#disable_user)
    - [enable_user](#enable_user)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_changeset](#get_changeset)
    - [get_data_view](#get_data_view)
    - [get_dataset](#get_dataset)
    - [get_programmatic_access_credentials](#get_programmatic_access_credentials)
    - [get_user](#get_user)
    - [get_working_location](#get_working_location)
    - [list_changesets](#list_changesets)
    - [list_data_views](#list_data_views)
    - [list_datasets](#list_datasets)
    - [list_permission_groups](#list_permission_groups)
    - [list_users](#list_users)
    - [reset_user_password](#reset_user_password)
    - [update_changeset](#update_changeset)
    - [update_dataset](#update_dataset)
    - [update_permission_group](#update_permission_group)
    - [update_user](#update_user)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="finspacedataclient"></a>

## FinSpaceDataClient

Type annotations for `session.create_client("finspace-data")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_finspace_data.client import FinSpaceDataClient

session = get_session()
async with session.create_client("finspace-data") as client:
    client: FinSpaceDataClient
```

Boto3 documentation:
[FinSpaceData.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_finspace_data.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.LimitExceededException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

FinSpaceDataClient exceptions.

Type annotations for `session.create_client("finspace-data").exceptions`
method.

Boto3 documentation:
[FinSpaceData.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("finspace-data").can_paginate`
method.

Boto3 documentation:
[FinSpaceData.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_changeset"></a>

### create_changeset

Creates a new Changeset in a FinSpace Dataset.

Type annotations for `session.create_client("finspace-data").create_changeset`
method.

Boto3 documentation:
[FinSpaceData.Client.create_changeset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_changeset)

Asynchronous method. Use `await create_changeset(...)` for a synchronous call.

Arguments mapping described in
[CreateChangesetRequestRequestTypeDef](./type_defs.md#createchangesetrequestrequesttypedef).

Keyword-only arguments:

- `datasetId`: `str` *(required)*
- `changeType`: [ChangeTypeType](./literals.md#changetypetype) *(required)*
- `sourceParams`: `Mapping`\[`str`, `str`\] *(required)*
- `formatParams`: `Mapping`\[`str`, `str`\] *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[CreateChangesetResponseTypeDef](./type_defs.md#createchangesetresponsetypedef).

<a id="create\_data\_view"></a>

### create_data_view

Creates a Dataview for a Dataset.

Type annotations for `session.create_client("finspace-data").create_data_view`
method.

Boto3 documentation:
[FinSpaceData.Client.create_data_view](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_data_view)

Asynchronous method. Use `await create_data_view(...)` for a synchronous call.

Arguments mapping described in
[CreateDataViewRequestRequestTypeDef](./type_defs.md#createdataviewrequestrequesttypedef).

Keyword-only arguments:

- `datasetId`: `str` *(required)*
- `destinationTypeParams`:
  [DataViewDestinationTypeParamsTypeDef](./type_defs.md#dataviewdestinationtypeparamstypedef)
  *(required)*
- `clientToken`: `str`
- `autoUpdate`: `bool`
- `sortColumns`: `Sequence`\[`str`\]
- `partitionColumns`: `Sequence`\[`str`\]
- `asOfTimestamp`: `int`

Returns a `Coroutine` for
[CreateDataViewResponseTypeDef](./type_defs.md#createdataviewresponsetypedef).

<a id="create\_dataset"></a>

### create_dataset

Creates a new FinSpace Dataset.

Type annotations for `session.create_client("finspace-data").create_dataset`
method.

Boto3 documentation:
[FinSpaceData.Client.create_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_dataset)

Asynchronous method. Use `await create_dataset(...)` for a synchronous call.

Arguments mapping described in
[CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef).

Keyword-only arguments:

- `datasetTitle`: `str` *(required)*
- `kind`: [DatasetKindType](./literals.md#datasetkindtype) *(required)*
- `permissionGroupParams`:
  [PermissionGroupParamsTypeDef](./type_defs.md#permissiongroupparamstypedef)
  *(required)*
- `clientToken`: `str`
- `datasetDescription`: `str`
- `ownerInfo`:
  [DatasetOwnerInfoTypeDef](./type_defs.md#datasetownerinfotypedef)
- `alias`: `str`
- `schemaDefinition`: [SchemaUnionTypeDef](./type_defs.md#schemauniontypedef)

Returns a `Coroutine` for
[CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef).

<a id="create\_permission\_group"></a>

### create_permission_group

Creates a group of permissions for various actions that a user can perform in
FinSpace.

Type annotations for
`session.create_client("finspace-data").create_permission_group` method.

Boto3 documentation:
[FinSpaceData.Client.create_permission_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_permission_group)

Asynchronous method. Use `await create_permission_group(...)` for a synchronous
call.

Arguments mapping described in
[CreatePermissionGroupRequestRequestTypeDef](./type_defs.md#createpermissiongrouprequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `applicationPermissions`:
  `Sequence`\[[ApplicationPermissionType](./literals.md#applicationpermissiontype)\]
  *(required)*
- `description`: `str`
- `clientToken`: `str`

Returns a `Coroutine` for
[CreatePermissionGroupResponseTypeDef](./type_defs.md#createpermissiongroupresponsetypedef).

<a id="create\_user"></a>

### create_user

Creates a new user in FinSpace.

Type annotations for `session.create_client("finspace-data").create_user`
method.

Boto3 documentation:
[FinSpaceData.Client.create_user](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_user)

Asynchronous method. Use `await create_user(...)` for a synchronous call.

Arguments mapping described in
[CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef).

Keyword-only arguments:

- `emailAddress`: `str` *(required)*
- `type`: [UserTypeType](./literals.md#usertypetype) *(required)*
- `firstName`: `str`
- `lastName`: `str`
- `ApiAccess`: [ApiAccessType](./literals.md#apiaccesstype)
- `apiAccessPrincipalArn`: `str`
- `clientToken`: `str`

Returns a `Coroutine` for
[CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef).

<a id="delete\_dataset"></a>

### delete_dataset

Deletes a FinSpace Dataset.

Type annotations for `session.create_client("finspace-data").delete_dataset`
method.

Boto3 documentation:
[FinSpaceData.Client.delete_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.delete_dataset)

Asynchronous method. Use `await delete_dataset(...)` for a synchronous call.

Arguments mapping described in
[DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef).

Keyword-only arguments:

- `datasetId`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[DeleteDatasetResponseTypeDef](./type_defs.md#deletedatasetresponsetypedef).

<a id="delete\_permission\_group"></a>

### delete_permission_group

Deletes a permission group.

Type annotations for
`session.create_client("finspace-data").delete_permission_group` method.

Boto3 documentation:
[FinSpaceData.Client.delete_permission_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.delete_permission_group)

Asynchronous method. Use `await delete_permission_group(...)` for a synchronous
call.

Arguments mapping described in
[DeletePermissionGroupRequestRequestTypeDef](./type_defs.md#deletepermissiongrouprequestrequesttypedef).

Keyword-only arguments:

- `permissionGroupId`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[DeletePermissionGroupResponseTypeDef](./type_defs.md#deletepermissiongroupresponsetypedef).

<a id="disable\_user"></a>

### disable_user

Denies access to the FinSpace web application and API for the specified user.

Type annotations for `session.create_client("finspace-data").disable_user`
method.

Boto3 documentation:
[FinSpaceData.Client.disable_user](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.disable_user)

Asynchronous method. Use `await disable_user(...)` for a synchronous call.

Arguments mapping described in
[DisableUserRequestRequestTypeDef](./type_defs.md#disableuserrequestrequesttypedef).

Keyword-only arguments:

- `userId`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[DisableUserResponseTypeDef](./type_defs.md#disableuserresponsetypedef).

<a id="enable\_user"></a>

### enable_user

Allows the specified user to access the FinSpace web application and API.

Type annotations for `session.create_client("finspace-data").enable_user`
method.

Boto3 documentation:
[FinSpaceData.Client.enable_user](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.enable_user)

Asynchronous method. Use `await enable_user(...)` for a synchronous call.

Arguments mapping described in
[EnableUserRequestRequestTypeDef](./type_defs.md#enableuserrequestrequesttypedef).

Keyword-only arguments:

- `userId`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[EnableUserResponseTypeDef](./type_defs.md#enableuserresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("finspace-data").generate_presigned_url` method.

Boto3 documentation:
[FinSpaceData.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_changeset"></a>

### get_changeset

Get information about a Changeset.

Type annotations for `session.create_client("finspace-data").get_changeset`
method.

Boto3 documentation:
[FinSpaceData.Client.get_changeset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.get_changeset)

Asynchronous method. Use `await get_changeset(...)` for a synchronous call.

Arguments mapping described in
[GetChangesetRequestRequestTypeDef](./type_defs.md#getchangesetrequestrequesttypedef).

Keyword-only arguments:

- `datasetId`: `str` *(required)*
- `changesetId`: `str` *(required)*

Returns a `Coroutine` for
[GetChangesetResponseTypeDef](./type_defs.md#getchangesetresponsetypedef).

<a id="get\_data\_view"></a>

### get_data_view

Gets information about a Dataview.

Type annotations for `session.create_client("finspace-data").get_data_view`
method.

Boto3 documentation:
[FinSpaceData.Client.get_data_view](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.get_data_view)

Asynchronous method. Use `await get_data_view(...)` for a synchronous call.

Arguments mapping described in
[GetDataViewRequestRequestTypeDef](./type_defs.md#getdataviewrequestrequesttypedef).

Keyword-only arguments:

- `dataViewId`: `str` *(required)*
- `datasetId`: `str` *(required)*

Returns a `Coroutine` for
[GetDataViewResponseTypeDef](./type_defs.md#getdataviewresponsetypedef).

<a id="get\_dataset"></a>

### get_dataset

Returns information about a Dataset.

Type annotations for `session.create_client("finspace-data").get_dataset`
method.

Boto3 documentation:
[FinSpaceData.Client.get_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.get_dataset)

Asynchronous method. Use `await get_dataset(...)` for a synchronous call.

Arguments mapping described in
[GetDatasetRequestRequestTypeDef](./type_defs.md#getdatasetrequestrequesttypedef).

Keyword-only arguments:

- `datasetId`: `str` *(required)*

Returns a `Coroutine` for
[GetDatasetResponseTypeDef](./type_defs.md#getdatasetresponsetypedef).

<a id="get\_programmatic\_access\_credentials"></a>

### get_programmatic_access_credentials

Request programmatic credentials to use with FinSpace SDK.

Type annotations for
`session.create_client("finspace-data").get_programmatic_access_credentials`
method.

Boto3 documentation:
[FinSpaceData.Client.get_programmatic_access_credentials](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.get_programmatic_access_credentials)

Asynchronous method. Use `await get_programmatic_access_credentials(...)` for a
synchronous call.

Arguments mapping described in
[GetProgrammaticAccessCredentialsRequestRequestTypeDef](./type_defs.md#getprogrammaticaccesscredentialsrequestrequesttypedef).

Keyword-only arguments:

- `environmentId`: `str` *(required)*
- `durationInMinutes`: `int`

Returns a `Coroutine` for
[GetProgrammaticAccessCredentialsResponseTypeDef](./type_defs.md#getprogrammaticaccesscredentialsresponsetypedef).

<a id="get\_user"></a>

### get_user

Retrieves details for a specific user.

Type annotations for `session.create_client("finspace-data").get_user` method.

Boto3 documentation:
[FinSpaceData.Client.get_user](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.get_user)

Asynchronous method. Use `await get_user(...)` for a synchronous call.

Arguments mapping described in
[GetUserRequestRequestTypeDef](./type_defs.md#getuserrequestrequesttypedef).

Keyword-only arguments:

- `userId`: `str` *(required)*

Returns a `Coroutine` for
[GetUserResponseTypeDef](./type_defs.md#getuserresponsetypedef).

<a id="get\_working\_location"></a>

### get_working_location

A temporary Amazon S3 location, where you can copy your files from a source
location to stage or use as a scratch space in FinSpace notebook.

Type annotations for
`session.create_client("finspace-data").get_working_location` method.

Boto3 documentation:
[FinSpaceData.Client.get_working_location](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.get_working_location)

Asynchronous method. Use `await get_working_location(...)` for a synchronous
call.

Arguments mapping described in
[GetWorkingLocationRequestRequestTypeDef](./type_defs.md#getworkinglocationrequestrequesttypedef).

Keyword-only arguments:

- `locationType`: [locationTypeType](./literals.md#locationtypetype)

Returns a `Coroutine` for
[GetWorkingLocationResponseTypeDef](./type_defs.md#getworkinglocationresponsetypedef).

<a id="list\_changesets"></a>

### list_changesets

Lists the FinSpace Changesets for a Dataset.

Type annotations for `session.create_client("finspace-data").list_changesets`
method.

Boto3 documentation:
[FinSpaceData.Client.list_changesets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.list_changesets)

Asynchronous method. Use `await list_changesets(...)` for a synchronous call.

Arguments mapping described in
[ListChangesetsRequestRequestTypeDef](./type_defs.md#listchangesetsrequestrequesttypedef).

Keyword-only arguments:

- `datasetId`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListChangesetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef).

<a id="list\_data\_views"></a>

### list_data_views

Lists all available Dataviews for a Dataset.

Type annotations for `session.create_client("finspace-data").list_data_views`
method.

Boto3 documentation:
[FinSpaceData.Client.list_data_views](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.list_data_views)

Asynchronous method. Use `await list_data_views(...)` for a synchronous call.

Arguments mapping described in
[ListDataViewsRequestRequestTypeDef](./type_defs.md#listdataviewsrequestrequesttypedef).

Keyword-only arguments:

- `datasetId`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListDataViewsResponseTypeDef](./type_defs.md#listdataviewsresponsetypedef).

<a id="list\_datasets"></a>

### list_datasets

Lists all of the active Datasets that a user has access to.

Type annotations for `session.create_client("finspace-data").list_datasets`
method.

Boto3 documentation:
[FinSpaceData.Client.list_datasets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.list_datasets)

Asynchronous method. Use `await list_datasets(...)` for a synchronous call.

Arguments mapping described in
[ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef).

<a id="list\_permission\_groups"></a>

### list_permission_groups

Lists all available permission groups in FinSpace.

Type annotations for
`session.create_client("finspace-data").list_permission_groups` method.

Boto3 documentation:
[FinSpaceData.Client.list_permission_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.list_permission_groups)

Asynchronous method. Use `await list_permission_groups(...)` for a synchronous
call.

Arguments mapping described in
[ListPermissionGroupsRequestRequestTypeDef](./type_defs.md#listpermissiongroupsrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int` *(required)*
- `nextToken`: `str`

Returns a `Coroutine` for
[ListPermissionGroupsResponseTypeDef](./type_defs.md#listpermissiongroupsresponsetypedef).

<a id="list\_users"></a>

### list_users

Lists all available user accounts in FinSpace.

Type annotations for `session.create_client("finspace-data").list_users`
method.

Boto3 documentation:
[FinSpaceData.Client.list_users](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.list_users)

Asynchronous method. Use `await list_users(...)` for a synchronous call.

Arguments mapping described in
[ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int` *(required)*
- `nextToken`: `str`

Returns a `Coroutine` for
[ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef).

<a id="reset\_user\_password"></a>

### reset_user_password

Resets the password for a specified user ID and generates a temporary one.

Type annotations for
`session.create_client("finspace-data").reset_user_password` method.

Boto3 documentation:
[FinSpaceData.Client.reset_user_password](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.reset_user_password)

Asynchronous method. Use `await reset_user_password(...)` for a synchronous
call.

Arguments mapping described in
[ResetUserPasswordRequestRequestTypeDef](./type_defs.md#resetuserpasswordrequestrequesttypedef).

Keyword-only arguments:

- `userId`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[ResetUserPasswordResponseTypeDef](./type_defs.md#resetuserpasswordresponsetypedef).

<a id="update\_changeset"></a>

### update_changeset

Updates a FinSpace Changeset.

Type annotations for `session.create_client("finspace-data").update_changeset`
method.

Boto3 documentation:
[FinSpaceData.Client.update_changeset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_changeset)

Asynchronous method. Use `await update_changeset(...)` for a synchronous call.

Arguments mapping described in
[UpdateChangesetRequestRequestTypeDef](./type_defs.md#updatechangesetrequestrequesttypedef).

Keyword-only arguments:

- `datasetId`: `str` *(required)*
- `changesetId`: `str` *(required)*
- `sourceParams`: `Mapping`\[`str`, `str`\] *(required)*
- `formatParams`: `Mapping`\[`str`, `str`\] *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[UpdateChangesetResponseTypeDef](./type_defs.md#updatechangesetresponsetypedef).

<a id="update\_dataset"></a>

### update_dataset

Updates a FinSpace Dataset.

Type annotations for `session.create_client("finspace-data").update_dataset`
method.

Boto3 documentation:
[FinSpaceData.Client.update_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_dataset)

Asynchronous method. Use `await update_dataset(...)` for a synchronous call.

Arguments mapping described in
[UpdateDatasetRequestRequestTypeDef](./type_defs.md#updatedatasetrequestrequesttypedef).

Keyword-only arguments:

- `datasetId`: `str` *(required)*
- `datasetTitle`: `str` *(required)*
- `kind`: [DatasetKindType](./literals.md#datasetkindtype) *(required)*
- `clientToken`: `str`
- `datasetDescription`: `str`
- `alias`: `str`
- `schemaDefinition`: [SchemaUnionTypeDef](./type_defs.md#schemauniontypedef)

Returns a `Coroutine` for
[UpdateDatasetResponseTypeDef](./type_defs.md#updatedatasetresponsetypedef).

<a id="update\_permission\_group"></a>

### update_permission_group

Modifies the details of a permission group.

Type annotations for
`session.create_client("finspace-data").update_permission_group` method.

Boto3 documentation:
[FinSpaceData.Client.update_permission_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_permission_group)

Asynchronous method. Use `await update_permission_group(...)` for a synchronous
call.

Arguments mapping described in
[UpdatePermissionGroupRequestRequestTypeDef](./type_defs.md#updatepermissiongrouprequestrequesttypedef).

Keyword-only arguments:

- `permissionGroupId`: `str` *(required)*
- `name`: `str`
- `description`: `str`
- `applicationPermissions`:
  `Sequence`\[[ApplicationPermissionType](./literals.md#applicationpermissiontype)\]
- `clientToken`: `str`

Returns a `Coroutine` for
[UpdatePermissionGroupResponseTypeDef](./type_defs.md#updatepermissiongroupresponsetypedef).

<a id="update\_user"></a>

### update_user

Modifies the details of the specified user account.

Type annotations for `session.create_client("finspace-data").update_user`
method.

Boto3 documentation:
[FinSpaceData.Client.update_user](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_user)

Asynchronous method. Use `await update_user(...)` for a synchronous call.

Arguments mapping described in
[UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef).

Keyword-only arguments:

- `userId`: `str` *(required)*
- `type`: [UserTypeType](./literals.md#usertypetype)
- `firstName`: `str`
- `lastName`: `str`
- `apiAccess`: [ApiAccessType](./literals.md#apiaccesstype)
- `apiAccessPrincipalArn`: `str`
- `clientToken`: `str`

Returns a `Coroutine` for
[UpdateUserResponseTypeDef](./type_defs.md#updateuserresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("finspace-data").__aenter__`
method.

Boto3 documentation:
[FinSpaceData.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [FinSpaceDataClient](#finspacedataclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("finspace-data").__aexit__` method.

Boto3 documentation:
[FinSpaceData.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("finspace-data").get_paginator`
method with overloads.

- `client.get_paginator("list_changesets")` ->
  [ListChangesetsPaginator](./paginators.md#listchangesetspaginator)
- `client.get_paginator("list_data_views")` ->
  [ListDataViewsPaginator](./paginators.md#listdataviewspaginator)
- `client.get_paginator("list_datasets")` ->
  [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
- `client.get_paginator("list_permission_groups")` ->
  [ListPermissionGroupsPaginator](./paginators.md#listpermissiongroupspaginator)
- `client.get_paginator("list_users")` ->
  [ListUsersPaginator](./paginators.md#listuserspaginator)
