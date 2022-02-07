<a id="finspaceclient-for-aiobotocore-finspace-module"></a>

# finspaceClient for aiobotocore finspace module

> [Index](..) > [finspace](.) > finspaceClient

Auto-generated documentation for
[finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
type annotations stubs module
[types-aiobotocore-finspace](https://pypi.org/project/types-aiobotocore-finspace/).

- [finspaceClient for aiobotocore finspace module](#finspaceclient-for-aiobotocore-finspace-module)
  - [finspaceClient](#finspaceclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_environment](#create_environment)
    - [delete_environment](#delete_environment)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_environment](#get_environment)
    - [list_environments](#list_environments)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_environment](#update_environment)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)

<a id="finspaceclient"></a>

## finspaceClient

Type annotations for `session.create_client("finspace")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_finspace.client import finspaceClient

session = get_session()
async with session.create_client("finspace") as client:
    client: finspaceClient
```

Boto3 documentation:
[finspace.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_finspace.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.InternalServerException`
- `Exceptions.InvalidRequestException`
- `Exceptions.LimitExceededException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

finspaceClient exceptions.

Type annotations for `session.create_client("finspace").exceptions` method.

Boto3 documentation:
[finspace.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("finspace").can_paginate` method.

Boto3 documentation:
[finspace.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_environment"></a>

### create_environment

Create a new FinSpace environment.

Type annotations for `session.create_client("finspace").create_environment`
method.

Boto3 documentation:
[finspace.Client.create_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_environment)

Asynchronous method. Use `await create_environment(...)` for a synchronous
call.

Arguments mapping described in
[CreateEnvironmentRequestRequestTypeDef](./type_defs.md#createenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `description`: `str`
- `kmsKeyId`: `str`
- `tags`: `Mapping`\[`str`, `str`\]
- `federationMode`: [FederationModeType](./literals.md#federationmodetype)
- `federationParameters`:
  [FederationParametersTypeDef](./type_defs.md#federationparameterstypedef)
- `superuserParameters`:
  [SuperuserParametersTypeDef](./type_defs.md#superuserparameterstypedef)
- `dataBundles`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef).

<a id="delete_environment"></a>

### delete_environment

Delete an FinSpace environment.

Type annotations for `session.create_client("finspace").delete_environment`
method.

Boto3 documentation:
[finspace.Client.delete_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_environment)

Asynchronous method. Use `await delete_environment(...)` for a synchronous
call.

Arguments mapping described in
[DeleteEnvironmentRequestRequestTypeDef](./type_defs.md#deleteenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `environmentId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("finspace").generate_presigned_url`
method.

Boto3 documentation:
[finspace.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_environment"></a>

### get_environment

Returns the FinSpace environment object.

Type annotations for `session.create_client("finspace").get_environment`
method.

Boto3 documentation:
[finspace.Client.get_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_environment)

Asynchronous method. Use `await get_environment(...)` for a synchronous call.

Arguments mapping described in
[GetEnvironmentRequestRequestTypeDef](./type_defs.md#getenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `environmentId`: `str` *(required)*

Returns a `Coroutine` for
[GetEnvironmentResponseTypeDef](./type_defs.md#getenvironmentresponsetypedef).

<a id="list_environments"></a>

### list_environments

A list of all of your FinSpace environments.

Type annotations for `session.create_client("finspace").list_environments`
method.

Boto3 documentation:
[finspace.Client.list_environments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_environments)

Asynchronous method. Use `await list_environments(...)` for a synchronous call.

Arguments mapping described in
[ListEnvironmentsRequestRequestTypeDef](./type_defs.md#listenvironmentsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

A list of all tags for a resource.

Type annotations for `session.create_client("finspace").list_tags_for_resource`
method.

Boto3 documentation:
[finspace.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Adds metadata tags to a FinSpace resource.

Type annotations for `session.create_client("finspace").tag_resource` method.

Boto3 documentation:
[finspace.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes metadata tags from a FinSpace resource.

Type annotations for `session.create_client("finspace").untag_resource` method.

Boto3 documentation:
[finspace.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_environment"></a>

### update_environment

Update your FinSpace environment.

Type annotations for `session.create_client("finspace").update_environment`
method.

Boto3 documentation:
[finspace.Client.update_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_environment)

Asynchronous method. Use `await update_environment(...)` for a synchronous
call.

Arguments mapping described in
[UpdateEnvironmentRequestRequestTypeDef](./type_defs.md#updateenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `environmentId`: `str` *(required)*
- `name`: `str`
- `description`: `str`
- `federationMode`: [FederationModeType](./literals.md#federationmodetype)
- `federationParameters`:
  [FederationParametersTypeDef](./type_defs.md#federationparameterstypedef)

Returns a `Coroutine` for
[UpdateEnvironmentResponseTypeDef](./type_defs.md#updateenvironmentresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("finspace").__aenter__` method.

Boto3 documentation:
[finspace.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [finspaceClient](#finspaceclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("finspace").__aexit__` method.

Boto3 documentation:
[finspace.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
