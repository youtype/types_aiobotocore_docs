<a id="examples-for-aiobotocore-kendra-module"></a>

# Examples for aiobotocore kendra module

> [Index](../README.md) > [kendra](./README.md) > Examples

- [Examples for aiobotocore kendra module](#examples-for-aiobotocore-kendra-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[kendra]` package installed.

Write your `kendra` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type kendraClient
# and provides type checking and code completion
async with session.create_client("kendra") as client:
    
    # result has type AssociateEntitiesToExperienceResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_entities_to_experience()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[kendra]` or a standalone
`types_aiobotocore_kendra` package, you have to explicitly specify
`client: kendraClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_kendra.client import kendraClient
from types_aiobotocore_kendra.type_defs import AssociateEntitiesToExperienceResponseTypeDef






session = get_session()

async with session.create_client("kendra") as client:
    client: kendraClient

    
    result: AssociateEntitiesToExperienceResponseTypeDef = client.associate_entities_to_experience()
    

    

    
```
