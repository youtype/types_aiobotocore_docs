<a id="examples-for-aiobotocore-resiliencehub-module"></a>

# Examples for aiobotocore ResilienceHub module

> [Index](../README.md) > [ResilienceHub](./README.md) > Examples

- [Examples for aiobotocore ResilienceHub module](#examples-for-aiobotocore-resiliencehub-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[resiliencehub]` package installed.

Write your `ResilienceHub` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ResilienceHubClient
# and provides type checking and code completion
async with session.create_client("resiliencehub") as client:
    
    # result has type AddDraftAppVersionResourceMappingsResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_draft_app_version_resource_mappings()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[resiliencehub]` or a standalone
`types_aiobotocore_resiliencehub` package, you have to explicitly specify
`client: ResilienceHubClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_resiliencehub.client import ResilienceHubClient
from types_aiobotocore_resiliencehub.type_defs import AddDraftAppVersionResourceMappingsResponseTypeDef






session = get_session()

async with session.create_client("resiliencehub") as client:
    client: ResilienceHubClient

    
    result: AddDraftAppVersionResourceMappingsResponseTypeDef = client.add_draft_app_version_resource_mappings()
    

    

    
```
