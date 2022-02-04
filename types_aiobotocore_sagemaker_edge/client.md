<a id="sagemakeredgemanagerclient-for-aiobotocore-sagemakeredgemanager-module"></a>

# SagemakerEdgeManagerClient for aiobotocore SagemakerEdgeManager module

> [Index](..) > [SagemakerEdgeManager](.) > SagemakerEdgeManagerClient

Auto-generated documentation for
[SagemakerEdgeManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
type annotations stubs module
[types-aiobotocore-sagemaker-edge](https://pypi.org/project/types-aiobotocore-sagemaker-edge/).

- [SagemakerEdgeManagerClient for aiobotocore SagemakerEdgeManager module](#sagemakeredgemanagerclient-for-aiobotocore-sagemakeredgemanager-module)
  - [SagemakerEdgeManagerClient](#sagemakeredgemanagerclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_device_registration](#get_device_registration)
    - [send_heartbeat](#send_heartbeat)

<a id="sagemakeredgemanagerclient"></a>

## SagemakerEdgeManagerClient

Type annotations for `aiobotocore.create_client("sagemaker-edge")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_sagemaker_edge.client import SagemakerEdgeManagerClient

def get_sagemaker-edge_client() -> SagemakerEdgeManagerClient:
    return Session().client("sagemaker-edge")
```

Boto3 documentation:
[SagemakerEdgeManager.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_sagemaker_edge.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InternalServiceException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

SagemakerEdgeManagerClient exceptions.

Type annotations for `aiobotocore.create_client("sagemaker-edge").exceptions`
method.

Boto3 documentation:
[SagemakerEdgeManager.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("sagemaker-edge").can_paginate`
method.

Boto3 documentation:
[SagemakerEdgeManager.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("sagemaker-edge").generate_presigned_url` method.

Boto3 documentation:
[SagemakerEdgeManager.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_device_registration"></a>

### get_device_registration

Use to check if a device is registered with SageMaker Edge Manager.

Type annotations for
`aiobotocore.create_client("sagemaker-edge").get_device_registration` method.

Boto3 documentation:
[SagemakerEdgeManager.Client.get_device_registration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client.get_device_registration)

Asynchronous method. Use `await get_device_registration(...)` for a synchronous
call.

Arguments mapping described in
[GetDeviceRegistrationRequestRequestTypeDef](./type_defs.md#getdeviceregistrationrequestrequesttypedef).

Keyword-only arguments:

- `DeviceName`: `str` *(required)*
- `DeviceFleetName`: `str` *(required)*

Returns a `Coroutine` for
[GetDeviceRegistrationResultTypeDef](./type_defs.md#getdeviceregistrationresulttypedef).

<a id="send_heartbeat"></a>

### send_heartbeat

Use to get the current status of devices registered on SageMaker Edge Manager.

Type annotations for
`aiobotocore.create_client("sagemaker-edge").send_heartbeat` method.

Boto3 documentation:
[SagemakerEdgeManager.Client.send_heartbeat](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client.send_heartbeat)

Asynchronous method. Use `await send_heartbeat(...)` for a synchronous call.

Arguments mapping described in
[SendHeartbeatRequestRequestTypeDef](./type_defs.md#sendheartbeatrequestrequesttypedef).

Keyword-only arguments:

- `AgentVersion`: `str` *(required)*
- `DeviceName`: `str` *(required)*
- `DeviceFleetName`: `str` *(required)*
- `AgentMetrics`:
  `Sequence`\[[EdgeMetricTypeDef](./type_defs.md#edgemetrictypedef)\]
- `Models`: `Sequence`\[[ModelTypeDef](./type_defs.md#modeltypedef)\]
