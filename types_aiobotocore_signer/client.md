<a id="signerclient-for-aiobotocore-signer-module"></a>

# signerClient for aiobotocore signer module

> [Index](..) > [signer](.) > signerClient

Auto-generated documentation for
[signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
type annotations stubs module
[types-aiobotocore-signer](https://pypi.org/project/types-aiobotocore-signer/).

- [signerClient for aiobotocore signer module](#signerclient-for-aiobotocore-signer-module)
  - [signerClient](#signerclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [add_profile_permission](#add_profile_permission)
    - [can_paginate](#can_paginate)
    - [cancel_signing_profile](#cancel_signing_profile)
    - [describe_signing_job](#describe_signing_job)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_signing_platform](#get_signing_platform)
    - [get_signing_profile](#get_signing_profile)
    - [list_profile_permissions](#list_profile_permissions)
    - [list_signing_jobs](#list_signing_jobs)
    - [list_signing_platforms](#list_signing_platforms)
    - [list_signing_profiles](#list_signing_profiles)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [put_signing_profile](#put_signing_profile)
    - [remove_profile_permission](#remove_profile_permission)
    - [revoke_signature](#revoke_signature)
    - [revoke_signing_profile](#revoke_signing_profile)
    - [start_signing_job](#start_signing_job)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="signerclient"></a>

## signerClient

Type annotations for `session.create_client("signer")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_signer.client import signerClient

session = get_session()
async with session.create_client("signer") as client:
    client: signerClient
```

Boto3 documentation:
[signer.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_signer.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServiceErrorException`
- `Exceptions.NotFoundException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceLimitExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.TooManyRequestsException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

signerClient exceptions.

Type annotations for `session.create_client("signer").exceptions` method.

Boto3 documentation:
[signer.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="add_profile_permission"></a>

### add_profile_permission

Adds cross-account permissions to a signing profile.

Type annotations for `session.create_client("signer").add_profile_permission`
method.

Boto3 documentation:
[signer.Client.add_profile_permission](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.add_profile_permission)

Asynchronous method. Use `await add_profile_permission(...)` for a synchronous
call.

Arguments mapping described in
[AddProfilePermissionRequestRequestTypeDef](./type_defs.md#addprofilepermissionrequestrequesttypedef).

Keyword-only arguments:

- `profileName`: `str` *(required)*
- `action`: `str` *(required)*
- `principal`: `str` *(required)*
- `statementId`: `str` *(required)*
- `profileVersion`: `str`
- `revisionId`: `str`

Returns a `Coroutine` for
[AddProfilePermissionResponseTypeDef](./type_defs.md#addprofilepermissionresponsetypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("signer").can_paginate` method.

Boto3 documentation:
[signer.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel_signing_profile"></a>

### cancel_signing_profile

Changes the state of an `ACTIVE` signing profile to `CANCELED`.

Type annotations for `session.create_client("signer").cancel_signing_profile`
method.

Boto3 documentation:
[signer.Client.cancel_signing_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.cancel_signing_profile)

Asynchronous method. Use `await cancel_signing_profile(...)` for a synchronous
call.

Arguments mapping described in
[CancelSigningProfileRequestRequestTypeDef](./type_defs.md#cancelsigningprofilerequestrequesttypedef).

Keyword-only arguments:

- `profileName`: `str` *(required)*

<a id="describe_signing_job"></a>

### describe_signing_job

Returns information about a specific code signing job.

Type annotations for `session.create_client("signer").describe_signing_job`
method.

Boto3 documentation:
[signer.Client.describe_signing_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.describe_signing_job)

Asynchronous method. Use `await describe_signing_job(...)` for a synchronous
call.

Arguments mapping described in
[DescribeSigningJobRequestRequestTypeDef](./type_defs.md#describesigningjobrequestrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeSigningJobResponseTypeDef](./type_defs.md#describesigningjobresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("signer").generate_presigned_url`
method.

Boto3 documentation:
[signer.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_signing_platform"></a>

### get_signing_platform

Returns information on a specific signing platform.

Type annotations for `session.create_client("signer").get_signing_platform`
method.

Boto3 documentation:
[signer.Client.get_signing_platform](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_platform)

Asynchronous method. Use `await get_signing_platform(...)` for a synchronous
call.

Arguments mapping described in
[GetSigningPlatformRequestRequestTypeDef](./type_defs.md#getsigningplatformrequestrequesttypedef).

Keyword-only arguments:

- `platformId`: `str` *(required)*

Returns a `Coroutine` for
[GetSigningPlatformResponseTypeDef](./type_defs.md#getsigningplatformresponsetypedef).

<a id="get_signing_profile"></a>

### get_signing_profile

Returns information on a specific signing profile.

Type annotations for `session.create_client("signer").get_signing_profile`
method.

Boto3 documentation:
[signer.Client.get_signing_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_profile)

Asynchronous method. Use `await get_signing_profile(...)` for a synchronous
call.

Arguments mapping described in
[GetSigningProfileRequestRequestTypeDef](./type_defs.md#getsigningprofilerequestrequesttypedef).

Keyword-only arguments:

- `profileName`: `str` *(required)*
- `profileOwner`: `str`

Returns a `Coroutine` for
[GetSigningProfileResponseTypeDef](./type_defs.md#getsigningprofileresponsetypedef).

<a id="list_profile_permissions"></a>

### list_profile_permissions

Lists the cross-account permissions associated with a signing profile.

Type annotations for `session.create_client("signer").list_profile_permissions`
method.

Boto3 documentation:
[signer.Client.list_profile_permissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_profile_permissions)

Asynchronous method. Use `await list_profile_permissions(...)` for a
synchronous call.

Arguments mapping described in
[ListProfilePermissionsRequestRequestTypeDef](./type_defs.md#listprofilepermissionsrequestrequesttypedef).

Keyword-only arguments:

- `profileName`: `str` *(required)*
- `nextToken`: `str`

Returns a `Coroutine` for
[ListProfilePermissionsResponseTypeDef](./type_defs.md#listprofilepermissionsresponsetypedef).

<a id="list_signing_jobs"></a>

### list_signing_jobs

Lists all your signing jobs.

Type annotations for `session.create_client("signer").list_signing_jobs`
method.

Boto3 documentation:
[signer.Client.list_signing_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_jobs)

Asynchronous method. Use `await list_signing_jobs(...)` for a synchronous call.

Arguments mapping described in
[ListSigningJobsRequestRequestTypeDef](./type_defs.md#listsigningjobsrequestrequesttypedef).

Keyword-only arguments:

- `status`: [SigningStatusType](./literals.md#signingstatustype)
- `platformId`: `str`
- `requestedBy`: `str`
- `maxResults`: `int`
- `nextToken`: `str`
- `isRevoked`: `bool`
- `signatureExpiresBefore`: `Union`\[`datetime`, `str`\]
- `signatureExpiresAfter`: `Union`\[`datetime`, `str`\]
- `jobInvoker`: `str`

Returns a `Coroutine` for
[ListSigningJobsResponseTypeDef](./type_defs.md#listsigningjobsresponsetypedef).

<a id="list_signing_platforms"></a>

### list_signing_platforms

Lists all signing platforms available in code signing that match the request
parameters.

Type annotations for `session.create_client("signer").list_signing_platforms`
method.

Boto3 documentation:
[signer.Client.list_signing_platforms](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_platforms)

Asynchronous method. Use `await list_signing_platforms(...)` for a synchronous
call.

Arguments mapping described in
[ListSigningPlatformsRequestRequestTypeDef](./type_defs.md#listsigningplatformsrequestrequesttypedef).

Keyword-only arguments:

- `category`: `str`
- `partner`: `str`
- `target`: `str`
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListSigningPlatformsResponseTypeDef](./type_defs.md#listsigningplatformsresponsetypedef).

<a id="list_signing_profiles"></a>

### list_signing_profiles

Lists all available signing profiles in your AWS account.

Type annotations for `session.create_client("signer").list_signing_profiles`
method.

Boto3 documentation:
[signer.Client.list_signing_profiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_profiles)

Asynchronous method. Use `await list_signing_profiles(...)` for a synchronous
call.

Arguments mapping described in
[ListSigningProfilesRequestRequestTypeDef](./type_defs.md#listsigningprofilesrequestrequesttypedef).

Keyword-only arguments:

- `includeCanceled`: `bool`
- `maxResults`: `int`
- `nextToken`: `str`
- `platformId`: `str`
- `statuses`:
  `Sequence`\[[SigningProfileStatusType](./literals.md#signingprofilestatustype)\]

Returns a `Coroutine` for
[ListSigningProfilesResponseTypeDef](./type_defs.md#listsigningprofilesresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Returns a list of the tags associated with a signing profile resource.

Type annotations for `session.create_client("signer").list_tags_for_resource`
method.

Boto3 documentation:
[signer.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="put_signing_profile"></a>

### put_signing_profile

Creates a signing profile.

Type annotations for `session.create_client("signer").put_signing_profile`
method.

Boto3 documentation:
[signer.Client.put_signing_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.put_signing_profile)

Asynchronous method. Use `await put_signing_profile(...)` for a synchronous
call.

Arguments mapping described in
[PutSigningProfileRequestRequestTypeDef](./type_defs.md#putsigningprofilerequestrequesttypedef).

Keyword-only arguments:

- `profileName`: `str` *(required)*
- `platformId`: `str` *(required)*
- `signingMaterial`:
  [SigningMaterialTypeDef](./type_defs.md#signingmaterialtypedef)
- `signatureValidityPeriod`:
  [SignatureValidityPeriodTypeDef](./type_defs.md#signaturevalidityperiodtypedef)
- `overrides`:
  [SigningPlatformOverridesTypeDef](./type_defs.md#signingplatformoverridestypedef)
- `signingParameters`: `Mapping`\[`str`, `str`\]
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[PutSigningProfileResponseTypeDef](./type_defs.md#putsigningprofileresponsetypedef).

<a id="remove_profile_permission"></a>

### remove_profile_permission

Removes cross-account permissions from a signing profile.

Type annotations for
`session.create_client("signer").remove_profile_permission` method.

Boto3 documentation:
[signer.Client.remove_profile_permission](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.remove_profile_permission)

Asynchronous method. Use `await remove_profile_permission(...)` for a
synchronous call.

Arguments mapping described in
[RemoveProfilePermissionRequestRequestTypeDef](./type_defs.md#removeprofilepermissionrequestrequesttypedef).

Keyword-only arguments:

- `profileName`: `str` *(required)*
- `revisionId`: `str` *(required)*
- `statementId`: `str` *(required)*

Returns a `Coroutine` for
[RemoveProfilePermissionResponseTypeDef](./type_defs.md#removeprofilepermissionresponsetypedef).

<a id="revoke_signature"></a>

### revoke_signature

Changes the state of a signing job to REVOKED.

Type annotations for `session.create_client("signer").revoke_signature` method.

Boto3 documentation:
[signer.Client.revoke_signature](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signature)

Asynchronous method. Use `await revoke_signature(...)` for a synchronous call.

Arguments mapping described in
[RevokeSignatureRequestRequestTypeDef](./type_defs.md#revokesignaturerequestrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*
- `reason`: `str` *(required)*
- `jobOwner`: `str`

<a id="revoke_signing_profile"></a>

### revoke_signing_profile

Changes the state of a signing profile to REVOKED.

Type annotations for `session.create_client("signer").revoke_signing_profile`
method.

Boto3 documentation:
[signer.Client.revoke_signing_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signing_profile)

Asynchronous method. Use `await revoke_signing_profile(...)` for a synchronous
call.

Arguments mapping described in
[RevokeSigningProfileRequestRequestTypeDef](./type_defs.md#revokesigningprofilerequestrequesttypedef).

Keyword-only arguments:

- `profileName`: `str` *(required)*
- `profileVersion`: `str` *(required)*
- `reason`: `str` *(required)*
- `effectiveTime`: `Union`\[`datetime`, `str`\] *(required)*

<a id="start_signing_job"></a>

### start_signing_job

Initiates a signing job to be performed on the code provided.

Type annotations for `session.create_client("signer").start_signing_job`
method.

Boto3 documentation:
[signer.Client.start_signing_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.start_signing_job)

Asynchronous method. Use `await start_signing_job(...)` for a synchronous call.

Arguments mapping described in
[StartSigningJobRequestRequestTypeDef](./type_defs.md#startsigningjobrequestrequesttypedef).

Keyword-only arguments:

- `source`: [SourceTypeDef](./type_defs.md#sourcetypedef) *(required)*
- `destination`: [DestinationTypeDef](./type_defs.md#destinationtypedef)
  *(required)*
- `profileName`: `str` *(required)*
- `clientRequestToken`: `str` *(required)*
- `profileOwner`: `str`

Returns a `Coroutine` for
[StartSigningJobResponseTypeDef](./type_defs.md#startsigningjobresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Adds one or more tags to a signing profile.

Type annotations for `session.create_client("signer").tag_resource` method.

Boto3 documentation:
[signer.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes one or more tags from a signing profile.

Type annotations for `session.create_client("signer").untag_resource` method.

Boto3 documentation:
[signer.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("signer").__aenter__` method.

Boto3 documentation:
[signer.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [signerClient](#signerclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("signer").__aexit__` method.

Boto3 documentation:
[signer.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("signer").get_paginator` method
with overloads.

- `client.get_paginator("list_signing_jobs")` ->
  [ListSigningJobsPaginator](./paginators.md#listsigningjobspaginator)
- `client.get_paginator("list_signing_platforms")` ->
  [ListSigningPlatformsPaginator](./paginators.md#listsigningplatformspaginator)
- `client.get_paginator("list_signing_profiles")` ->
  [ListSigningProfilesPaginator](./paginators.md#listsigningprofilespaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("signer").get_waiter` method with
overloads.

- `client.get_waiter("successful_signing_job")` ->
  [SuccessfulSigningJobWaiter](./waiters.md#successfulsigningjobwaiter)
