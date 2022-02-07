<a id="augmentedairuntimeclient-for-aiobotocore-augmentedairuntime-module"></a>

# AugmentedAIRuntimeClient for aiobotocore AugmentedAIRuntime module

> [Index](..) > [AugmentedAIRuntime](.) > AugmentedAIRuntimeClient

Auto-generated documentation for
[AugmentedAIRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
type annotations stubs module
[types-aiobotocore-sagemaker-a2i-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime/).

- [AugmentedAIRuntimeClient for aiobotocore AugmentedAIRuntime module](#augmentedairuntimeclient-for-aiobotocore-augmentedairuntime-module)
  - [AugmentedAIRuntimeClient](#augmentedairuntimeclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [delete_human_loop](#delete_human_loop)
    - [describe_human_loop](#describe_human_loop)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_human_loops](#list_human_loops)
    - [start_human_loop](#start_human_loop)
    - [stop_human_loop](#stop_human_loop)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="augmentedairuntimeclient"></a>

## AugmentedAIRuntimeClient

Type annotations for `session.create_client("sagemaker-a2i-runtime")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_sagemaker_a2i_runtime.client import AugmentedAIRuntimeClient

session = get_session()
async with session.create_client("sagemaker-a2i-runtime") as client:
    client: AugmentedAIRuntimeClient
```

Boto3 documentation:
[AugmentedAIRuntime.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_sagemaker_a2i_runtime.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

AugmentedAIRuntimeClient exceptions.

Type annotations for
`session.create_client("sagemaker-a2i-runtime").exceptions` method.

Boto3 documentation:
[AugmentedAIRuntime.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`session.create_client("sagemaker-a2i-runtime").can_paginate` method.

Boto3 documentation:
[AugmentedAIRuntime.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="delete_human_loop"></a>

### delete_human_loop

Deletes the specified human loop for a flow definition.

Type annotations for
`session.create_client("sagemaker-a2i-runtime").delete_human_loop` method.

Boto3 documentation:
[AugmentedAIRuntime.Client.delete_human_loop](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.delete_human_loop)

Asynchronous method. Use `await delete_human_loop(...)` for a synchronous call.

Arguments mapping described in
[DeleteHumanLoopRequestRequestTypeDef](./type_defs.md#deletehumanlooprequestrequesttypedef).

Keyword-only arguments:

- `HumanLoopName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_human_loop"></a>

### describe_human_loop

Returns information about the specified human loop.

Type annotations for
`session.create_client("sagemaker-a2i-runtime").describe_human_loop` method.

Boto3 documentation:
[AugmentedAIRuntime.Client.describe_human_loop](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.describe_human_loop)

Asynchronous method. Use `await describe_human_loop(...)` for a synchronous
call.

Arguments mapping described in
[DescribeHumanLoopRequestRequestTypeDef](./type_defs.md#describehumanlooprequestrequesttypedef).

Keyword-only arguments:

- `HumanLoopName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeHumanLoopResponseTypeDef](./type_defs.md#describehumanloopresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("sagemaker-a2i-runtime").generate_presigned_url` method.

Boto3 documentation:
[AugmentedAIRuntime.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_human_loops"></a>

### list_human_loops

Returns information about human loops, given the specified parameters.

Type annotations for
`session.create_client("sagemaker-a2i-runtime").list_human_loops` method.

Boto3 documentation:
[AugmentedAIRuntime.Client.list_human_loops](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.list_human_loops)

Asynchronous method. Use `await list_human_loops(...)` for a synchronous call.

Arguments mapping described in
[ListHumanLoopsRequestRequestTypeDef](./type_defs.md#listhumanloopsrequestrequesttypedef).

Keyword-only arguments:

- `FlowDefinitionArn`: `str` *(required)*
- `CreationTimeAfter`: `Union`\[`datetime`, `str`\]
- `CreationTimeBefore`: `Union`\[`datetime`, `str`\]
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListHumanLoopsResponseTypeDef](./type_defs.md#listhumanloopsresponsetypedef).

<a id="start_human_loop"></a>

### start_human_loop

Starts a human loop, provided that at least one activation condition is met.

Type annotations for
`session.create_client("sagemaker-a2i-runtime").start_human_loop` method.

Boto3 documentation:
[AugmentedAIRuntime.Client.start_human_loop](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.start_human_loop)

Asynchronous method. Use `await start_human_loop(...)` for a synchronous call.

Arguments mapping described in
[StartHumanLoopRequestRequestTypeDef](./type_defs.md#starthumanlooprequestrequesttypedef).

Keyword-only arguments:

- `HumanLoopName`: `str` *(required)*
- `FlowDefinitionArn`: `str` *(required)*
- `HumanLoopInput`:
  [HumanLoopInputTypeDef](./type_defs.md#humanloopinputtypedef) *(required)*
- `DataAttributes`:
  [HumanLoopDataAttributesTypeDef](./type_defs.md#humanloopdataattributestypedef)

Returns a `Coroutine` for
[StartHumanLoopResponseTypeDef](./type_defs.md#starthumanloopresponsetypedef).

<a id="stop_human_loop"></a>

### stop_human_loop

Stops the specified human loop.

Type annotations for
`session.create_client("sagemaker-a2i-runtime").stop_human_loop` method.

Boto3 documentation:
[AugmentedAIRuntime.Client.stop_human_loop](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.stop_human_loop)

Asynchronous method. Use `await stop_human_loop(...)` for a synchronous call.

Arguments mapping described in
[StopHumanLoopRequestRequestTypeDef](./type_defs.md#stophumanlooprequestrequesttypedef).

Keyword-only arguments:

- `HumanLoopName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="__aenter__"></a>

### __aenter__

Type annotations for
`session.create_client("sagemaker-a2i-runtime").__aenter__` method.

Boto3 documentation:
[AugmentedAIRuntime.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[AugmentedAIRuntimeClient](#augmentedairuntimeclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("sagemaker-a2i-runtime").__aexit__`
method.

Boto3 documentation:
[AugmentedAIRuntime.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for
`session.create_client("sagemaker-a2i-runtime").get_paginator` method with
overloads.

- `client.get_paginator("list_human_loops")` ->
  [ListHumanLoopsPaginator](./paginators.md#listhumanloopspaginator)
