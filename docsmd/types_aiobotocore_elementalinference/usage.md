# Examples

> [Index](../README.md) > [ElementalInference](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ElementalInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference.html#elementalinference)
    type annotations stubs module [types-aiobotocore-elementalinference](https://pypi.org/project/types-aiobotocore-elementalinference/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[elementalinference]` package installed.

Write your `ElementalInference` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ElementalInferenceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elementalinference") as client:  # (1)
    result = await client.associate_feed()  # (2)
```

1. client: [ElementalInferenceClient](./client.md)
2. result: [:material-code-braces: AssociateFeedResponseTypeDef](./type_defs.md#associatefeedresponsetypedef)



#### Paginator usage example

```python
# ListFeedsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elementalinference") as client:  # (1)
    paginator = client.get_paginator("list_feeds")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ElementalInferenceClient](./client.md)
2. paginator: [ListFeedsPaginator](./paginators.md#listfeedspaginator)
3. item: [:material-code-braces: ListFeedsResponseTypeDef](./type_defs.md#listfeedsresponsetypedef)



#### Waiter usage example

```python
# FeedDeletedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elementalinference") as client:  # (1)
    waiter = client.get_waiter("feed_deleted")  # (2)
    await waiter.wait(...)
```

1. client: [ElementalInferenceClient](./client.md)
2. waiter: [FeedDeletedWaiter](./waiters.md#feeddeletedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[elementalinference]`
or a standalone `types_aiobotocore_elementalinference` package, you have to explicitly specify
`client: ElementalInferenceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ElementalInferenceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elementalinference.client import ElementalInferenceClient
from types_aiobotocore_elementalinference.type_defs import AssociateFeedResponseTypeDef
from types_aiobotocore_elementalinference.type_defs import AssociateFeedRequestTypeDef


session = get_session()

async with session.create_client("elementalinference") as client:
    client: ElementalInferenceClient
    kwargs: AssociateFeedRequestTypeDef = {...}
    result: AssociateFeedResponseTypeDef = await client.associate_feed(**kwargs)
```



#### Paginator usage example

```python
# ListFeedsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elementalinference.client import ElementalInferenceClient
from types_aiobotocore_elementalinference.paginator import ListFeedsPaginator
from types_aiobotocore_elementalinference.type_defs import ListFeedsResponseTypeDef


session = get_session()

async with session.create_client("elementalinference") as client:
    client: ElementalInferenceClient
    paginator: ListFeedsPaginator = client.get_paginator("list_feeds")
    async for item in paginator.paginate(...):
        item: ListFeedsResponseTypeDef
        print(item)
```



#### Waiter usage example

```python
# FeedDeletedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elementalinference.client import ElementalInferenceClient
from types_aiobotocore_elementalinference.waiter import FeedDeletedWaiter


session = get_session()

async with session.create_client("elementalinference") as client:
    client: ElementalInferenceClient
    waiter: FeedDeletedWaiter = client.get_waiter("feed_deleted")
    await waiter.wait(...)
```
