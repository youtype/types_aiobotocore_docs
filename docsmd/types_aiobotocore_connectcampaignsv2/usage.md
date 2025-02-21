# Examples

> [Index](../README.md) > [ConnectCampaignServiceV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ConnectCampaignServiceV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaignsv2.html#connectcampaignservicev2)
    type annotations stubs module [types-aiobotocore-connectcampaignsv2](https://pypi.org/project/types-aiobotocore-connectcampaignsv2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[connectcampaignsv2]` package installed.

Write your `ConnectCampaignServiceV2` code as usual,
type checking and code completion should work out of the box.



```python
# ConnectCampaignServiceV2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("connectcampaignsv2") as client:  # (1)
    result = await client.create_campaign()  # (2)
```

1. client: [ConnectCampaignServiceV2Client](./client.md)
2. result: [:material-code-braces: CreateCampaignResponseTypeDef](./type_defs.md#createcampaignresponsetypedef) 



```python
# ListCampaignsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("connectcampaignsv2") as client:  # (1)
    paginator = client.get_paginator("list_campaigns")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ConnectCampaignServiceV2Client](./client.md)
2. paginator: [ListCampaignsPaginator](./paginators.md#listcampaignspaginator)
3. item: [:material-code-braces: ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[connectcampaignsv2]`
or a standalone `types_aiobotocore_connectcampaignsv2` package, you have to explicitly specify
`client: ConnectCampaignServiceV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ConnectCampaignServiceV2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_connectcampaignsv2.client import ConnectCampaignServiceV2Client
from types_aiobotocore_connectcampaignsv2.type_defs import CreateCampaignResponseTypeDef
from types_aiobotocore_connectcampaignsv2.type_defs import CreateCampaignRequestTypeDef


session = get_session()

async with session.create_client("connectcampaignsv2") as client:
    client: ConnectCampaignServiceV2Client
    kwargs: CreateCampaignRequestTypeDef = {...}
    result: CreateCampaignResponseTypeDef = await client.create_campaign(**kwargs)
```



```python
# ListCampaignsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_connectcampaignsv2.client import ConnectCampaignServiceV2Client
from types_aiobotocore_connectcampaignsv2.paginator import ListCampaignsPaginator
from types_aiobotocore_connectcampaignsv2.type_defs import ListCampaignsResponseTypeDef


session = get_session()

async with session.create_client("connectcampaignsv2") as client:
    client: ConnectCampaignServiceV2Client
    paginator: ListCampaignsPaginator = client.get_paginator("list_campaigns")
    async for item in paginator.paginate(...):
        item: ListCampaignsResponseTypeDef
        print(item)
```


