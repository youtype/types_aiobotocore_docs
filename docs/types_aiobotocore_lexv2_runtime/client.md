<a id="lexruntimev2client-for-aiobotocore-lexruntimev2-module"></a>

# LexRuntimeV2Client for aiobotocore LexRuntimeV2 module

> [Index](../README.md) > [LexRuntimeV2](./README.md) > LexRuntimeV2Client

Auto-generated documentation for
[LexRuntimeV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
type annotations stubs module
[types-aiobotocore-lexv2-runtime](https://pypi.org/project/types-aiobotocore-lexv2-runtime/).

- [LexRuntimeV2Client for aiobotocore LexRuntimeV2 module](#lexruntimev2client-for-aiobotocore-lexruntimev2-module)
  - [LexRuntimeV2Client](#lexruntimev2client)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [delete_session](#delete_session)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_session](#get_session)
    - [put_session](#put_session)
    - [recognize_text](#recognize_text)
    - [recognize_utterance](#recognize_utterance)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="lexruntimev2client"></a>

## LexRuntimeV2Client

Type annotations for `session.create_client("lexv2-runtime")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_lexv2_runtime.client import LexRuntimeV2Client

session = get_session()
async with session.create_client("lexv2-runtime") as client:
    client: LexRuntimeV2Client
```

Boto3 documentation:
[LexRuntimeV2.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_lexv2_runtime.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.BadGatewayException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.DependencyFailedException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

LexRuntimeV2Client exceptions.

Type annotations for `session.create_client("lexv2-runtime").exceptions`
method.

Boto3 documentation:
[LexRuntimeV2.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("lexv2-runtime").can_paginate`
method.

Boto3 documentation:
[LexRuntimeV2.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="delete\_session"></a>

### delete_session

Removes session information for a specified bot, alias, and user ID.

Type annotations for `session.create_client("lexv2-runtime").delete_session`
method.

Boto3 documentation:
[LexRuntimeV2.Client.delete_session](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.delete_session)

Asynchronous method. Use `await delete_session(...)` for a synchronous call.

Arguments mapping described in
[DeleteSessionRequestRequestTypeDef](./type_defs.md#deletesessionrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botAliasId`: `str` *(required)*
- `localeId`: `str` *(required)*
- `sessionId`: `str` *(required)*

Returns a `Coroutine` for
[DeleteSessionResponseTypeDef](./type_defs.md#deletesessionresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("lexv2-runtime").generate_presigned_url` method.

Boto3 documentation:
[LexRuntimeV2.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_session"></a>

### get_session

Returns session information for a specified bot, alias, and user.

Type annotations for `session.create_client("lexv2-runtime").get_session`
method.

Boto3 documentation:
[LexRuntimeV2.Client.get_session](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.get_session)

Asynchronous method. Use `await get_session(...)` for a synchronous call.

Arguments mapping described in
[GetSessionRequestRequestTypeDef](./type_defs.md#getsessionrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botAliasId`: `str` *(required)*
- `localeId`: `str` *(required)*
- `sessionId`: `str` *(required)*

Returns a `Coroutine` for
[GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef).

<a id="put\_session"></a>

### put_session

Creates a new session or modifies an existing session with an Amazon Lex V2
bot.

Type annotations for `session.create_client("lexv2-runtime").put_session`
method.

Boto3 documentation:
[LexRuntimeV2.Client.put_session](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.put_session)

Asynchronous method. Use `await put_session(...)` for a synchronous call.

Arguments mapping described in
[PutSessionRequestRequestTypeDef](./type_defs.md#putsessionrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botAliasId`: `str` *(required)*
- `localeId`: `str` *(required)*
- `sessionId`: `str` *(required)*
- `sessionState`: [SessionStateTypeDef](./type_defs.md#sessionstatetypedef)
  *(required)*
- `messages`: `Sequence`\[[MessageTypeDef](./type_defs.md#messagetypedef)\]
- `requestAttributes`: `Mapping`\[`str`, `str`\]
- `responseContentType`: `str`

Returns a `Coroutine` for
[PutSessionResponseTypeDef](./type_defs.md#putsessionresponsetypedef).

<a id="recognize\_text"></a>

### recognize_text

Sends user input to Amazon Lex V2.

Type annotations for `session.create_client("lexv2-runtime").recognize_text`
method.

Boto3 documentation:
[LexRuntimeV2.Client.recognize_text](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_text)

Asynchronous method. Use `await recognize_text(...)` for a synchronous call.

Arguments mapping described in
[RecognizeTextRequestRequestTypeDef](./type_defs.md#recognizetextrequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botAliasId`: `str` *(required)*
- `localeId`: `str` *(required)*
- `sessionId`: `str` *(required)*
- `text`: `str` *(required)*
- `sessionState`: [SessionStateTypeDef](./type_defs.md#sessionstatetypedef)
- `requestAttributes`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[RecognizeTextResponseTypeDef](./type_defs.md#recognizetextresponsetypedef).

<a id="recognize\_utterance"></a>

### recognize_utterance

Sends user input to Amazon Lex V2.

Type annotations for
`session.create_client("lexv2-runtime").recognize_utterance` method.

Boto3 documentation:
[LexRuntimeV2.Client.recognize_utterance](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_utterance)

Asynchronous method. Use `await recognize_utterance(...)` for a synchronous
call.

Arguments mapping described in
[RecognizeUtteranceRequestRequestTypeDef](./type_defs.md#recognizeutterancerequestrequesttypedef).

Keyword-only arguments:

- `botId`: `str` *(required)*
- `botAliasId`: `str` *(required)*
- `localeId`: `str` *(required)*
- `sessionId`: `str` *(required)*
- `requestContentType`: `str` *(required)*
- `sessionState`: `str`
- `requestAttributes`: `str`
- `responseContentType`: `str`
- `inputStream`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]

Returns a `Coroutine` for
[RecognizeUtteranceResponseTypeDef](./type_defs.md#recognizeutteranceresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("lexv2-runtime").__aenter__`
method.

Boto3 documentation:
[LexRuntimeV2.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [LexRuntimeV2Client](#lexruntimev2client).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("lexv2-runtime").__aexit__` method.

Boto3 documentation:
[LexRuntimeV2.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.