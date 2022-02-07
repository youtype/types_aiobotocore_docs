<a id="route53recoveryclusterclient-for-aiobotocore-route53recoverycluster-module"></a>

# Route53RecoveryClusterClient for aiobotocore Route53RecoveryCluster module

> [Index](..) > [Route53RecoveryCluster](.) > Route53RecoveryClusterClient

Auto-generated documentation for
[Route53RecoveryCluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
type annotations stubs module
[types-aiobotocore-route53-recovery-cluster](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster/).

- [Route53RecoveryClusterClient for aiobotocore Route53RecoveryCluster module](#route53recoveryclusterclient-for-aiobotocore-route53recoverycluster-module)
  - [Route53RecoveryClusterClient](#route53recoveryclusterclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_routing_control_state](#get_routing_control_state)
    - [update_routing_control_state](#update_routing_control_state)
    - [update_routing_control_states](#update_routing_control_states)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)

<a id="route53recoveryclusterclient"></a>

## Route53RecoveryClusterClient

Type annotations for `session.create_client("route53-recovery-cluster")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_route53_recovery_cluster.client import Route53RecoveryClusterClient

session = get_session()
async with session.create_client("route53-recovery-cluster") as client:
    client: Route53RecoveryClusterClient
```

Boto3 documentation:
[Route53RecoveryCluster.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_route53_recovery_cluster.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.EndpointTemporarilyUnavailableException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

Route53RecoveryClusterClient exceptions.

Type annotations for
`session.create_client("route53-recovery-cluster").exceptions` method.

Boto3 documentation:
[Route53RecoveryCluster.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`session.create_client("route53-recovery-cluster").can_paginate` method.

Boto3 documentation:
[Route53RecoveryCluster.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("route53-recovery-cluster").generate_presigned_url`
method.

Boto3 documentation:
[Route53RecoveryCluster.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_routing_control_state"></a>

### get_routing_control_state

Get the state for a routing control.

Type annotations for
`session.create_client("route53-recovery-cluster").get_routing_control_state`
method.

Boto3 documentation:
[Route53RecoveryCluster.Client.get_routing_control_state](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.get_routing_control_state)

Asynchronous method. Use `await get_routing_control_state(...)` for a
synchronous call.

Arguments mapping described in
[GetRoutingControlStateRequestRequestTypeDef](./type_defs.md#getroutingcontrolstaterequestrequesttypedef).

Keyword-only arguments:

- `RoutingControlArn`: `str` *(required)*

Returns a `Coroutine` for
[GetRoutingControlStateResponseTypeDef](./type_defs.md#getroutingcontrolstateresponsetypedef).

<a id="update_routing_control_state"></a>

### update_routing_control_state

Set the state of the routing control to reroute traffic.

Type annotations for
`session.create_client("route53-recovery-cluster").update_routing_control_state`
method.

Boto3 documentation:
[Route53RecoveryCluster.Client.update_routing_control_state](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.update_routing_control_state)

Asynchronous method. Use `await update_routing_control_state(...)` for a
synchronous call.

Arguments mapping described in
[UpdateRoutingControlStateRequestRequestTypeDef](./type_defs.md#updateroutingcontrolstaterequestrequesttypedef).

Keyword-only arguments:

- `RoutingControlArn`: `str` *(required)*
- `RoutingControlState`:
  [RoutingControlStateType](./literals.md#routingcontrolstatetype) *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_routing_control_states"></a>

### update_routing_control_states

Set multiple routing control states.

Type annotations for
`session.create_client("route53-recovery-cluster").update_routing_control_states`
method.

Boto3 documentation:
[Route53RecoveryCluster.Client.update_routing_control_states](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.update_routing_control_states)

Asynchronous method. Use `await update_routing_control_states(...)` for a
synchronous call.

Arguments mapping described in
[UpdateRoutingControlStatesRequestRequestTypeDef](./type_defs.md#updateroutingcontrolstatesrequestrequesttypedef).

Keyword-only arguments:

- `UpdateRoutingControlStateEntries`:
  `Sequence`\[[UpdateRoutingControlStateEntryTypeDef](./type_defs.md#updateroutingcontrolstateentrytypedef)\]
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="__aenter__"></a>

### __aenter__

Type annotations for
`session.create_client("route53-recovery-cluster").__aenter__` method.

Boto3 documentation:
[Route53RecoveryCluster.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[Route53RecoveryClusterClient](#route53recoveryclusterclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for
`session.create_client("route53-recovery-cluster").__aexit__` method.

Boto3 documentation:
[Route53RecoveryCluster.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
