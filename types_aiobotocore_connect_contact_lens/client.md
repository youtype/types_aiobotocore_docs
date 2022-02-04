<a id="connectcontactlensclient-for-aiobotocore-connectcontactlens-module"></a>

# ConnectContactLensClient for aiobotocore ConnectContactLens module

> [Index](..) > [ConnectContactLens](.) > ConnectContactLensClient

Auto-generated documentation for
[ConnectContactLens](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
type annotations stubs module
[types-aiobotocore-connect-contact-lens](https://pypi.org/project/types-aiobotocore-connect-contact-lens/).

- [ConnectContactLensClient for aiobotocore ConnectContactLens module](#connectcontactlensclient-for-aiobotocore-connectcontactlens-module)
  - [ConnectContactLensClient](#connectcontactlensclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_realtime_contact_analysis_segments](#list_realtime_contact_analysis_segments)

<a id="connectcontactlensclient"></a>

## ConnectContactLensClient

Type annotations for `aiobotocore.create_client("connect-contact-lens")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_connect_contact_lens.client import ConnectContactLensClient

def get_connect-contact-lens_client() -> ConnectContactLensClient:
    return Session().client("connect-contact-lens")
```

Boto3 documentation:
[ConnectContactLens.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_connect_contact_lens.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.InternalServiceException`
- `Exceptions.InvalidRequestException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ThrottlingException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ConnectContactLensClient exceptions.

Type annotations for
`aiobotocore.create_client("connect-contact-lens").exceptions` method.

Boto3 documentation:
[ConnectContactLens.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`aiobotocore.create_client("connect-contact-lens").can_paginate` method.

Boto3 documentation:
[ConnectContactLens.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("connect-contact-lens").generate_presigned_url`
method.

Boto3 documentation:
[ConnectContactLens.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_realtime_contact_analysis_segments"></a>

### list_realtime_contact_analysis_segments

Provides a list of analysis segments for a real-time analysis session.

Type annotations for
`aiobotocore.create_client("connect-contact-lens").list_realtime_contact_analysis_segments`
method.

Boto3 documentation:
[ConnectContactLens.Client.list_realtime_contact_analysis_segments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens.Client.list_realtime_contact_analysis_segments)

Asynchronous method. Use `await list_realtime_contact_analysis_segments(...)`
for a synchronous call.

Arguments mapping described in
[ListRealtimeContactAnalysisSegmentsRequestRequestTypeDef](./type_defs.md#listrealtimecontactanalysissegmentsrequestrequesttypedef).

Keyword-only arguments:

- `InstanceId`: `str` *(required)*
- `ContactId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListRealtimeContactAnalysisSegmentsResponseTypeDef](./type_defs.md#listrealtimecontactanalysissegmentsresponsetypedef).
