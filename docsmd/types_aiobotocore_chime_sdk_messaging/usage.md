# Examples

> [Index](../README.md) > [ChimeSDKMessaging](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ChimeSDKMessaging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
    type annotations stubs module [types-aiobotocore-chime-sdk-messaging](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[chime-sdk-messaging]` package installed.

Write your `ChimeSDKMessaging` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("chime-sdk-messaging") as client:  # (1)
        result = await client.batch_create_channel_membership()  # (2)
    ```

    1. client: [ChimeSDKMessagingClient](./client.md)
    2. result: [:material-code-braces: BatchCreateChannelMembershipResponseTypeDef](./type_defs.md#batchcreatechannelmembershipresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[chime-sdk-messaging]`
or a standalone `types_aiobotocore_chime_sdk_messaging` package, you have to explicitly specify
`client: ChimeSDKMessagingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_chime_sdk_messaging.client import ChimeSDKMessagingClient
    from types_aiobotocore_chime_sdk_messaging.type_defs import BatchCreateChannelMembershipResponseTypeDef
    from types_aiobotocore_chime_sdk_messaging.type_defs import BatchCreateChannelMembershipRequestRequestTypeDef


    session = get_session()

    async with session.create_client("chime-sdk-messaging") as client:
        client: ChimeSDKMessagingClient
        kwargs: BatchCreateChannelMembershipRequestRequestTypeDef = {...}
        result: BatchCreateChannelMembershipResponseTypeDef = await client.batch_create_channel_membership(**kwargs)
    ```




