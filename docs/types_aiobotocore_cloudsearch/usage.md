<a id="examples-for-aiobotocore-cloudsearch-module"></a>

# Examples for aiobotocore CloudSearch module

> [Index](../README.md) > [CloudSearch](./README.md) > Examples

- [Examples for aiobotocore CloudSearch module](#examples-for-aiobotocore-cloudsearch-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cloudsearch]` package installed.

Write your `CloudSearch` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CloudSearchClient
# and provides type checking and code completion
async with session.create_client("cloudsearch") as client:
    
    # result has type BuildSuggestersResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.build_suggesters()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cloudsearch]` or a standalone
`types_aiobotocore_cloudsearch` package, you have to explicitly specify
`client: CloudSearchClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudsearch.client import CloudSearchClient
from types_aiobotocore_cloudsearch.type_defs import BuildSuggestersResponseTypeDef






session = get_session()

async with session.create_client("cloudsearch") as client:
    client: CloudSearchClient

    
    result: BuildSuggestersResponseTypeDef = client.build_suggesters()
    

    

    
```
