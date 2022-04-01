# Examples

> [Index](../README.md) > [LexModelsV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LexModelsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
    type annotations stubs module [types-aiobotocore-lexv2-models](https://pypi.org/project/types-aiobotocore-lexv2-models/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[lexv2-models]` package installed.

Write your `LexModelsV2` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("lexv2-models") as client:  # (1)
        result = await client.build_bot_locale()  # (2)
    ```

    1. client: [LexModelsV2Client](./client.md)
    2. result: [:material-code-braces: BuildBotLocaleResponseTypeDef](./type_defs.md#buildbotlocaleresponsetypedef) 





=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("lexv2-models") as client:  # (1)
        waiter = client.get_waiter("bot_alias_available")  # (2)
        await waiter.wait()
    ```

    1. client: [LexModelsV2Client](./client.md)
    2. waiter: [BotAliasAvailableWaiter](./waiters.md#botaliasavailablewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[lexv2-models]`
or a standalone `types_aiobotocore_lexv2_models` package, you have to explicitly specify
`client: LexModelsV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_lexv2_models.client import LexModelsV2Client
    from types_aiobotocore_lexv2_models.type_defs import BuildBotLocaleResponseTypeDef
    from types_aiobotocore_lexv2_models.type_defs import BuildBotLocaleRequestRequestTypeDef


    session = get_session()

    async with session.create_client("lexv2-models") as client:
        client: LexModelsV2Client
        kwargs: BuildBotLocaleRequestRequestTypeDef = {...}
        result: BuildBotLocaleResponseTypeDef = await client.build_bot_locale(**kwargs)
    ```





=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_lexv2_models.client import LexModelsV2Client
    from types_aiobotocore_lexv2_models.waiter import BotAliasAvailableWaiter


    session = get_session()

    async with session.create_client("lexv2-models") as client:
        client: LexModelsV2Client
        waiter: BotAliasAvailableWaiter = client.get_waiter("bot_alias_available")
        await waiter.wait()
    ```
