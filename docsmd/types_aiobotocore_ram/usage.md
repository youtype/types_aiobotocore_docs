# Examples

> [Index](../README.md) > [RAM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#ram)
    type annotations stubs module [types-aiobotocore-ram](https://pypi.org/project/types-aiobotocore-ram/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ram]` package installed.

Write your `RAM` code as usual,
type checking and code completion should work out of the box.



```python
# RAMClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ram") as client:  # (1)
    result = await client.accept_resource_share_invitation()  # (2)
```

1. client: [RAMClient](./client.md)
2. result: [:material-code-braces: AcceptResourceShareInvitationResponseTypeDef](./type_defs.md#acceptresourceshareinvitationresponsetypedef) 



```python
# GetResourcePoliciesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ram") as client:  # (1)
    paginator = client.get_paginator("get_resource_policies")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [RAMClient](./client.md)
2. paginator: [GetResourcePoliciesPaginator](./paginators.md#getresourcepoliciespaginator)
3. item: [:material-code-braces: GetResourcePoliciesResponseTypeDef](./type_defs.md#getresourcepoliciesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[ram]`
or a standalone `types_aiobotocore_ram` package, you have to explicitly specify
`client: RAMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# RAMClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ram.client import RAMClient
from types_aiobotocore_ram.type_defs import AcceptResourceShareInvitationResponseTypeDef
from types_aiobotocore_ram.type_defs import AcceptResourceShareInvitationRequestTypeDef


session = get_session()

async with session.create_client("ram") as client:
    client: RAMClient
    kwargs: AcceptResourceShareInvitationRequestTypeDef = {...}
    result: AcceptResourceShareInvitationResponseTypeDef = await client.accept_resource_share_invitation(**kwargs)
```



```python
# GetResourcePoliciesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ram.client import RAMClient
from types_aiobotocore_ram.paginator import GetResourcePoliciesPaginator
from types_aiobotocore_ram.type_defs import GetResourcePoliciesResponseTypeDef


session = get_session()

async with session.create_client("ram") as client:
    client: RAMClient
    paginator: GetResourcePoliciesPaginator = client.get_paginator("get_resource_policies")
    async for item in paginator.paginate(...):
        item: GetResourcePoliciesResponseTypeDef
        print(item)
```


