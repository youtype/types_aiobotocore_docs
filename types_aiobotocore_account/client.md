<a id="accountclient-for-aiobotocore-account-module"></a>

# AccountClient for aiobotocore Account module

> [Index](..) > [Account](.) > AccountClient

Auto-generated documentation for
[Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
type annotations stubs module
[types-aiobotocore-account](https://pypi.org/project/types-aiobotocore-account/).

- [AccountClient for aiobotocore Account module](#accountclient-for-aiobotocore-account-module)
  - [AccountClient](#accountclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [delete_alternate_contact](#delete_alternate_contact)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_alternate_contact](#get_alternate_contact)
    - [put_alternate_contact](#put_alternate_contact)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)

<a id="accountclient"></a>

## AccountClient

Type annotations for `session.create_client("account")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_account.client import AccountClient

session = get_session()
async with session.create_client("account") as client:
    client: AccountClient
```

Boto3 documentation:
[Account.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_account.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.TooManyRequestsException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

AccountClient exceptions.

Type annotations for `session.create_client("account").exceptions` method.

Boto3 documentation:
[Account.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("account").can_paginate` method.

Boto3 documentation:
[Account.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="delete_alternate_contact"></a>

### delete_alternate_contact

Deletes the specified alternate contact from an Amazon Web Services account.

Type annotations for
`session.create_client("account").delete_alternate_contact` method.

Boto3 documentation:
[Account.Client.delete_alternate_contact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.delete_alternate_contact)

Asynchronous method. Use `await delete_alternate_contact(...)` for a
synchronous call.

Arguments mapping described in
[DeleteAlternateContactRequestRequestTypeDef](./type_defs.md#deletealternatecontactrequestrequesttypedef).

Keyword-only arguments:

- `AlternateContactType`:
  [AlternateContactTypeType](./literals.md#alternatecontacttypetype)
  *(required)*
- `AccountId`: `str`

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("account").generate_presigned_url`
method.

Boto3 documentation:
[Account.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_alternate_contact"></a>

### get_alternate_contact

Retrieves the specified alternate contact attached to an Amazon Web Services
account.

Type annotations for `session.create_client("account").get_alternate_contact`
method.

Boto3 documentation:
[Account.Client.get_alternate_contact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.get_alternate_contact)

Asynchronous method. Use `await get_alternate_contact(...)` for a synchronous
call.

Arguments mapping described in
[GetAlternateContactRequestRequestTypeDef](./type_defs.md#getalternatecontactrequestrequesttypedef).

Keyword-only arguments:

- `AlternateContactType`:
  [AlternateContactTypeType](./literals.md#alternatecontacttypetype)
  *(required)*
- `AccountId`: `str`

Returns a `Coroutine` for
[GetAlternateContactResponseTypeDef](./type_defs.md#getalternatecontactresponsetypedef).

<a id="put_alternate_contact"></a>

### put_alternate_contact

Modifies the specified alternate contact attached to an Amazon Web Services
account.

Type annotations for `session.create_client("account").put_alternate_contact`
method.

Boto3 documentation:
[Account.Client.put_alternate_contact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.put_alternate_contact)

Asynchronous method. Use `await put_alternate_contact(...)` for a synchronous
call.

Arguments mapping described in
[PutAlternateContactRequestRequestTypeDef](./type_defs.md#putalternatecontactrequestrequesttypedef).

Keyword-only arguments:

- `AlternateContactType`:
  [AlternateContactTypeType](./literals.md#alternatecontacttypetype)
  *(required)*
- `EmailAddress`: `str` *(required)*
- `Name`: `str` *(required)*
- `PhoneNumber`: `str` *(required)*
- `Title`: `str` *(required)*
- `AccountId`: `str`

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("account").__aenter__` method.

Boto3 documentation:
[Account.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [AccountClient](#accountclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("account").__aexit__` method.

Boto3 documentation:
[Account.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
