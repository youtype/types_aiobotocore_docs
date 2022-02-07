<a id="importexportclient-for-aiobotocore-importexport-module"></a>

# ImportExportClient for aiobotocore ImportExport module

> [Index](..) > [ImportExport](.) > ImportExportClient

Auto-generated documentation for
[ImportExport](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
type annotations stubs module
[types-aiobotocore-importexport](https://pypi.org/project/types-aiobotocore-importexport/).

- [ImportExportClient for aiobotocore ImportExport module](#importexportclient-for-aiobotocore-importexport-module)
  - [ImportExportClient](#importexportclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [cancel_job](#cancel_job)
    - [create_job](#create_job)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_shipping_label](#get_shipping_label)
    - [get_status](#get_status)
    - [list_jobs](#list_jobs)
    - [update_job](#update_job)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="importexportclient"></a>

## ImportExportClient

Type annotations for `session.create_client("importexport")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_importexport.client import ImportExportClient

session = get_session()
async with session.create_client("importexport") as client:
    client: ImportExportClient
```

Boto3 documentation:
[ImportExport.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_importexport.client import Exceptions

def handle_error(exc: Exceptions.BucketPermissionException) -> None:
    ...
```

Exceptions:

- `Exceptions.BucketPermissionException`
- `Exceptions.CanceledJobIdException`
- `Exceptions.ClientError`
- `Exceptions.CreateJobQuotaExceededException`
- `Exceptions.ExpiredJobIdException`
- `Exceptions.InvalidAccessKeyIdException`
- `Exceptions.InvalidAddressException`
- `Exceptions.InvalidCustomsException`
- `Exceptions.InvalidFileSystemException`
- `Exceptions.InvalidJobIdException`
- `Exceptions.InvalidManifestFieldException`
- `Exceptions.InvalidParameterException`
- `Exceptions.InvalidVersionException`
- `Exceptions.MalformedManifestException`
- `Exceptions.MissingCustomsException`
- `Exceptions.MissingManifestFieldException`
- `Exceptions.MissingParameterException`
- `Exceptions.MultipleRegionsException`
- `Exceptions.NoSuchBucketException`
- `Exceptions.UnableToCancelJobIdException`
- `Exceptions.UnableToUpdateJobIdException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ImportExportClient exceptions.

Type annotations for `session.create_client("importexport").exceptions` method.

Boto3 documentation:
[ImportExport.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("importexport").can_paginate`
method.

Boto3 documentation:
[ImportExport.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel_job"></a>

### cancel_job

This operation cancels a specified job.

Type annotations for `session.create_client("importexport").cancel_job` method.

Boto3 documentation:
[ImportExport.Client.cancel_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.cancel_job)

Asynchronous method. Use `await cancel_job(...)` for a synchronous call.

Arguments mapping described in
[CancelJobInputRequestTypeDef](./type_defs.md#canceljobinputrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*
- `APIVersion`: `str`

Returns a `Coroutine` for
[CancelJobOutputTypeDef](./type_defs.md#canceljoboutputtypedef).

<a id="create_job"></a>

### create_job

This operation initiates the process of scheduling an upload or download of
your data.

Type annotations for `session.create_client("importexport").create_job` method.

Boto3 documentation:
[ImportExport.Client.create_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.create_job)

Asynchronous method. Use `await create_job(...)` for a synchronous call.

Arguments mapping described in
[CreateJobInputRequestTypeDef](./type_defs.md#createjobinputrequesttypedef).

Keyword-only arguments:

- `JobType`: [JobTypeType](./literals.md#jobtypetype) *(required)*
- `Manifest`: `str` *(required)*
- `ValidateOnly`: `bool` *(required)*
- `ManifestAddendum`: `str`
- `APIVersion`: `str`

Returns a `Coroutine` for
[CreateJobOutputTypeDef](./type_defs.md#createjoboutputtypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("importexport").generate_presigned_url` method.

Boto3 documentation:
[ImportExport.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_shipping_label"></a>

### get_shipping_label

This operation generates a pre-paid UPS shipping label that you will use to
ship your device to AWS for processing.

Type annotations for `session.create_client("importexport").get_shipping_label`
method.

Boto3 documentation:
[ImportExport.Client.get_shipping_label](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.get_shipping_label)

Asynchronous method. Use `await get_shipping_label(...)` for a synchronous
call.

Arguments mapping described in
[GetShippingLabelInputRequestTypeDef](./type_defs.md#getshippinglabelinputrequesttypedef).

Keyword-only arguments:

- `jobIds`: `Sequence`\[`str`\] *(required)*
- `name`: `str`
- `company`: `str`
- `phoneNumber`: `str`
- `country`: `str`
- `stateOrProvince`: `str`
- `city`: `str`
- `postalCode`: `str`
- `street1`: `str`
- `street2`: `str`
- `street3`: `str`
- `APIVersion`: `str`

Returns a `Coroutine` for
[GetShippingLabelOutputTypeDef](./type_defs.md#getshippinglabeloutputtypedef).

<a id="get_status"></a>

### get_status

This operation returns information about a job, including where the job is in
the processing pipeline, the status of the results, and the signature value
associated with the job.

Type annotations for `session.create_client("importexport").get_status` method.

Boto3 documentation:
[ImportExport.Client.get_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.get_status)

Asynchronous method. Use `await get_status(...)` for a synchronous call.

Arguments mapping described in
[GetStatusInputRequestTypeDef](./type_defs.md#getstatusinputrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*
- `APIVersion`: `str`

Returns a `Coroutine` for
[GetStatusOutputTypeDef](./type_defs.md#getstatusoutputtypedef).

<a id="list_jobs"></a>

### list_jobs

This operation returns the jobs associated with the requester.

Type annotations for `session.create_client("importexport").list_jobs` method.

Boto3 documentation:
[ImportExport.Client.list_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.list_jobs)

Asynchronous method. Use `await list_jobs(...)` for a synchronous call.

Arguments mapping described in
[ListJobsInputRequestTypeDef](./type_defs.md#listjobsinputrequesttypedef).

Keyword-only arguments:

- `MaxJobs`: `int`
- `Marker`: `str`
- `APIVersion`: `str`

Returns a `Coroutine` for
[ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef).

<a id="update_job"></a>

### update_job

You use this operation to change the parameters specified in the original
manifest file by supplying a new manifest file.

Type annotations for `session.create_client("importexport").update_job` method.

Boto3 documentation:
[ImportExport.Client.update_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.update_job)

Asynchronous method. Use `await update_job(...)` for a synchronous call.

Arguments mapping described in
[UpdateJobInputRequestTypeDef](./type_defs.md#updatejobinputrequesttypedef).

Keyword-only arguments:

- `JobId`: `str` *(required)*
- `Manifest`: `str` *(required)*
- `JobType`: [JobTypeType](./literals.md#jobtypetype) *(required)*
- `ValidateOnly`: `bool` *(required)*
- `APIVersion`: `str`

Returns a `Coroutine` for
[UpdateJobOutputTypeDef](./type_defs.md#updatejoboutputtypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("importexport").__aenter__` method.

Boto3 documentation:
[ImportExport.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [ImportExportClient](#importexportclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("importexport").__aexit__` method.

Boto3 documentation:
[ImportExport.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("importexport").get_paginator`
method with overloads.

- `client.get_paginator("list_jobs")` ->
  [ListJobsPaginator](./paginators.md#listjobspaginator)
