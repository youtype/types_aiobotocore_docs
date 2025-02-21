# Examples

> [Index](../README.md) > [PartnerCentralSellingAPI](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PartnerCentralSellingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#partnercentralsellingapi)
    type annotations stubs module [types-aiobotocore-partnercentral-selling](https://pypi.org/project/types-aiobotocore-partnercentral-selling/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[partnercentral-selling]` package installed.

Write your `PartnerCentralSellingAPI` code as usual,
type checking and code completion should work out of the box.



```python
# PartnerCentralSellingAPIClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("partnercentral-selling") as client:  # (1)
    result = await client.accept_engagement_invitation()  # (2)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListEngagementByAcceptingInvitationTasksPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("partnercentral-selling") as client:  # (1)
    paginator = client.get_paginator("list_engagement_by_accepting_invitation_tasks")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. paginator: [ListEngagementByAcceptingInvitationTasksPaginator](./paginators.md#listengagementbyacceptinginvitationtaskspaginator)
3. item: [:material-code-braces: ListEngagementByAcceptingInvitationTasksResponseTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[partnercentral-selling]`
or a standalone `types_aiobotocore_partnercentral_selling` package, you have to explicitly specify
`client: PartnerCentralSellingAPIClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PartnerCentralSellingAPIClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_selling.client import PartnerCentralSellingAPIClient
from types_aiobotocore_partnercentral_selling.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_partnercentral_selling.type_defs import AcceptEngagementInvitationRequestTypeDef


session = get_session()

async with session.create_client("partnercentral-selling") as client:
    client: PartnerCentralSellingAPIClient
    kwargs: AcceptEngagementInvitationRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.accept_engagement_invitation(**kwargs)
```



```python
# ListEngagementByAcceptingInvitationTasksPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_selling.client import PartnerCentralSellingAPIClient
from types_aiobotocore_partnercentral_selling.paginator import ListEngagementByAcceptingInvitationTasksPaginator
from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementByAcceptingInvitationTasksResponseTypeDef


session = get_session()

async with session.create_client("partnercentral-selling") as client:
    client: PartnerCentralSellingAPIClient
    paginator: ListEngagementByAcceptingInvitationTasksPaginator = client.get_paginator("list_engagement_by_accepting_invitation_tasks")
    async for item in paginator.paginate(...):
        item: ListEngagementByAcceptingInvitationTasksResponseTypeDef
        print(item)
```


