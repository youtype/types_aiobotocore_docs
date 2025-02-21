# Examples

> [Index](../README.md) > [CognitoSync](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CognitoSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#cognitosync)
    type annotations stubs module [types-aiobotocore-cognito-sync](https://pypi.org/project/types-aiobotocore-cognito-sync/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cognito-sync]` package installed.

Write your `CognitoSync` code as usual,
type checking and code completion should work out of the box.



```python
# CognitoSyncClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cognito-sync") as client:  # (1)
    result = await client.bulk_publish()  # (2)
```

1. client: [CognitoSyncClient](./client.md)
2. result: [:material-code-braces: BulkPublishResponseTypeDef](./type_defs.md#bulkpublishresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[cognito-sync]`
or a standalone `types_aiobotocore_cognito_sync` package, you have to explicitly specify
`client: CognitoSyncClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CognitoSyncClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cognito_sync.client import CognitoSyncClient
from types_aiobotocore_cognito_sync.type_defs import BulkPublishResponseTypeDef
from types_aiobotocore_cognito_sync.type_defs import BulkPublishRequestTypeDef


session = get_session()

async with session.create_client("cognito-sync") as client:
    client: CognitoSyncClient
    kwargs: BulkPublishRequestTypeDef = {...}
    result: BulkPublishResponseTypeDef = await client.bulk_publish(**kwargs)
```




