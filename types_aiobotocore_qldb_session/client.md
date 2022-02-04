<a id="qldbsessionclient-for-aiobotocore-qldbsession-module"></a>

# QLDBSessionClient for aiobotocore QLDBSession module

> [Index](..) > [QLDBSession](.) > QLDBSessionClient

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

<a id="qldbsessionclient"></a>

## QLDBSessionClient

Type annotations for `aiobotocore.create_client("qldb-session")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_qldb_session.client import QLDBSessionClient

def get_qldb-session_client() -> QLDBSessionClient:
    return Session().client("qldb-session")
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

Type annotations for `aiobotocore.create_client("qldb-session").exceptions`
method.

Boto3 documentation:
[QLDBSession.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("qldb-session").can_paginate`
method.

Boto3 documentation:
[QLDBSession.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("qldb-session").generate_presigned_url` method.

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

<a id="send_command"></a>

### send_command

Sends a command to an Amazon QLDB ledger.

Type annotations for `aiobotocore.create_client("qldb-session").send_command`
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
