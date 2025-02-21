# Examples

> [Index](../README.md) > [Route53](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Route53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#route53)
    type annotations stubs module [types-aiobotocore-route53](https://pypi.org/project/types-aiobotocore-route53/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[route53]` package installed.

Write your `Route53` code as usual,
type checking and code completion should work out of the box.



```python
# Route53Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("route53") as client:  # (1)
    result = await client.activate_key_signing_key()  # (2)
```

1. client: [Route53Client](./client.md)
2. result: [:material-code-braces: ActivateKeySigningKeyResponseTypeDef](./type_defs.md#activatekeysigningkeyresponsetypedef) 



```python
# ListCidrBlocksPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("route53") as client:  # (1)
    paginator = client.get_paginator("list_cidr_blocks")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListCidrBlocksPaginator](./paginators.md#listcidrblockspaginator)
3. item: [:material-code-braces: ListCidrBlocksResponseTypeDef](./type_defs.md#listcidrblocksresponsetypedef) 



```python
# ResourceRecordSetsChangedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("route53") as client:  # (1)
    waiter = client.get_waiter("resource_record_sets_changed")  # (2)
    await waiter.wait()
```

1. client: [Route53Client](./client.md)
2. waiter: [ResourceRecordSetsChangedWaiter](./waiters.md#resourcerecordsetschangedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[route53]`
or a standalone `types_aiobotocore_route53` package, you have to explicitly specify
`client: Route53Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# Route53Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_route53.client import Route53Client
from types_aiobotocore_route53.type_defs import ActivateKeySigningKeyResponseTypeDef
from types_aiobotocore_route53.type_defs import ActivateKeySigningKeyRequestTypeDef


session = get_session()

async with session.create_client("route53") as client:
    client: Route53Client
    kwargs: ActivateKeySigningKeyRequestTypeDef = {...}
    result: ActivateKeySigningKeyResponseTypeDef = await client.activate_key_signing_key(**kwargs)
```



```python
# ListCidrBlocksPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_route53.client import Route53Client
from types_aiobotocore_route53.paginator import ListCidrBlocksPaginator
from types_aiobotocore_route53.type_defs import ListCidrBlocksResponseTypeDef


session = get_session()

async with session.create_client("route53") as client:
    client: Route53Client
    paginator: ListCidrBlocksPaginator = client.get_paginator("list_cidr_blocks")
    async for item in paginator.paginate(...):
        item: ListCidrBlocksResponseTypeDef
        print(item)
```



```python
# ResourceRecordSetsChangedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_route53.client import Route53Client
from types_aiobotocore_route53.waiter import ResourceRecordSetsChangedWaiter


session = get_session()

async with session.create_client("route53") as client:
    client: Route53Client
    waiter: ResourceRecordSetsChangedWaiter = client.get_waiter("resource_record_sets_changed")
    await waiter.wait()
```
