<a id="qldbsessionclient-for-aiobotocore-qldbsession-module"></a>

# QLDBSessionClient for aiobotocore QLDBSession module

> [Index](../README.md) > [QLDBSession](./README.md) > QLDBSessionClient

Auto-generated documentation for
[QLDBSession](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
type annotations stubs module
[types-aiobotocore-qldb-session](https://pypi.org/project/types-aiobotocore-qldb-session/).

- [QLDBSessionClient for aiobotocore QLDBSession module](#qldbsessionclient-for-aiobotocore-qldbsession-module)
  - [QLDBSessionClient](#qldbsessionclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [generate_presigned_url](#generate_presigned_url)
    - [send_command](#send_command)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="qldbsessionclient"></a>

## QLDBSessionClient

Type annotations for `session.create_client("qldb-session")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_qldb_session.client import QLDBSessionClient

session = get_session()
async with session.create_client("qldb-session") as client:
    client: QLDBSessionClient
```

Boto3 documentation:
[QLDBSession.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_qldb_session.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.CapacityExceededException`
- `Exceptions.ClientError`
- `Exceptions.InvalidSessionException`
- `Exceptions.LimitExceededException`
- `Exceptions.OccConflictException`
- `Exceptions.RateExceededException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

QLDBSessionClient exceptions.

Type annotations for `session.create_client("qldb-session").exceptions` method.

Boto3 documentation:
[QLDBSession.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("qldb-session").can_paginate`
method.

Boto3 documentation:
[QLDBSession.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("qldb-session").generate_presigned_url` method.

Boto3 documentation:
[QLDBSession.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="send\_command"></a>

### send_command

Sends a command to an Amazon QLDB ledger.

Type annotations for `session.create_client("qldb-session").send_command`
method.

Boto3 documentation:
[QLDBSession.Client.send_command](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.send_command)

Asynchronous method. Use `await send_command(...)` for a synchronous call.

Arguments mapping described in
[SendCommandRequestRequestTypeDef](./type_defs.md#sendcommandrequestrequesttypedef).

Keyword-only arguments:

- `SessionToken`: `str`
- `StartSession`:
  [StartSessionRequestTypeDef](./type_defs.md#startsessionrequesttypedef)
- `StartTransaction`: `Mapping`\[`str`, `Any`\]
- `EndSession`: `Mapping`\[`str`, `Any`\]
- `CommitTransaction`:
  [CommitTransactionRequestTypeDef](./type_defs.md#committransactionrequesttypedef)
- `AbortTransaction`: `Mapping`\[`str`, `Any`\]
- `ExecuteStatement`:
  [ExecuteStatementRequestTypeDef](./type_defs.md#executestatementrequesttypedef)
- `FetchPage`:
  [FetchPageRequestTypeDef](./type_defs.md#fetchpagerequesttypedef)

Returns a `Coroutine` for
[SendCommandResultTypeDef](./type_defs.md#sendcommandresulttypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("qldb-session").__aenter__` method.

Boto3 documentation:
[QLDBSession.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [QLDBSessionClient](#qldbsessionclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("qldb-session").__aexit__` method.

Boto3 documentation:
[QLDBSession.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
