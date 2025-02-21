# Examples

> [Index](../README.md) > [Macie2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Macie2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#macie2)
    type annotations stubs module [types-aiobotocore-macie2](https://pypi.org/project/types-aiobotocore-macie2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[macie2]` package installed.

Write your `Macie2` code as usual,
type checking and code completion should work out of the box.



```python
# Macie2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("macie2") as client:  # (1)
    result = await client.batch_get_custom_data_identifiers()  # (2)
```

1. client: [Macie2Client](./client.md)
2. result: [:material-code-braces: BatchGetCustomDataIdentifiersResponseTypeDef](./type_defs.md#batchgetcustomdataidentifiersresponsetypedef) 



```python
# DescribeBucketsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("macie2") as client:  # (1)
    paginator = client.get_paginator("describe_buckets")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [DescribeBucketsPaginator](./paginators.md#describebucketspaginator)
3. item: [:material-code-braces: DescribeBucketsResponseTypeDef](./type_defs.md#describebucketsresponsetypedef) 



```python
# FindingRevealedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("macie2") as client:  # (1)
    waiter = client.get_waiter("finding_revealed")  # (2)
    await waiter.wait()
```

1. client: [Macie2Client](./client.md)
2. waiter: [FindingRevealedWaiter](./waiters.md#findingrevealedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[macie2]`
or a standalone `types_aiobotocore_macie2` package, you have to explicitly specify
`client: Macie2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# Macie2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_macie2.client import Macie2Client
from types_aiobotocore_macie2.type_defs import BatchGetCustomDataIdentifiersResponseTypeDef
from types_aiobotocore_macie2.type_defs import BatchGetCustomDataIdentifiersRequestTypeDef


session = get_session()

async with session.create_client("macie2") as client:
    client: Macie2Client
    kwargs: BatchGetCustomDataIdentifiersRequestTypeDef = {...}
    result: BatchGetCustomDataIdentifiersResponseTypeDef = await client.batch_get_custom_data_identifiers(**kwargs)
```



```python
# DescribeBucketsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_macie2.client import Macie2Client
from types_aiobotocore_macie2.paginator import DescribeBucketsPaginator
from types_aiobotocore_macie2.type_defs import DescribeBucketsResponseTypeDef


session = get_session()

async with session.create_client("macie2") as client:
    client: Macie2Client
    paginator: DescribeBucketsPaginator = client.get_paginator("describe_buckets")
    async for item in paginator.paginate(...):
        item: DescribeBucketsResponseTypeDef
        print(item)
```



```python
# FindingRevealedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_macie2.client import Macie2Client
from types_aiobotocore_macie2.waiter import FindingRevealedWaiter


session = get_session()

async with session.create_client("macie2") as client:
    client: Macie2Client
    waiter: FindingRevealedWaiter = client.get_waiter("finding_revealed")
    await waiter.wait()
```
