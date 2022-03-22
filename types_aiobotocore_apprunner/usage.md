<a id="examples-for-aiobotocore-apprunner-module"></a>

# Examples for aiobotocore AppRunner module

> [Index](../README.md) > [AppRunner](./README.md) > Examples

- [Examples for aiobotocore AppRunner module](#examples-for-aiobotocore-apprunner-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[apprunner]` package installed.

Write your `AppRunner` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AppRunnerClient
# and provides type checking and code completion
async with session.create_client("apprunner") as client:
    
    # result has type AssociateCustomDomainResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_custom_domain()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[apprunner]` or a standalone
`types_aiobotocore_apprunner` package, you have to explicitly specify
`client: AppRunnerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_apprunner.client import AppRunnerClient
from types_aiobotocore_apprunner.type_defs import AssociateCustomDomainResponseTypeDef






session = get_session()

async with session.create_client("apprunner") as client:
    client: AppRunnerClient

    
    result: AssociateCustomDomainResponseTypeDef = client.associate_custom_domain()
    

    

    
```
