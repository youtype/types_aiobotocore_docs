<a id="examples-for-aiobotocore-lexmodelsv2-module"></a>

# Examples for aiobotocore LexModelsV2 module

> [Index](../README.md) > [LexModelsV2](./README.md) > Examples

- [Examples for aiobotocore LexModelsV2 module](#examples-for-aiobotocore-lexmodelsv2-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[lexv2-models]` package installed.

Write your `LexModelsV2` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type LexModelsV2Client
# and provides type checking and code completion
async with session.create_client("lexv2-models") as client:
    
    # result has type BuildBotLocaleResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.build_bot_locale()
    

    

    
    # waiter has type BotAliasAvailableWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("bot_alias_available")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[lexv2-models]` or a standalone
`types_aiobotocore_lexv2_models` package, you have to explicitly specify
`client: LexModelsV2Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_lexv2_models.client import LexModelsV2Client
from types_aiobotocore_lexv2_models.type_defs import BuildBotLocaleResponseTypeDef

from types_aiobotocore_lexv2_models.waiter import BotAliasAvailableWaiter

from types_aiobotocore_lexv2_models.literals import WaiterName


session = get_session()

async with session.create_client("lexv2-models") as client:
    client: LexModelsV2Client

    
    result: BuildBotLocaleResponseTypeDef = client.build_bot_locale()
    

    

    
    waiter_name: WaiterName = "bot_alias_available"
    waiter: BotAliasAvailableWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
