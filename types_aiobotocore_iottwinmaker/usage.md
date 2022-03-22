<a id="examples-for-aiobotocore-iottwinmaker-module"></a>

# Examples for aiobotocore IoTTwinMaker module

> [Index](../README.md) > [IoTTwinMaker](./README.md) > Examples

- [Examples for aiobotocore IoTTwinMaker module](#examples-for-aiobotocore-iottwinmaker-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iottwinmaker]` package installed.

Write your `IoTTwinMaker` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoTTwinMakerClient
# and provides type checking and code completion
async with session.create_client("iottwinmaker") as client:
    
    # result has type BatchPutPropertyValuesResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_put_property_values()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iottwinmaker]` or a standalone
`types_aiobotocore_iottwinmaker` package, you have to explicitly specify
`client: IoTTwinMakerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iottwinmaker.client import IoTTwinMakerClient
from types_aiobotocore_iottwinmaker.type_defs import BatchPutPropertyValuesResponseTypeDef






session = get_session()

async with session.create_client("iottwinmaker") as client:
    client: IoTTwinMakerClient

    
    result: BatchPutPropertyValuesResponseTypeDef = client.batch_put_property_values()
    

    

    
```
