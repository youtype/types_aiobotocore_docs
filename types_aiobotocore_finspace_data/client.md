<a id="finspacedataclient-for-aiobotocore-finspacedata-module"></a>

# FinSpaceDataClient for aiobotocore FinSpaceData module

> [Index](..) > [FinSpaceData](.) > FinSpaceDataClient

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
    - [delete_dataset](#delete_dataset)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_changeset](#get_changeset)
    - [get_data_view](#get_data_view)
    - [get_dataset](#get_dataset)
    - [get_programmatic_access_credentials](#get_programmatic_access_credentials)
    - [get_working_location](#get_working_location)
    - [list_changesets](#list_changesets)
    - [list_data_views](#list_data_views)
    - [list_datasets](#list_datasets)
    - [update_changeset](#update_changeset)
    - [update_dataset](#update_dataset)
    - [get_paginator](#get_paginator)

<a id="finspacedataclient"></a>

## FinSpaceDataClient

Type annotations for `aiobotocore.create_client("finspace-data")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_finspace_data.client import FinSpaceDataClient

def get_finspace-data_client() -> FinSpaceDataClient:
    return Session().client("finspace-data")
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

Type annotations for `aiobotocore.create_client("finspace-data").exceptions`
method.

Boto3 documentation:
[FinSpaceData.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("finspace-data").can_paginate`
method.

Boto3 documentation:
[FinSpaceData.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_changeset"></a>

### create_changeset

Creates a new Changeset in a FinSpace Dataset.

Type annotations for
`aiobotocore.create_client("finspace-data").create_changeset` method.

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

<a id="create_data_view"></a>

### create_data_view

Creates a Dataview for a Dataset.

Type annotations for
`aiobotocore.create_client("finspace-data").create_data_view` method.

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

<a id="create_dataset"></a>

### create_dataset

Creates a new FinSpace Dataset.

Type annotations for
`aiobotocore.create_client("finspace-data").create_dataset` method.

Boto3 documentation:
[FinSpaceData.Client.create_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_dataset)

Asynchronous method. Use `await create_dataset(...)` for a synchronous call.

Arguments mapping described in
[CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef).

Keyword-only arguments:

- `datasetTitle`: `str` *(required)*
- `kind`: [DatasetKindType](./literals.md#datasetkindtype) *(required)*
- `datasetDescription`: `str` *(required)*
- `permissionGroupParams`:
  [PermissionGroupParamsTypeDef](./type_defs.md#permissiongroupparamstypedef)
  *(required)*
- `alias`: `str` *(required)*
- `clientToken`: `str`
- `ownerInfo`:
  [DatasetOwnerInfoTypeDef](./type_defs.md#datasetownerinfotypedef)
- `schemaDefinition`: [SchemaUnionTypeDef](./type_defs.md#schemauniontypedef)

Returns a `Coroutine` for
[CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef).

<a id="delete_dataset"></a>

### delete_dataset

Deletes a FinSpace Dataset.

Type annotations for
`aiobotocore.create_client("finspace-data").delete_dataset` method.

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

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("finspace-data").generate_presigned_url` method.

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

<a id="get_changeset"></a>

### get_changeset

Get information about a Changeset.

Type annotations for `aiobotocore.create_client("finspace-data").get_changeset`
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

<a id="get_data_view"></a>

### get_data_view

Gets information about a Dataview.

Type annotations for `aiobotocore.create_client("finspace-data").get_data_view`
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

<a id="get_dataset"></a>

### get_dataset

Returns information about a Dataset.

Type annotations for `aiobotocore.create_client("finspace-data").get_dataset`
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

<a id="get_programmatic_access_credentials"></a>

### get_programmatic_access_credentials

Request programmatic credentials to use with FinSpace SDK.

Type annotations for
`aiobotocore.create_client("finspace-data").get_programmatic_access_credentials`
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

<a id="get_working_location"></a>

### get_working_location

A temporary Amazon S3 location, where you can copy your files from a source
location to stage or use as a scratch space in FinSpace notebook.

Type annotations for
`aiobotocore.create_client("finspace-data").get_working_location` method.

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

<a id="list_changesets"></a>

### list_changesets

Lists the FinSpace Changesets for a Dataset.

Type annotations for
`aiobotocore.create_client("finspace-data").list_changesets` method.

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

<a id="list_data_views"></a>

### list_data_views

Lists all available Dataviews for a Dataset.

Type annotations for
`aiobotocore.create_client("finspace-data").list_data_views` method.

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

<a id="list_datasets"></a>

### list_datasets

Lists all of the active Datasets that a user has access to.

Type annotations for `aiobotocore.create_client("finspace-data").list_datasets`
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

<a id="update_changeset"></a>

### update_changeset

Updates a FinSpace Changeset.

Type annotations for
`aiobotocore.create_client("finspace-data").update_changeset` method.

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

<a id="update_dataset"></a>

### update_dataset

Updates a FinSpace Dataset.

Type annotations for
`aiobotocore.create_client("finspace-data").update_dataset` method.

Boto3 documentation:
[FinSpaceData.Client.update_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_dataset)

Asynchronous method. Use `await update_dataset(...)` for a synchronous call.

Arguments mapping described in
[UpdateDatasetRequestRequestTypeDef](./type_defs.md#updatedatasetrequestrequesttypedef).

Keyword-only arguments:

- `datasetId`: `str` *(required)*
- `datasetTitle`: `str` *(required)*
- `kind`: [DatasetKindType](./literals.md#datasetkindtype) *(required)*
- `alias`: `str` *(required)*
- `clientToken`: `str`
- `datasetDescription`: `str`
- `schemaDefinition`: [SchemaUnionTypeDef](./type_defs.md#schemauniontypedef)

Returns a `Coroutine` for
[UpdateDatasetResponseTypeDef](./type_defs.md#updatedatasetresponsetypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("finspace-data").get_paginator`
method with overloads.

- `client.get_paginator("list_changesets")` ->
  [ListChangesetsPaginator](./paginators.md#listchangesetspaginator)
- `client.get_paginator("list_data_views")` ->
  [ListDataViewsPaginator](./paginators.md#listdataviewspaginator)
- `client.get_paginator("list_datasets")` ->
  [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
