# Examples

> [Index](../README.md) > [EventBridge](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EventBridge](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
    type annotations stubs module [types-aiobotocore-events](https://pypi.org/project/types-aiobotocore-events/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[events]` package installed.

Write your `EventBridge` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("events") as client:  # (1)
        result = await client.cancel_replay()  # (2)
    ```

    1. client: [EventBridgeClient](./client.md)
    2. result: [:material-code-braces: CancelReplayResponseTypeDef](./type_defs.md#cancelreplayresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("events") as client:  # (1)
        paginator = client.get_paginator("list_rule_names_by_target")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [EventBridgeClient](./client.md)
    2. paginator: [ListRuleNamesByTargetPaginator](./paginators.md#listrulenamesbytargetpaginator)
    3. item: [:material-code-braces: ListRuleNamesByTargetResponseTypeDef](./type_defs.md#listrulenamesbytargetresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[events]`
or a standalone `types_aiobotocore_events` package, you have to explicitly specify
`client: EventBridgeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_events.client import EventBridgeClient
    from types_aiobotocore_events.type_defs import CancelReplayResponseTypeDef
    from types_aiobotocore_events.type_defs import CancelReplayRequestRequestTypeDef


    session = get_session()

    async with session.create_client("events") as client:
        client: EventBridgeClient
        kwargs: CancelReplayRequestRequestTypeDef = {...}
        result: CancelReplayResponseTypeDef = await client.cancel_replay(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_events.client import EventBridgeClient
    from types_aiobotocore_events.paginator import ListRuleNamesByTargetPaginator
    from types_aiobotocore_events.type_defs import ListRuleNamesByTargetResponseTypeDef


    session = get_session()

    async with session.create_client("events") as client:
        client: EventBridgeClient
        paginator: ListRuleNamesByTargetPaginator = client.get_paginator("list_rule_names_by_target")
        async for item in paginator.paginate(...):
            item: ListRuleNamesByTargetResponseTypeDef
            print(item)
    ```

