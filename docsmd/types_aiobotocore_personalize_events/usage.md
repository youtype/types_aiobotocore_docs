# Examples

> [Index](../README.md) > [PersonalizeEvents](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PersonalizeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#personalizeevents)
    type annotations stubs module [types-aiobotocore-personalize-events](https://pypi.org/project/types-aiobotocore-personalize-events/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[personalize-events]` package installed.

Write your `PersonalizeEvents` code as usual,
type checking and code completion should work out of the box.



```python
# PersonalizeEventsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("personalize-events") as client:  # (1)
    result = await client.put_action_interactions()  # (2)
```

1. client: [PersonalizeEventsClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[personalize-events]`
or a standalone `types_aiobotocore_personalize_events` package, you have to explicitly specify
`client: PersonalizeEventsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PersonalizeEventsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_personalize_events.client import PersonalizeEventsClient
from types_aiobotocore_personalize_events.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_personalize_events.type_defs import PutActionInteractionsRequestTypeDef


session = get_session()

async with session.create_client("personalize-events") as client:
    client: PersonalizeEventsClient
    kwargs: PutActionInteractionsRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.put_action_interactions(**kwargs)
```




