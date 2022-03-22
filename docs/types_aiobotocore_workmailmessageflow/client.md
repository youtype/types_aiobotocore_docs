<a id="workmailmessageflowclient-for-aiobotocore-workmailmessageflow-module"></a>

# WorkMailMessageFlowClient for aiobotocore WorkMailMessageFlow module

> [Index](../README.md) > [WorkMailMessageFlow](./README.md) >
> WorkMailMessageFlowClient

Auto-generated documentation for
[WorkMailMessageFlow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow)
type annotations stubs module
[types-aiobotocore-workmailmessageflow](https://pypi.org/project/types-aiobotocore-workmailmessageflow/).

- [WorkMailMessageFlowClient for aiobotocore WorkMailMessageFlow module](#workmailmessageflowclient-for-aiobotocore-workmailmessageflow-module)
  - [WorkMailMessageFlowClient](#workmailmessageflowclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_raw_message_content](#get_raw_message_content)
    - [put_raw_message_content](#put_raw_message_content)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="workmailmessageflowclient"></a>

## WorkMailMessageFlowClient

Type annotations for `session.create_client("workmailmessageflow")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_workmailmessageflow.client import WorkMailMessageFlowClient

session = get_session()
async with session.create_client("workmailmessageflow") as client:
    client: WorkMailMessageFlowClient
```

Boto3 documentation:
[WorkMailMessageFlow.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_workmailmessageflow.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InvalidContentLocation`
- `Exceptions.MessageFrozen`
- `Exceptions.MessageRejected`
- `Exceptions.ResourceNotFoundException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

WorkMailMessageFlowClient exceptions.

Type annotations for `session.create_client("workmailmessageflow").exceptions`
method.

Boto3 documentation:
[WorkMailMessageFlow.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`session.create_client("workmailmessageflow").can_paginate` method.

Boto3 documentation:
[WorkMailMessageFlow.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("workmailmessageflow").generate_presigned_url` method.

Boto3 documentation:
[WorkMailMessageFlow.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_raw\_message\_content"></a>

### get_raw_message_content

Retrieves the raw content of an in-transit email message, in MIME format.

Type annotations for
`session.create_client("workmailmessageflow").get_raw_message_content` method.

Boto3 documentation:
[WorkMailMessageFlow.Client.get_raw_message_content](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client.get_raw_message_content)

Asynchronous method. Use `await get_raw_message_content(...)` for a synchronous
call.

Arguments mapping described in
[GetRawMessageContentRequestRequestTypeDef](./type_defs.md#getrawmessagecontentrequestrequesttypedef).

Keyword-only arguments:

- `messageId`: `str` *(required)*

Returns a `Coroutine` for
[GetRawMessageContentResponseTypeDef](./type_defs.md#getrawmessagecontentresponsetypedef).

<a id="put\_raw\_message\_content"></a>

### put_raw_message_content

Updates the raw content of an in-transit email message, in MIME format.

Type annotations for
`session.create_client("workmailmessageflow").put_raw_message_content` method.

Boto3 documentation:
[WorkMailMessageFlow.Client.put_raw_message_content](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client.put_raw_message_content)

Asynchronous method. Use `await put_raw_message_content(...)` for a synchronous
call.

Arguments mapping described in
[PutRawMessageContentRequestRequestTypeDef](./type_defs.md#putrawmessagecontentrequestrequesttypedef).

Keyword-only arguments:

- `messageId`: `str` *(required)*
- `content`:
  [RawMessageContentTypeDef](./type_defs.md#rawmessagecontenttypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("workmailmessageflow").__aenter__`
method.

Boto3 documentation:
[WorkMailMessageFlow.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[WorkMailMessageFlowClient](#workmailmessageflowclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("workmailmessageflow").__aexit__`
method.

Boto3 documentation:
[WorkMailMessageFlow.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
