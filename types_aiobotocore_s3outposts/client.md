<a id="s3outpostsclient-for-aiobotocore-s3outposts-module"></a>

# S3OutpostsClient for aiobotocore S3Outposts module

> [Index](..) > [S3Outposts](.) > S3OutpostsClient

Auto-generated documentation for
[S3Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
type annotations stubs module
[types-aiobotocore-s3outposts](https://pypi.org/project/types-aiobotocore-s3outposts/).

- [S3OutpostsClient for aiobotocore S3Outposts module](#s3outpostsclient-for-aiobotocore-s3outposts-module)
  - [S3OutpostsClient](#s3outpostsclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_endpoint](#create_endpoint)
    - [delete_endpoint](#delete_endpoint)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_endpoints](#list_endpoints)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="s3outpostsclient"></a>

## S3OutpostsClient

Type annotations for `session.create_client("s3outposts")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_s3outposts.client import S3OutpostsClient

session = get_session()
async with session.create_client("s3outposts") as client:
    client: S3OutpostsClient
```

Boto3 documentation:
[S3Outposts.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_s3outposts.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

S3OutpostsClient exceptions.

Type annotations for `session.create_client("s3outposts").exceptions` method.

Boto3 documentation:
[S3Outposts.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("s3outposts").can_paginate` method.

Boto3 documentation:
[S3Outposts.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_endpoint"></a>

### create_endpoint

Amazon S3 on Outposts Access Points simplify managing data access at scale for
shared datasets in S3 on Outposts.

Type annotations for `session.create_client("s3outposts").create_endpoint`
method.

Boto3 documentation:
[S3Outposts.Client.create_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.create_endpoint)

Asynchronous method. Use `await create_endpoint(...)` for a synchronous call.

Arguments mapping described in
[CreateEndpointRequestRequestTypeDef](./type_defs.md#createendpointrequestrequesttypedef).

Keyword-only arguments:

- `OutpostId`: `str` *(required)*
- `SubnetId`: `str` *(required)*
- `SecurityGroupId`: `str` *(required)*
- `AccessType`: [EndpointAccessTypeType](./literals.md#endpointaccesstypetype)
- `CustomerOwnedIpv4Pool`: `str`

Returns a `Coroutine` for
[CreateEndpointResultTypeDef](./type_defs.md#createendpointresulttypedef).

<a id="delete_endpoint"></a>

### delete_endpoint

Amazon S3 on Outposts Access Points simplify managing data access at scale for
shared datasets in S3 on Outposts.

Type annotations for `session.create_client("s3outposts").delete_endpoint`
method.

Boto3 documentation:
[S3Outposts.Client.delete_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.delete_endpoint)

Asynchronous method. Use `await delete_endpoint(...)` for a synchronous call.

Arguments mapping described in
[DeleteEndpointRequestRequestTypeDef](./type_defs.md#deleteendpointrequestrequesttypedef).

Keyword-only arguments:

- `EndpointId`: `str` *(required)*
- `OutpostId`: `str` *(required)*

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("s3outposts").generate_presigned_url` method.

Boto3 documentation:
[S3Outposts.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_endpoints"></a>

### list_endpoints

Amazon S3 on Outposts Access Points simplify managing data access at scale for
shared datasets in S3 on Outposts.

Type annotations for `session.create_client("s3outposts").list_endpoints`
method.

Boto3 documentation:
[S3Outposts.Client.list_endpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.list_endpoints)

Asynchronous method. Use `await list_endpoints(...)` for a synchronous call.

Arguments mapping described in
[ListEndpointsRequestRequestTypeDef](./type_defs.md#listendpointsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListEndpointsResultTypeDef](./type_defs.md#listendpointsresulttypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("s3outposts").__aenter__` method.

Boto3 documentation:
[S3Outposts.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [S3OutpostsClient](#s3outpostsclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("s3outposts").__aexit__` method.

Boto3 documentation:
[S3Outposts.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("s3outposts").get_paginator` method
with overloads.

- `client.get_paginator("list_endpoints")` ->
  [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
