<a id="examples-for-aiobotocore-cognitosync-module"></a>

# Examples for aiobotocore CognitoSync module

> [Index](../README.md) > [CognitoSync](./README.md) > Examples

- [Examples for aiobotocore CognitoSync module](#examples-for-aiobotocore-cognitosync-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cognito-sync]` package installed.

Write your `CognitoSync` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CognitoSyncClient
# and provides type checking and code completion
async with session.create_client("cognito-sync") as client:
    
    # result has type BulkPublishResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.bulk_publish()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cognito-sync]` or a standalone
`types_aiobotocore_cognito_sync` package, you have to explicitly specify
`client: CognitoSyncClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cognito_sync.client import CognitoSyncClient
from types_aiobotocore_cognito_sync.type_defs import BulkPublishResponseTypeDef






session = get_session()

async with session.create_client("cognito-sync") as client:
    client: CognitoSyncClient

    
    result: BulkPublishResponseTypeDef = client.bulk_publish()
    

    

    
```
